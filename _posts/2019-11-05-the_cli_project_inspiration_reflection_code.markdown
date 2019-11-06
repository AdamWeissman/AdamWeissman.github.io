---
layout: post
title:      "The CLI Project: Inspiration, Reflection, Code."
date:       2019-11-05 06:04:44 -0500
permalink:  the_cli_project_inspiration_reflection_code
---

**THIS PART IS ABOUT THANKS, AND INSPIRATION -- SKIP IT IF YOU WANT JUST THE PART ABOUT CODING.**

So, before I get into this retrospective, I want to show special thanks to the people that made this project possible.  There is former Flatiron student Sammy Steiner who inpsired me to THINK BIG.  I never got to meet Sammy, but when I saw the CLI Project looming on the horizon I started watching "show and tells", and googling around for CLI project.  I thought wouldn't it be cool if you could animate something from the CLI, but was uncertain if it was even possible.  [Sammy Steiner's blog post](https://sammysteiner.github.io/blog/2017/04/13/bringing-terminal-applications-to-life-cli-animations-with-ruby/) captured my imagination.  Thanks to my friend Ryan Louie, an artist/animator who helped me brainstorm a better 'product'.  And, most of all thanks to instructor Beth Schofield whose patience and instruction made it possible for me to create this project, and become confident that I could.

In my "past life," I had been an aspiring writer.  I wasn't the kind of dude to spend 7 years on a single script, but due to the nature of 'writing' it was ALWAYS possible to doubt whether a project was finished... plague yourself with questions like: how might I say this better; or differently; or not at all; or something else entirely. I was almost going to bring that handicap to the world of code -- and I probably would have -- except, Beth (who had been a musician before a coder) made it clear that I needed to forget all that if I wanted to thrive.

Below is a 'walkthrough' of me using the program.

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/Pm98ZQAE9t4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</center>

**THIS PART IS MY REFLECTION OF THE LEARNING EXPERIENCE --- SKIP IT IF YOU WANT JUST THE PART ABOUT CODING.**

Before I got to the CLI project there, I was a bit terrified.  I felt like there was too much hand-holding on the labs thanks (or no thanks) to RSPEC which made it nary impossible to get beyond the feeling that I was reassembling someone else's puzzle.  Anyways, as I had accelerated through a jungle of labs, I began to worry whether or not I would become more lost OR if I would just get to the other side more quickly...

Long story short... I made it to the other side, (more quickly).

And, I discovered that nearly all of the significant learning took place during the project.

It's not to say I don't value RSPEC, I do, but I suspect I would probably get more out of it if I wrote them myself.  I realize I'm not at the point in my knowledge, so it's sort of a moot point... but I can't help but feel (even now) that many of those labs were more like 'detours' than 'treacherous roads' (treacherous roads where you grow from the experience).

**FINALLY... ABOUT THAT CODE...**

The Narrabot.

What is it?

It scrapes [read.gov's aesop's fables](http://www.read.gov/aesop/001.html) in order to grab the table of contents (titles and links) as the first part of the Story Object... and then it will scrape each of the stories on demand.  It uses the user selection as the determining factor of which story to scrape (on demand).

It attempts to mimic natural language processing -- at least to the extent that it uses a reglar expression to make it seem that way.  For example:

```
def search_for_yes(get_input) #helper for yes_or_no
      get_input.to_s.match? /yes|yep|yeah|yah|\by$|okay|ok|fine|of course|please|would|more|sure|why not|wonderful|awesome|great|maybe yes|alright|like/i
    end
```

The code I'm probably most proud of, although it's probably terrible -- is plays_and_puts:

```
def play_and_puts(a_string)
    too_long_to_be_trapped_in_audio = a_string.split
    if too_long_to_be_trapped_in_audio.count >= 26 #words
      break_up_the_text = a_string.split("\n")
      "Heads up! This story is #{too_long_to_be_trapped_in_audio.count.to_s} words long. You'll be prompted if a passage is more than 25 words.".play ("en")
      print "CLOSED CAPTIONING: " + "This story is #{too_long_to_be_trapped_in_audio.count.to_s} words long. You'll be prompted if a passage is more than 25 words." + "\n"
      break_up_the_text.each do |section|

        if section.split.count <= 25
          "#{section}".play ("en")
          print "CLOSED CAPTIONING: " + section + "\n"
        else
          puts "\n"
          puts "...may I go on? "
          input = gets.chomp
          if yes_or_no(input) || (input == "") || (input == " ") || (input == "  ")
            puts ""
            "#{section}".play ("en")
            print "CLOSED CAPTIONING: " + section + "\n"
          else
            break
          end
        end

      end
    else
      "#{a_string}".play ("en")
      print "CLOSED CAPTIONING: " + a_string + "\n"
  end
```

It started off as a refactor of all the times I was typing out the .play method and the puts method in tandem.  But, as you can't escape from audio (the TTS gem) once it starts, I added some conditional logic that would prompt the user to continue or not, thus giving them the opportunity to escape.

The object orientation which was the reason for the project is probably the "cleanest" code.

```
class Narrabot::Story
  attr_reader :title, :the_link
  attr_accessor :the_text, :the_moral, :text_and_moral, :parting_moral

  @@table_of_contents = []
  @@morals = []

  def initialize(title, link)
    @title = title
    @the_link = link
    @@table_of_contents << self
  end

  def self.table_of_contents
    @@table_of_contents
  end

  def parting_moral=(x)
    @@morals << x
  end

  def self.morals
    @@morals
  end

end
```

It's relatively "self.explanatory" (bad joke) except the def parting_moral and @@morals.  That code is used at the end of the program... so, upon exiting, the user is reminded of a "random" moral sampled from a story they listened to.  If you listened to a dozen stories, one moral comes back to haunt you when you quit.

The other OO concept I attempted was a module.

My CLI was becoming a mess, so I created a module called helper elves to "include" in the CLI.  It wasn't working and I almost abandoned the effort to include a module until I realized the answer lay in the order of which I was requiring stuff in my environment,rb file; something I didn't think mattered but will now never forget that it does.

In the meanwhile am looking forward to the gauntlet/review.




