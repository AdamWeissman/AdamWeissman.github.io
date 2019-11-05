---
layout: post
title:      "The CLI Project: Inspiration, Reflection, Code."
date:       2019-11-05 06:04:44 -0500
permalink:  the_cli_project_inspiration_reflection_code
---

**THIS PART IS ABOUT THANKS, AND INSPIRATION -- SKIP IT IF YOU WANT JUST THE PART ABOUT CODING.**

So, before I get into this retrospective, I want to show special thanks to the people that made this project possible.  There is former Flatiron student Sammy Steiner who inpsired me to THINK BIG.  I never got to meet Sammy, but when I saw the CLI Project looming on the horizon I started watching "show and tells", and googling around for CLI project.  I thought wouldn't it be cool if you could animate something from the CLI, but was uncertain if it was even possible.  [Sammy Steiner's blog post](https://sammysteiner.github.io/blog/2017/04/13/bringing-terminal-applications-to-life-cli-animations-with-ruby/) captured my imagination.  Thanks to my friend Ryan Louie, an artist/animator who helped me brainstorm a better 'product'.  And, most of all thanks to instructor Beth Schofield whose patience and instruction made it possible for me to create this project, and become confident that I could.

In my "past life," I had been an aspiring screenwriter/novelist.  I even had a manager.  I wasn't the kind of dude to spend 7 years on a single project, but due to the nature of 'writing' it was always possible to doubt whether a project was finished; how might I say this better; or differently; or not at all; or something else entirely... I was almost going to bring that handicap to the world of code -- and I probably would have -- except, Beth (who had been a musician before a coder) made it clear that I needed to forget all that if I wanted to thrive.

Lastly, and I probably shouldn't include the next 'Thanks' (because it may seem spiteful) BUT it was HUGE part of why you see the project as it is.  You see, I almost decided NOT to include the animation at all.  The project was done and I felt ready to move on to Sinatra and beyond... except, while discussing projects with other students, I was told "no offense, but your project is a toy."  Of course I was -- offended that is.  But, neither could I be mad at the student for they were trying to help me... and neither could I be mad because my project IS a toy.

So I thought to myself about toys and had the realization that if I were building a toy (which I was), that it should be as novel as I could make it within the confines of the project.  I also had the realization that even toys have value.  To the people that use them, and those who create them.  Do I marvel more at the creator of Krazy Glue or The Slinky.  Perhaps both inventions pale in comparison to the creator of The Pet Rock, for that genius sold us all what was free and became a millionaire in the process -- all for seeing the world a little bit differently.  Kind of like Steve Jobs.

Strangely, that off the cuff comment inspired quite the revelation: that if I could have been one of the creators of GoLang (the Programming Language developed at Google), or a creator on Pokémon Go... well, I'd rather have been part of Pokémon Go.  And as the word TOY reverberated inside my skill I was reminded of Steven Johnson's book *Wonderland: How Play Made the Modern World.*  The thesis of the book may be debatable, but as Johnson's perspective spans history and shows how [The Mechanical Turk ](https://en.wikipedia.org/wiki/The_Turk), (a toy) was the first link in a chain that reached through Charles Babbage to: IBM's Deep Blue which became Watson.  You might even say "full circle!" as you point to Amazon's Mechanical Turk, brainchild of Jeff Bezos -- inspired by... a toy.

Long story short, had I not consiously and fully embraced that this project is/was a toy.  It would not have the animation it does had I not been forced to view it so.  And, if I were to refactor this, or start from scratch.  I think I'd probably just build a fortune telling chatbot that employed tricks snatched from mentalism, things like: "picture a large animal, it is grey, etc etc"... until... "were you thinking of an elephant?" or "imagine two very simple shapes, the first that come to mind... really DO it NOW  Visualize one as VIOLET and the other as YELLOW.  One shape inside the other... did you picture a circle and a triangle?" ... that sort of thing.

Below is a 'walkthrough' of me using the program.

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/Pm98ZQAE9t4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</center>

**THIS PART IS MY REFLECTION OF THE LEARNING EXPERIENCE --- SKIP IT IF YOU WANT JUST THE PART ABOUT CODING.**

Before I got to the CLI project there, I was a bit terrified.  I felt like there was too much hand-holding on the labs thanks (or no thanks) to RSPEC which made it nary impossible to get beyond the feeling that I was reassembling someone else's puzzle.  Anyways, as I had accelerated through a jungle of labs, I began to worry whether or not I would become more lost OR if I would just get to the other side more quickly...

Long story short... I made it to the other side, more quickly.  Instead of grabbing at every empty canteen or rusty machete that littered 'the jungle' floor, and attempting to carry them all (and dying in the process) I discovered there was a shopping mall just over the ridge.

Looking back from the food court...  I realize it wasn't a jungle of information, but a desert.

For struggling to decipher the design of someone else's code (through RSPEC) seems a little bit like admiring pyramids and ruins and then attempting to do it backwards.  There were also mirages, fill-in-the-blank, guess-wildly-until-blank-is-filled-in, and fill-in-the-blank that felt like victories only if they remained unexamined.  

Thus the real oasis of knowledge was The Project.

I only wish I had gotten there sooner.  For the project, it wasn't a matter of guessing until I got it right (maybe a little) but having to decide whether or not I would abandon a feature if I couldn't do it, or learning how.

In the course of labs, I perceived Instructors as Priests on High.  The Ask a Question button as something vaguely shameful.  Like the button rats press to get a pellet of sweets in their cage -- only, you don't always get the sweet.  Sometimes you get nothing, or a piece of a salt... and you have to struggle on The Wheel until you can come back later and press the button again (only more desperately).

On the project however, the instructors became Mentors and Allies.  Heroes to emulate and learn from.  Squad leaders in the trenches and on the front line.

Maintaining the battle analogy: labs versus projects; labs are like training in a swamp where you might die of malaria or end up with a rotten foot.  Projects on the other hand are for real.  Maybe you'll get killed and have to drop out.  On the other hand, maybe you'll get wounded (and you probably should), but at least then you're a veteran.  Still a rookie, still a beginner, but at least you know the quest has really begun. 


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




