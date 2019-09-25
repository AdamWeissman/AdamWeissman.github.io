---
layout: post
title:      "TOC for Software, Abstract Whiteboard Session 1"
date:       2019-09-25 07:56:34 -0400
permalink:  toc_for_software_abstract_whiteboard_session_1
---


This blog is basically a recap of the first (of hopefully many) whiteboarding experiences.  The focus is on the process, with as little commentary as possible.

NOTE: TOC is often talked about in the context of large scale projects, in which there are "work flow pipelines" and multiple teams.  In modifying the Theory of Constraints for individual problems (to boil it down from what you see above) -- we basically cycle through three perspectives on a given problem (in the context of a goal).  At it's most basic, those perspectives are matters of classification, correlation, and effect-cause-effect.  Read about it here [Theory of Constraints Book](https://www.amazon.com/dp/B0029IEYHQ/ref=cm_sw_em_r_mt_dp_U_Y-ZIDbRMW67DE)

One more quick note before you dive into this: this is basically a transcription, so please read carefully or you may get lost.

So, for the whiteboarding session we started off with a sort of abstract goal.  Since we're beginners we defined that goal as:  

> To speedily create/develop a CLI project (or other portfolio project) with *the least* amount of hiccups along the way.

We then listed what we considered to be constraints -- things that were holding us back from being able to accomplish the above goal.  In other words: the obstacles.  We listed them randomly, as they came to us.  The original order was as follows:

> * We are unfamiliar with the best practices (syntax, libraries, etc)
> * Unsure of where to begin
> * Uncertain of what the program does
> * Uncertain of the necessary inputs
> * Uncertain which data structures to use, eg hashes vs arrays etc
> * Uncertain of control flow
> * General concern that "I might accidentally be developing a lousy user experience"
> 

At this point, we tried to determine how we were classifying things, to make sure we understood what we had written.  This was not a redundant step.  In doing so, we realized the last item on the unordered list: the general concern that we might be developing a lousy user experience was actually something to be included in the original goal.  In other words, we revised the original goal to read:

> To speedily create/develop a CLI project (or other portfolio project) with *the least* amount of hiccups along the way.  AND have it be good!

Thus, the unordered list newly looked as follows:

> * We are unfamiliar with the best practices (syntax, libraries, etc)
> * Unsure of where to begin
> * Uncertain of what the program does
> * Uncertain of the necessary inputs
> * Uncertain which data structures to use, eg hashes vs arrays etc
> * Uncertain of control flow
> 

From there we went through the list, commenting on each item.  It's important to note, that given we have imperfect knowledge about how to rank each item, our goal at this point could be more clearly described as trying to 

> *  **Unsure of where to begin** *1) Let's begin here, and NO this is obviously not the final step necessary to accomlishing the goal.  However, it will likely become a byproduct of everything else.*
> * **We are unfamiliar with the best practices (syntax, libraries, etc)** *2) This also doesn't really matter... if the project works, it works.  As beginners, trying to figure out what the 'best practices' are when we don't have the knowledge base to make those judgements is an unneccessary obstacle.*
> * **Uncertain of what the program does** AND **Uncertain of the necessary inputs** *3) These two items seem to have a cause and effect relationship*
> * **Uncertain of control flow** *4) This will be dependent on the stuff in "3"*
> * **Uncertain which data structures to use, eg hashes vs arrays etc** *5) This will also be dependent on the stuff in step 3 *
>

Going through this process made us realize that being "Uncertain of What the Program Does" and being "Uncertain of The Necessary Inputs" were really the most important thing -- and one in the same.  Also, it was THE PLACE to begin.  While it's obvious in hindsight, and even as "common sense", it was interesting to discover/recognize how many other perceived problems were sources of procrastination and debilitation.

From there we rephrased this:

> * **Uncertain of what the program does** AND **Uncertain of the necessary inputs**
>

with the following commentary...

"We're not sure of all the outputs, nor all of the inputs, BUT!!!  Having a list (even if only partially complete) of the outputs (to the user) will inform us:

> * What inputs are necessary 
> * How they might be stored 
> * In what order they might be stored 
> * In what order the program will process them
> * Some idea of the associated best practices.
>

After that we had a new goal:

> Determine final outputs, in order to determine dependencies and preconditions
> 

That lead us to the constraint/problem of the whole **"WHERE TO BEGIN" ISSUE** striking/rising again.  So, we reframed the goal.  With the following commentary:  Knowing where to being IS NOT the issue actual... the actual issue is assuming that we need to determine the "absolutely final" outputs.

