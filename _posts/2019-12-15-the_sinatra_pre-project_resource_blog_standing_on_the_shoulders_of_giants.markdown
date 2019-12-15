---
layout: post
title:      "The Sinatra Pre-Project Resource Blog; Standing on the Shoulders of Giants"
date:       2019-12-15 09:25:13 -0500
permalink:  the_sinatra_pre-project_resource_blog_standing_on_the_shoulders_of_giants
---

**ACKNOWLEDGMENTS** I believe it’s important to give credit where credit is due, and the blog post you're about to read would not be possible without instructor Ayana Zaire and fellow student Daniel Dawson.  To make a long story short (and to avoid an introduction that would be repetitive of my comments on the Slack channel): the repl below was built 

<iframe height="400px" width="100%" src="https://repl.it/@AdamWeissman/Learnmagazine?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

Essentially it was entirely built by Daniel.  It allows you to search the Flatiron Learn Magazine using a keyword in the title of a blog post.  You could swap out 'Sinatra' for 'Rails' or 'CLI', and all the blogs featuring the keyword in the title will come up.  

To expand your query, just change the numeral in the constant URL listed in the repl.  NOTE: for this post, I only did two pages of Sinatra Blogs, and despite curating the ones I found most helpful, the immenseness of all that's 'out there' is overwhelming.  My apologies for blogs I missed, there's too much great stuff out there for one person too curate.  But hopefully someone might be as inspired as me and do a sequel to this blog.

This post would not have been possible without the repl above, but also I wouldn't have thought to do it without Ayana's suggestion of compiling useful resources in place.

**THANK YOU.**: Having access to all the Sinatra blogs has not only reaffirmed my conviction of how important they are, but having that access has made me feel indebted to the students that came before me -- to all those students that hacked their way through the jungles of code.  And not only did they hack through it, they documented their journey for all who would come after them; to make it easier.  I probably watch too many movies, but I sorta felt like Indiana Jones stumbling upon a lost city when I realized I had access to hundreds upon hundreds of useful blogs.

Going through the content has made the Sinatra project seem less daunting.  The blogs have given me ideas of where I might stumble.  They've also shown me tips and tricks to get ahead.  They've also expanded my imagination of what is possible.  To all the students who've come before me: I feel like I'm standing on the shoulders of giants -- and the view is wonderful.  So, thank you.
# <center>**THE BLOGS**</center>

<center>**BUILDING THE BIG PICTURE (start here... it will make everything easier)**</center>

John Guest's "[How To Build a Sinatra Web App](https://jcguest.github.io/how_to_build_a_sinatra_web_app)"  is a great place to start. It gives you a bird's eye view of what you will be doing.  It doesn't mention the Corneal Gem which most of the other blogs DO mention.  But, because it covers the manual equivalent of what the Corneal Gem will do for you, it seemed a nice place to start; giving you a better understanding of what corneal does.

Richard Pascarelli's post "[Sinatra - Getting Started](https://rpascar1.github.io/sinatra_-_getting_started)"  is presented as a checklist and concise enough to serve as an outline for your own project.

Audrea Cook's "[ClassReads: My Sinatra Project](https://audthecodewitch.github.io/classreads_my_sinatra_project)"  gives you an example of how it all comes together.  Audrea also has a video demo which helps you see what is possible -- especially how CSS and HTML come into the picture.  There's a lot of CSS and HTML, and while it may seem intimidating, her post explains it well. 

Aurangzaib Danial Liaqat Khan's "[URL Shortener Made in Sinatra](https://aurangzaib-danial.github.io/url_shortener_made_in_sinatra)"  was eye opening on many levels.  Seeing someone build a URL Shortener prompted me to think bigger about what is possible for a student project.  His blog is also a retrospective and refactor.  His other blog "[Sinatra Portfolio Project](https://aurangzaib-danial.github.io/sinatra_portfolio_project)"  is a bit less of a checklist, but reading both provide a better portrait of an aspiring developer's journey.

Another combo of posts are by Alice Brunel. "[Sinatra Portfolio Project - Database Design](https://alicebrunel.github.io/sinatra_portfolio_project_-_database_design)"  and "[Sinatra project: Menus CMS and what I learned](https://alicebrunel.github.io/sinatra_project_menucms_and_what_i_learned)"  ... the first talks about designing the project.  She includes diagrams and additional helpful links.  The other blog addresses models, crud, erb, all in one place.  It's not only a great tutorial but a model blog post.

