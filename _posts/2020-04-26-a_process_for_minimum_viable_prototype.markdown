---
layout: post
title:      "A Process for Minimum Viable Prototype"
date:       2020-04-26 16:59:04 +0000
permalink:  a_process_for_minimum_viable_prototype
---


When we typically talk about an MVP (or minimum viable product) we typically have "the Lean Version" in mind.  But, as revealed in Marty Cagan's book "Inspired: How to Create Tech Products Customer's Love", Cagan makes the concept of MVP much more concrete, and it starts with thinking: "Minimum Viable Prototype" as opposed to a "Minimum Viable Product."

At first blush, it seems like only the change of a word... but actually, when you consider something in the context of a prototype as opposed to a product, it is extremely liberating.  Consider: a product is something you ship, something that users can be expected to use, something with all the necessary validations and authentications and security features and layers upon layers of functionality that a protoype DOES NOT NEED.  A prototype on the other hand proves only that some such "solution" CAN work.  The MVP as it is typically approached has all the unnecessary bells and whistles that will not matter if it never gets used, it is considered the minumum standard of a product.  The Minimum Viable Prototype on the otherhand reveals THE REASON of why the finished product should actually be built.  To illustrate the point, a typical "minimum viable product" may be approached as a new shell for a Lamborghini with all of last years parts.  A minimum viable prototype might only be the modified engine.  To illustrate the point from a movie: in James Cameron's "Terminator 2" the minimum viable prototype might be: The terminator's skeleton hand salvaged from T1, the hand that was held in cyberdyne's vault and used by Miles Dyson to reverse engineer the monster.

For students working through Flatiron's Software Engineering curriculum, you might find this line of thinking helpful when desiging your projects.  Taking my lead from Miles Dyson: an MVP is not necessarily the easiest thing for me to build, but the smallest element or hologram that reveals the larger application of what can be.   For students it is easy to fall intot he trap of assuming an MVP should be the easiest and the fastest thing to build, but to me that seems a dangerous habit of priorities to fall into.  While it's often advocated that we complete an MVP and not go far beyond the base requirements, consider if the thing that appears to be a Stretch Goal is actually your reason for building the project.  If it is, don't get bogged down in trying to build out every single error message for something that you will NOT use, nor anyone else.  If the project is effectively just a product to get someone to see your potential as an engieer, then don't build a template.  And if you do build a template, let the viewer be impressed by something other than it's a template.  Let it be memorable.  Push yourself.  And always be aware what exactly and MVP is and MVP for.  (which is why I find Cagan's explanation and book so helpful).

--

With that in mind, I'm documenting my process for planning out an JS Rails Project.  It will probably seem ambitious and perhaps "the opposite" of what an MVP is typically described (or interpreted) as.  That said, if I expect it to be something that I as a novice programmer can build solo in less than a month... then it's probably not a stretch to think it really is an MVP; sure in the context of me as a novice, it may be more than an MVP... but in the context of the world, IT IS, and I would rather judge a finished product by the scales and standards of the world as opposed to the limits of my ability.  Considering competition in the broadest sense will force me to stretch and grow.  Considering competition to be only with myself might be good for today and tomorrow, but perhaps useless in planning the long term if I never consider what I'm aiming for.  To illustrate the point: does the kid that grows up to be a pro-athlete judge themselves only by how good they are Today and Tomorrow, or do they judge Today and Tomorrow in the Context of how they might ultimately be judged.  So, if I suspect something will take me a month with my limited ability and limited time, I try to think how fast a professional programmer at Google, or HP,  IBM, Amazon, or Facebook might be able to build it... one week?  If it were two programmers, perhaps 2-3 days?  

-- 

**STEP 1 -- THE PROBLEM AND A COMMON SENSE SOLUTION**
I started off with two "life problems" that seem to generalize to parents with kids 4-years of age and under... I haven't "quantified" the problem with market research, only verbally with other parents and their own experiences.
1) We (parents) want to make sure the media that our kids consume is educational and engaging... or at least not totally moronic.
2) We (parents) dislike sticky fingers handling the computer keyboard (drool and crumbs are a bad combo with electronics); this second is a problem because kids seem to prefer adult electronics to their own toys.

My non-technical solution was: a game that allows kids (under 4) to learn letters and words on a desktop without messing up the keyboard.

**STEP 2 -- CONSIDER DIFFERENT WAYS THE COMMON SENSE SOLUTION MIGHT BE IMPLEMENTED... SEARCH FOR THE EASIEST (AND MOST NOVEL)... ALSO CONSIDER CONSTRAINTS.**
Imagine my ideal solution and then look to see if it exists, how accessible or expensive something similar is.. and research associated technologies that might make "my ideal" possible if it doesn't exist (or if it does, but isn't very captivating).  Always consider everything within "Real World Constraints".

**STEP 3 -- CREATE A USER STORY (Overview of how it "could" most likely work)**
  ((below is my user story))
Basically the user gets to the landing page, is asked for the name and a dozen or so words to learn.  (The parent would type the kids name in and a handful of words).

The words are parsed into unique individual letters. Only the letters that comprised the words selected are entered into rotation.. 

The game begins, a Siri-type voice asks “$NAME point to the letter ‘A’” (there’s no text).  The screen is divided into two panels, the letter “A” on one side, some other random letter on the other.  Using motion capture, the computer camera would know whether or not the kid is pointing to the correct letter (to the left or right side of the screen).

Once enough points have been accrued on the letters that make up a word “CAR” for instance.  The game would add into rotation something like “Point to the word CAR. C. A. R.”

And the whole thing would just cycle through until the user closed the browser, or they got a congratulations message.

Would be easy to scale the game up to include sentences once everything else was working, and maybe even an animated avatar that stands in the center of the screen and would look at or point to the correct letter if too much time elapsed.

Points would be accrued by how fast the letter or word is pointed to, and taken out of rotation when a certain threshold is reached.

**STEP 4 - VISUALIZE THE USER EXPERIENCE AND SHALLOW "MECHANIC" TO MAKE IT WORK**

[THIS IS THE VISUALIZATION](https://pdfhost.io/v/23h.NFmLP_Kids_Letter_Gamepdf.pdf)

**STEP 5 - EXECUTION**
Code the ugly version from step 4, low focus on interface, error handling, and edge cases, high focus on getting "the mechanic" to work.

--

As a final thought/hope... I think of the early days of Steven Spielberg, George Lucas, John Milius, Dennis Hopper, and beyond... a generation of filmmakers that came up together.  My wish for those of us at Flatiron is not only that we find someone to pair program with, or create an above average portfolio... but that we might discover cofounders to build visions.