With that in mind, the replacement goal became

> Listing ANYTHING that we might need
> 

the implicit idea being that we could then try to figure out Effect-Cause-Effect relationships, and that would be sufficient enough to build a skeleton and then as a byproduct determine what blanks to fill in.

So, the NEW "new goal" became:

> List the possible ingredients/building blocks, with a "mind" or "eye" for what the user might experience.
> 

The problem/obstacle/constraint here was:

> "How will we know whether or not an ingredient or building block is relevant?"
> 

We were able to answer that pretty quickly with:

> It will be relevant if it serves as a link from one thing to another, and also that it should be testable (it should work) if the "to"/"from" or "before"/"after" code is written.
> 

Here we came to a bit of a hiccup.  Since we had been working on an abstract problem we didn't know whether or not we should then solve a "real problem" like TicTacToe or something concrete.  We were concerned that we'd be able to "cheat" a solution if we were working on a problem that we had already done in a lab.  With that in mind, we thought we'd might as well try something abstract and see if it could be ordered into something logical.  What follows are the "What the Program Does Requirements" as they were rattled off:

> * The user can type X
> * The program modifies X, Y, Z
> * In order to modify X, it needs Y
> * The value of Y must already be stored
> * The program loads with Z
> * A,B,C can all "happen" to X
> * In order for A,B,C to happen, the program must check X&Y
> * The user gets back "H" after X is modified
> 

There was a moment where we were at a stand still,uncertain whether to progress from here -- if it was even possible, given there was no actual logic to what we came up with.  How might we even attempt to rank these?  In the spirit of the session we decided to trust in the process and look for dependencies. 

We decided we would rank the items with/by multiples of "10" so it would be easy to insert additional steps if anything seemed to be missing after prioritization.  We came away with the following.  I bolded two additional steps, italicized stuff we thought we'd need to keep track of, and bolded commentary.

> * 10 The user can type X
> * 20 The program modifies X, Y, Z
> * 30 In order to modify X, ***it needs Y***  <- **-1**
> * -10The value of Y must already be stored
> * -20 The program loads with Z ) **-15** **Y is loaded with Z**
> * 40 A,B,C can all "happen" to X **5** **A,B,C** **must all exist prior to the user typing X**
> * 35 In order for A,B,C to happen, the program must check *X&Y  **X will depend on 10 AND Y will depend on -10***
> * 50 The user gets back "H" after X is modified
> 

The biggest surprise came when put it into order, instead of using the multiples of 10, we just ranked as steps in order -- and broke certain implicit ideas down for example: knowing that A, B, C needed to exist, we decided to define A, B, C as separate steps:

> 1. The Program Loads with Z
> 2. Y Loads with Z or shortly thereafter... it may depend on a random condition caused by Z
> 3. Y is ready for use
> 4. A,B,C, must exist
> 5. Define A
> 6. Define B
> 7. Define C 
> 8. User types X
> 9. Program modifies X, Y, Z
> 10. It uses Y to modify X
>  11. But Y is also changed (**we added this**)
>  12. Z is also changed (**we added this**) **and we noted that if Y is part of Z -- perhaps an array, then we only need to change Z... maybe**
>  13. A, B, C can happen to X
>  14. A(X) **add this**
>  15. B(X) **add this**
>  16. C(X) **add this**
>  17. "H" (or 14,15,or16)  is returned
>  

Some additional notes we added when our final goal became "What else is missing?" was:

* we may need additional logic to determine what causes A, B, or C
* we realized that the item ranked "35" did not need to be included in the 1-17 steps because the linear process made the note (35) implicit
* we also realized that steps 1&2 could possibly be combined as long as "y" can be specifically referenced
* we realized that step 3 might be redundant
* also reaized that steps 4-7 could not be tested until step 10
* also that steps 13-16 could be if/else statements in a single function, or perhaps separate functions depending on complexity.

The biggest takeaway, surprise, of this particular whiteboarding sessions was that we were able to work towards a concrete solution despite dealing with random conditions on a completely abstract problem.

Thanks for reading.  If you found this interesting or problematic please message me on slack AdamWeissman so I can make sure the next whiteboarding session is even more productive.  It occurs to me that there is always the potential pitfall of groupthink when dealing with the inertia of a group activity -- so any thoughts are appreciated! 