Assane Savadogo's "[Approach on the Sinatra Final project from Flatiron School](https://assansav.github.io/approach_on_the_sinatra_final_project_from_flatiron_school)"  breaks the process down into 10 major segments.  It could serve as the first blog post you read to prime your mental models, but on the other hand... getting to it after reading a bunch of other posts will give you an "AHA" moment (or at least it did for me).  I suspect the reason why it's more helpful to read this post later than at the beginning is because it's a concise organization, and having more information loaded into your mind (from the previous posts) gives you more to work with.

Kathleen Kamali's "[Sinatra CMS Project](https://kkamali.github.io/sinatra_cms_project)"  for an easy to understand example of creating the tables for migration.  In the context of Assane's post, this would probably serve as a more in depth explanation of Assane's "Third Step" which includes configuring the database.

Gio Zavaglia's "[Project #2: Let Sinatra Sing!](https://gzavaglia.github.io/project_2_let_sinatra_sing)"  goes over all of Flatiron's project requirements, once again reminding you of the greatest context your project must fulfill.  Gio's post explains Model View Controller, Separation of Concerns, Has Many, Belongs To, CRUD, and how it all fits in with Sinatra.


<center>**POSTS WITH SUPPORTING VISUALS **</center>

Elizabeth Parisi's "[Sinatra Project - Glam Guide App]( https://elizparisi.github.io/sinatra_project_-_glam_guide_app)" has SUPERB visual explanations of paths and routes, and a helpful table.  There is also useful advice and shoutouts to helpful instructors -- Elizabeth's attitude and mindset is one to emulate.

Alethia Quintero's "[Cuisine Cloud- Sinatra Portfolio Project](https://alethiaq.github.io/cuisine_cloud-_sinatra_portfolio_project)"  covers both planning and implementation.  The visuals are very helpful for every step covered in this post.

Tracy Reuther's "[Sinatra - In Relation to Bugs](https://treuther.github.io/sinatra_-_in_relation_to_bugs)"  has a great sketch by hand of how you might plan your project in addition to other planning tips and problems to look out for.


<center>**TIPS AND TRICKS**</center>

Edras Vallecillo's "[Sinatra - Gym](https://samirv16.github.io/sinatra_-_gym)"  was an interesting article and had a great tip on using CSS to render all error messages red.

Kari O'Neal wrote "[10 Helpful Tips for Creating a Sinatra App](https://coneal81.github.io/10_helpful_tips_for_creating_a_sinatra_app)" which was very digestible.

Diana Whalen's "[Sinatra. The framework, not the singer.](http://dianawhalen.github.io/sinatra_the_framework_not_the_singer)"  has a bunch of definitions in one place. A handy reference.

Kyle Luke's "[Plants & Things - Sinatra Portfolio Project](https://lukekyl.github.io/plants_and_things_-_sinatra_portfolio_project)"  is a good follow up to Gio's post in that it forewarns of some technical problems you may encounter.  It's not much of a checklist, more of a first person account, but the paragraph about "roadblocks" and how Kyle overcame them is very helpful.  Not just in terms of mindset, but of the kind of problems that sound common to many.

Huy Do's "[Sinatra Project](https://huyddo.github.io/sinatra_project)" covers some unique obstacles with links on how to solve them. Shotgun, Seed and more are touched upon.

Brittany Javalera's "[Sinatra Portfolio Project](https://brittjavs.github.io/sinatra_portfolio_project)"  has an example with excel that may help you wrap your mind around the project.

Carl Palumbo's "[Sinatra Porfolio Project](https://carlumbo.github.io/sinatra_porfolio_project)"  forms and paths has thorough examples of the code for creating forms.  If you've been going through the blog posts and were starting to wonder: "WHEN ARE WE GONNA GET TO FORMS?!" well, here they are.


<center>**MVCS**</center>

Anthony Prescott-Brooks's "[Sinatra MVCs](https://anthonbrooks.github.io/sinatra_mvcs)"  covers MVCs and REST, in depth, in context, and well integrated with concise code.

Kristin Kraemer's "[Planning Out My Sinatra Project](https://kristinhannah.github.io/planning_out_my_sinatra_project)"  gives an example of how she mapped about her models, views, and controllers.

Maasa Kono's "[MVC in Sinatra](https://maasa333.github.io/mvc_in_sinatrahas)"  some code, but shines as an analogy to understand MVC.  The code is very straightforward.

Warren Yao's "[Sinatra Project: Expense Tracker](https://wyao905.github.io/sinatra_project_expense_tracker)"  discusses models and migration tables.  Its discussion of models and migration tables -- more conceptual than code)

Chris Junker's "[Sinatra Final Project – Under the Hood](https://elevatemedfit.github.io/sinatra_final_project_under_the_hood)" helps you make sense out of everything with his discussion of middleware (the stuff that makes the magic work).

Aaron Parkening's "[Tea Tastes Sinatra App](https://aparkening.github.io/draft_post_on_tea_taster)" has an Old Model compared to a New Model.  It gives you a good idea of the before and after and how you might more quickly get to The After for your own project.


<center>**SECURITY**</center>

CPH Blogger's "[Another Project Down](https://chalpenny.github.io/another_project_down)"  has an interesting discussion on safe code and security authentication.

Mackenzie Moore's "[Secure Session Secrets for Sinatra](https://mackenzie-km.github.io/secure_session_secrets_for_sinatra)"  talks about generating a secret code.


<center>**EXAMPLES WITH CODE**</center>
<center>NOTE: Posts in the other sections also have code, but for the ones here the code really seems to shine.</center>

Tom White's "[Who's Damn Toy Is This: My Sinatra Portfolio Project.](https://tomciv9000.github.io/whos_damn_toy_is_this)"  along with Aurangzaib's is one of my favorite blog posts (of all the posts I'm writing about).  It has the requirements of the project, it has a drawing, it has code with logic, and object relationships explained... all with a sense of humor.  Also I have two small children so my empathy for this project was through the roof!

Cody Frank's "[Sinatra project mode Pokemon](https://codyfrank.github.io/sinatra_project_mode_pokemon)" provides detailed explanations of code and the relationships of the objects in your project.  In essence, Cody gets to The Why.  AND, with enough technical details to start "filling in the blanks" in the contextual frame/container you've created from reading the stuff above.

Stuart Hahn's "[Sinatra MVC Application](https://stuart-hahn.github.io/sinatra_mvc_application)" includes another overview of the project, from pre-code work to code.  Since the details are in the context of an overview, it makes it easier to absorb the info.

Karly Mareka's "[Bear Tracker: Building a Sinatra MVC Application](https://karlymareka.github.io/bear_tracker_building_a_sinatra_mvc_application)"  has code and the dev suite essentially side by side which help give you additional perspective into the final picture.

Lan Nguyen's "[Sinatra Project - Self Development](https://nguyenlan13.github.io/sinatra_project_-_shelf_development)"  gives an example of the MVC with code.  The focus is on a comments controller.

David Bermudez's "[Answerville with Sinatra and ActiveRecord](https://david-bermudez1102.github.io/answerville_with_sinatra_and_activerecord)"  along with a post he links to on Medium will give you an idea of how to build your own social network in Sinatra.  NOTE: the post on medium is more about rails, [it's here](https://medium.com/@esmerycornielle/making-a-followers-feature-with-ruby-on-rails-and-active-record-ddb3d1dda060).   David's is a very ambitious project.  There is no code in his blog, but he links to the GitHub repo which will help show you how he does the magic.  The styling of the images he's used to create his project is also very nice.

Sami Suliman's "[Sinatra Portfolio Project – Kanban Application](https://sami-suliman.github.io/sinatra_portfolio_project_kanban_application)"  has illustrative Has Many relationships.

Annalisa Graziano's "[To-Do Lister: My Sinatra Portfolio Project Blog](http://annalisagrazianoblog.com/to-do_lister_my_sinatra_portfolio_project_blog)"  code has reflections on the process, code, a video walkthrough and link to her project repo.

Juny McArdle's "[Sinatra Project Movieview](https://junymc.github.io/sinatra_project_movieview)"  is a project from scratch. It's not everything you'll need but covers most of the major points.

<center>**BONUS CONTENT ABOUT HEROKU BY AURANGZAIB**</center>

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/CKIWZNLQHx8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></center>

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/m_tRqz9wu_0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></center>
  
