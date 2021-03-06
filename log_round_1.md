# 100 Days Of Code - Log

### Day 100: October 17th, 2017 ###
(8:06 - 9:47pm, with a 10-minute break in between)

**Progress**:
* Worked on budget app today
  * Added pagination to transactions shown on individual budget's page
  * Added form for entering transactions
  
**Thoughts**:
Yay, day 100!  Felt like just another day working on my budget app, but I can definitely tell I've been learning - even though I've got so much more to learn!  I want to be much faster than I am today at working on Rails apps and coding in general, but I'm still proud of myself.

Today I learned that I do indeed need more than 30 records in my table for the will\_paginates gem to work, and I learned that I need to understand a bit better about how form labels work (rather than just switching things out based on skimming the documentation and seeing something that looked like what I wanted to do).  Right now, I need to figure out why the records in the form don't want to save properly - I have a suspicion that it has to do with the format that the date field wants.  

There are also so many more features to add!  I feel like I could write out a feature map for v1, v2, and maybe even v3 right now for all the fancy stuff I want to do :)

I want to write a longer analysis of some things I've learned during my 100 days and look back through my log, but for now I need to go do some dishes!!

**Link to work**:
Here's today's commit: 
* https://github.com/twoesplease/budget-app/commit/5bc034cbc1be116c471edb76a134d2477cc486b3

### Day 99: October 16th, 2017 ###
(7:28 - 8:28pm)

**Progress**:
* Worked on an original project today, my budget app
  * Added linked budget names to individual user profile pages
  * Added transactions to each individual budget's page
  
**Thoughts**:
Didn't make as much progress as I would have hoped today, but I can feel myself getting faster.  I tried to paginate the transactions on the individual budget page will the will\_paginate gem like I learned yesterday in the [Hartl Rails tutorial](https://www.railstutorial.org/book/basic_login), but I think I need more than 30 transactions in order to do that.  I also need to get into better habits of writing tests!

On my lunch break today I also made it through 10 exercises/chapters in [Learn Ruby the Hard Way](https://learnrubythehardway.org/) as I have a goal to read back through that one this week.

**Link to work**:
Here's today's commit:
* https://github.com/twoesplease/budget-app/commit/2533966848ba9476add238ff55d52ad44ff8d4e8

### Day 98: October 15th, 2017 ###
(8:55 - 10:19pm)

**Progress**:
* Continued Chapter 10 of [Hartl Rails tutorial](https://www.railstutorial.org/book/basic_login) book
  * Added index page to display all users
  * Installed Faker gem to add some sample users to app
  * Added pagination to app via will\_paginate & bootstrap-will\_paginate gems
  * Added test that pagination works
  
**Thoughts**:
Luckily, today felt much less like I was slogging through the content and begging my brain to absorb what I was reading - even though I worked outside all day and was pretty tired.  All the content still felt really applicable to building web apps everyday too.  The one thing that held me up was some indentation that was ever-so-slightly off in my test fixtures yaml file, which seemed to break EVERY one of my tests multiple ways!  Definitely a good thing to know for the future.

I'll probalby move on from the Hartl book for a little while starting tomorrow, even though I'm really eager to finish.  The reason is because I put together an 8-week learning plan to prepare for an Engineering apprenticeship just in case they post it at the beginning of November, and finishing the Hartl book was what I had lined up for last week.  I'll still plan to work on it if I get spare time and do think it'll be really good for me to finish it, I just didn't realize that each remaining chapter would take me 3+ hours to complete.  The last 2 weeks I also left open for review, so I may be able to fit in some more Hartl content then.

Also, I got a cable I need to connect my Raspberry Pi to a monitor at work, so tomorrow I hope to get the Pi on the internet at work to see if I can get the Pegacorn scripts working there.  Fingers crossed!

**Link to work**:
Here's today's commit:
* https://github.com/twoesplease/sample_app_hartl/commit/ad04a1e14d03a316db227f11b07e7c66365439dd


### Day 97: October 14th, 2017 ###
(9:05 - 10:20pm)

**Progress**:
* Continued Chapter 10 of [Hartl Rails tutorial](https://www.railstutorial.org/book/basic_login) book
  * Added code so that users can only edit their own profiles
  * Added friendly forwarding so that when users who aren't logged in try to complete an action, the page they were trying to reach is saved and they're redirected back to it once they're logged in
  * Added tests for the above functionality
  
**Thoughts**:
It doesn't look like I made much progress today, but a typo hindered my progress for a while and caused my tests to fail, so I was hunting it down for about 25 minutes (facepalm).  I also read back through the code a couple of times and through the description of the steps in the book once more, because I didn't feel confident that I'd completely gotten it the first time around.  

I've started taking less detailed notes so that I can progress a bit faster through the book, so I'm just tyring to summarize things and add details if there's really a detail I feel it's pertinent to remember.  That means I really have to get the concepts for things solidified in my mind so I can write them down which is good, but today my brain felt like it didn't want to wrap all the way around what it was doing quite as fast as I hoped.  I'd still rather understand properly than finish faster.  I think the more code you add the more there is to keep in tyour mind because the code references other code all over the place!  And this is such a small codebase, I'm sure that problem gets exponentially bigger with large codebases.  Some of this will become second nature to me as I use it more though, so it won't feel quite so much like another thing I have to hold in my head.

I know that I usually want to be writing original code instead of following a tutorial on my #100DaysofCode time, but I'm trying to make it through as much of this book this week as I can.

**Link to work**:
Here's today's commit: 
* https://github.com/twoesplease/sample_app_hartl/commit/34158f76e8e4c8df5061a44f690009648642982a

### Day 96: October 13th, 2017 ###
(9:57 -11pm)

**Progress**
* Worked on Chapter 10 of [Hartl Rails tutorial](https://www.railstutorial.org/book/basic_login) book
  * Added before filter to Users Controller requiring that users be logged in to access edit & update actions
  * Defined a logged\_in user action so that the before filter would work & that would redirect folks who weren't logged in
  * Wrote test to test that the before filter worked
  
**Thoughts**
Sad that it doesn't look like I'm going to finish the Hartl book this week like I was hoping, but I'd rather learn well than speed through this.  All of what I'm learning is definitely highly applicable to writing web apps irl.  There are gems for a lot of this logging in and authorization behavior but it's nice to know how to do it myself, and I'm learning a lot of other important concepts on the way.

**Link to work**
Didn't do a commit today.

### October 12th, 2017 ###
* Worked some in Hartl on my lunch break but I'm not going to count it because I didn't make it to an hour and I generally don't like to count my lunch break time as part of my hour.

I sat down to do my hour of code tonight but my partner's sister was over and I wasn't able to focus to get it done.

### Day 95: October 11th, 2017 ###
(7 - 9:57pm)

**Progress**:
* Completed Chapter 9; Advanced Login in [Hartl Rails tutorial](https://www.railstutorial.org/book/basic_login) book
 * Added 'remember me' functionality to sample app's login form
 * Learned how to generate remember token and corresponding remember digest to store session information in a cookie safely (doesn't store remember token in the user database)
 * Learned that deleting a session and cookie are the way to log a user out
 * Added tests AND a test of a test to make sure this functionality is working properly
 
**Thoughts**:
I set a goal for myself to finish this book this week, but taking 3 hours to finish this one chapter on a Wednesday makes it seem very unlikely, even with me taking more succinct notes.  I don't want to blast through it and not retain anything either, so I may have to adjust that plan or choose another time to finish the book if I want to continue on schedule for the other items I've got on my learning schedule for the next 5 weeks.

As always, there was lots of good info in this chapter (including a sidebar about ternaries which I probably won't use but want to be able to read). Please stick in my brain, info!!

**Link to work**:
(Note that I worked some outside of my code time this evening too and finished chapter 8, so there's a commit for that too):
* https://github.com/twoesplease/sample_app_hartl/commit/c26a90cba9fa040daf70720c72a15f038a49dbd0
* https://github.com/twoesplease/sample_app_hartl/commit/a6ef9ecec80449addc15845413d43db694902d95
 

### Day 94: October 10th, 2017 ###
(7:40 - 8pm, 9:52 - 10:30pm)

**Progress**:
* Continued through Chapter 8 in [Hartl Rails tutorial](https://www.railstutorial.org/book/basic_login)
  * Updated header links conditionally based on whether user is logged in
  * Wrote test to confirm that these updates to the header links update upon login
  
**Thoughts**:
I'm trying to finish this book this week, as I've updated my learning plan and have new tasks written down for next week - otherwise I wouldn't be spending my coding time on tutorials.  Even though this one is a wonderful learning resource, I generally prefer the idea of spending my lunch break on reading and tutorials and evenings on writing original code.  But, everything I read is chock full of good info as usual.

I paused in the middle of my coding time to have a Slack chat for RubyCOnf Opportunity Scholars this evening, which is exciting!!  I got to hear from some organizers and other scholars and got to ask a question.  I really want to push myself out of my major introvert comfort zone at RubyConf since it's such a fantastic opportunity I'm getting.

**Link to work**:
The book didn't direct me to make a commit yet, but I'm thinking I should start doing that at the end of my coding sessions anyway.

### Day 93: October 9th, 2017 ###
(9:25 - 10:25pm)

**Progress**: 
* Skimmed through a bit of the Odin project to check out the content and compare my own progress to it
* Worked through parts of Chapter 8 in [Hartl Rails tutorial](https://www.railstutorial.org/book/basic_login#sec-logging_in) on logging users in

**Thoughts**: 
I always feel like I learn a ton every time I work through a bit of the Hartl tutorial.

I took my Raspberry Pi to work today and hoped to get it set up to light up when the scripts triggered, but I couldn't get the right display dongle so I had to order one.

**Link to work**: 
No commits today!

### Day 92: October 8th, 2017 ###
(2+ hours in the early afternoon)

**Progress**: 
* Got to a minimum viable product with my 3 Pegacorn Project scripts!
  * Figured out how to retry the watch_chat_waits script a couple of times if it wasn't successful the first time
  * Fied a bug in count_good_ratings file caused by a change to the Zendesk API where it wasn't gettisng the count of the good ratings any longer
  * Moved scripts over to storage on Raspberry Pi and updated file referencing my auth credentials to the right path
  * Updated Ruby on Raspberry Pi to latest version instead of the much older version it was one
  * Installed Vim on Rapsberry Pi and set some defaults like theme + turning on line numbers & syntax highlighting
  
  **Thoughts**: 
 I didn't have any experience with retrying code blocks previously so it took me several tries to get logic right and learn some rules about when redo/retry can and cannot be used.I ended up having to write out the flow I wanted on paper to think through how I wanted my code to work, and that was helpful. 
 
I also used Pry for the first time today (instead of byebug/debugger) to help me figure out why the count_good_ratings script wasn't working any longer and it was super helpful!  I know this is a tool that I'll make lots of use of in the future, so I'm glad to be learning a bit about it.  Some other things that I tried when debugging this that I think will come in handy in the future were the `git diff` command and checking out earlier commits to see if the script worked in those (which would let me know if a recent change to the file broke things).
 
My code definitely needs some refactoring, since I think some pieces of the code can be broken out into their own units and I know there are some errorss from Rubocop that I should fix.  That said, I'm glad to have finished these three scripts and to get things set up at work tomorrow to get them working!

**Link to work**:
Here are today's commits:
* https://github.com/twoesplease/pegacorn_project/commit/b95503cebddd65f06f8a8d5b22f160163c252b91
* https://github.com/twoesplease/pegacorn_project/commit/12cb302ba0c7d6aff96540c111a42f8d0226a550

### Day 91: October 7th, 2017 ###
(8:24 - 9:29pm)

**Progress**:
* Used [this article](http://blog.mirthlab.com/2012/05/25/cleanly-retrying-blocks-of-code-after-an-exception-in-ruby/) to learn how to retry the wait time check a couple of times if it doesn't run successfully the first time.

**Thoughts**: 
I found that using rescue/retry only worked properly in my script when used in a method definition, but not when used in a code block.  The logic isn't perfect yet, but I feel fairly confident that I know what I need to do in order to get it working - which is a nice feeling!

**Link to work**:
Here's today's commit:
* https://github.com/twoesplease/pegacorn_project/commit/d6c1b72a75d73c91a56d9c934e979313c623e3df

### Day 90: October 6th, 2017 ###
(9:15 - 10:18pm)

**Progress**: 
* Figured out how to access chat wait time buried inside an array, inside a hash, inside a hash, inside another hash, inside a JSON object for Pegacorn Project
* Added basic triggers on chat wait time in preparation for lighting the pegacorn based on chat wait time
* Did a bit of googling on handling errors and retrying a couple of times before giving up

**Thoughts**:
My code's not beautiful, but I made some good progress on the Pegacorn Project today I think.  I can also clearly see (or so I think) the next steps that I need to take in this file to get things working.  This project has really been a lesson in patience, asking for help, dealing with third-party software, and all kinds of other mini-lessons.  I'm glad that my next step will be error handling, because I feel like that's a skill that I could definitely stand to build.  While Rubocop errors are a bit annoying a lot of the time, it gives me good and helpful suggestions & my code is better overall for using it.

I feel a bit bad that I didn't end up writing any tests today, but I was excited about making some progress on this project in this particular file.  And there are definitely some tests I can write to make my code better.

As a side note, I got asked for help for someone who was trying to work with the Zendesk API today!  I was a little nervous (because social anxiety) and didn't explain things was well as I'd hoped, but the person I helped got what he needed and I got some tips on how I can improve next time.

And one more thing, when I tried making an edit in this log just now I totally tried to use vim editing commands #vimlyfe.

**Link to work**:
Here are today's commits:
* https://github.com/twoesplease/pegacorn_project/commit/d5946a8677b173b6f856ab8b1938275f4a5aaeea
* https://github.com/twoesplease/pegacorn_project/commit/185cbdafd68da2c3a25c58c01e87081d31e285f0


### Day 89: October 5th, 2017 ###
(7:54 - 8:54pm)

**Progress**:
* Finished the [article on Minitest](https://semaphoreci.com/community/tutorials/getting-started-with-minitest) that I've been working through
* Worked through [another article from that same site](https://semaphoreci.com/community/tutorials/mocking-in-ruby-with-minitest) on mocking and stubbing in Rails applications
* Read another [short article on Minitest](https://mattbrictson.com/minitest-and-rails) that I had in an open tab

**Thoughts**:
I feel a bit guilty for working through tutorials, so tomorrow I'll have to push myself to use this stuff!  That said, I'm excited to have read something about mocking and stubbing because I've been curious about those terms for a while now.  I don't have the differences between them all the way down yet, but I've saved the article I read and now have a framework so that I can build my knowledge up more with other soruces.

**Link to work**:
Didn't push anything today.

### Day 88: October 4th, 2017 ###
(8:50 - 9:53pm)

**Progress**:
* Continued working through the [article on Minitest](https://semaphoreci.com/community/tutorials/getting-started-with-minitest) that I started yesterday
* Worked a bit on the watch_chat_waits portion of the Pegacorn Project

**Thoughts**:
I wrote to Zendesk support yesterday to ask for sample code that I could compare to the code I'd written for the real-time chat API and they told me that when I request to subscribe to a metric, I needed to do it using JSON.  When I updated my code to do that and followed their example of putting my subscription arguments in a hash, the code worked!  For the last few minutes of today, I worked on trying to pretty format my output but my first attempt at using the built in PrettyPrint didn't work.  I'll have to work on that tomorrow so that I can tell my light to turn on when the conditions are right!

I need to start practicing TDD/BDD and using the minitest knowledge I'm gaining so I don't forget it.

Side note: I found out who my guide for RubyConf is and wrote my first email to her today! 🎉

**Link to work**:
Here's today's commit: 
* https://github.com/twoesplease/pegacorn_project/commit/7fd4e45b3863c74d6863c725fc896450cdbc2ad8

### Day 87: October 3rd, 2017 ###
(10:15 - 11:20pm)

**Progress**:
* Started working through an [article on Minitest](https://semaphoreci.com/community/tutorials/getting-started-with-minitest) that you can code along with
  * Read a couple of other articles on the way
* Fixed an issue that moved over from old machine to new with me regarding Minitest

**Thoughts**:
Today involved a lot of getting off track!  I started with one article on minitest that I was going to quickly read and then switch over to exercises.  That article reommended I read another introduction to minitest article, which then recommended that I needed to read an article about Behavior-Driven Development first.  I made it through that one and partway through the introduction to minitest.

In the process of testing I also raninto an issue where the dot, F, or S was displaying twice with minitest output and figured out that it was the minitest-reporter gem.  Uninstalling that fixed thigns up!

Finally, I thought I would run a quick brew update && brew upgrade while I was reading but I got an error and went on a goose chase of reading articles and finally updating xcode + opening it + installing additional packages to get that brew updae && brew upgrade to work.

**Link to work**:
Nothing to link to today.

### Day 86: October 2nd, 2017 ###

### Day 85: October 1st, 2017 ###

### Day 84: September 30th, 2017 ###

### Day 83: Septebmer 29th, 2017 ###

### Day 82: September 28th, 2017 ###
(9 - 10pm)

**Progress**: 
* Finished functionality for blog app! 
  * Implemented user sign-in with Devise and 
  * Note that I'm following along with a [video by Mackenzie Child](https://www.youtube.com/watch?v=BI_VnnOLSKY&list=PL23ZvcdS3XPLNdRYB_QyomQsShx59tpc-&index=2)
* Fiddled a bit with subscribing to a metric in Zendesk's Real-Time chat API with the [faye-websocket](https://github.com/faye/faye-websocket-ruby) gem but no luck

**Thoughts**:
Glad to have finished functionality on the blog and that I've been able to lean a thing or two and get some practice in a guided way.  I want to make some updates and change the styling to make it my own, so I watched a couple of minutes of a Bootstrap tutorial.  But then, I decided that I'd rather focus on Ruby & Rails for now since being a front-end developer isn't my goal.  So I switched over to working on the Pegacorn Project for the rest of my hour.

If I do a second round of 100 Days of Code though, I'd like to use the blog on my site just so I could use something that I put the pieces together for myself.

**Link to work**: 
Here's today's commit: 
* https://github.com/twoesplease/personal_site_blog/commit/9c88b28b7e7372c8b5297dcc14e7e28b259b0195

### Day 81: September 27th, 2017 ###
(10:06 - 11:22pm)

**Progress**:
* Fixed comment functionality 
* Added about page
* Added a Bootstrap icon for the home page
  * Note that I'm following along with a [video by Mackenzie Child](https://www.youtube.com/watch?v=BI_VnnOLSKY&list=PL23ZvcdS3XPLNdRYB_QyomQsShx59tpc-&index=2)

**Thoughts**: 
In my exhaustion last night I put some totally incorrect code in my comment partial.  It caused my server to continually try to load something it couldn't get to (so I just SQL lookup lines being entered repeatedly in my server log) and the page wouldn't load.  I had to close the tab to stop the server log from going on forever (ctrl+c & ctrl+d didn't work) and then go in and kill the server job twice before I went in and fixed the code in the comment partial.  Silly sleep-brain!

I also copied the content off my current ~ * vanity site * ~ home page and stuck it in my about page.  The styling isn't gorgeous but I'm focused on functionality & learning, people!  I don't have aspirations to be a front-end.

I also used a bootstrap icon for the first time so that I could have an easy link back to the home page from the sidebar.

**Link to work**: 
* https://github.com/twoesplease/personal_site_blog/commit/9a1696d298f11a8da87a3f190be1c6d8030555a6
* https://github.com/twoesplease/personal_site_blog/commit/fa5279377cd0ed3dbffd336ccfa043b42714fe3e
* https://github.com/twoesplease/personal_site_blog/commit/b93de0946c684b630f321a54d6bb5116f60fd6ee
* https://github.com/twoesplease/personal_site_blog/commit/c5fb5696111a4ade7261de42dacbbb87929fc790
* https://github.com/twoesplease/personal_site_blog/commit/0d2126fb8d7818cb1183210a34d4f9dcc5b353b2

### Day 80: September 26th, 2017 ###
(10:30 - 11:30pm)

**Progress**: 
* Added ability to edit and delete blog posts
* Started on commenting functionality
  * Note that I'm following along with a [video by Mackenzie Child](https://www.youtube.com/watch?v=BI_VnnOLSKY&list=PL23ZvcdS3XPLNdRYB_QyomQsShx59tpc-&index=2)

**Thoughts**:
Was so exhausted and fighting sleep today.  Not my best work but hopefully some of it sinks in.

**Link to work**: 
Here are today's commits:
* https://github.com/twoesplease/personal_site_blog/commit/ee6e7927d49c8c8db58396fdd22ac44ffda3e95c
* https://github.com/twoesplease/personal_site_blog/commit/f621bc00022fac54707c5f4df0fad6d658df3a47

### Day 79: September 25th, 2017 ###
(10:21 - 11:34pm)

**Progress**:
* Fixed the issues from yesterday in my blog app
  * Strong params weren't working on the new post form because of an error in my posts controller - I had some code in the 'new' method that was trying to save the form, but that was a job for the 'create' method instead
  * The linter error I was getting for the posts form seems to be an issue of the linter being outdated.  I saw that in older versions of Rails, it wasn't necessary to put the '=' in the erb tag on the 'form\_for' line.  The linter error went away when I removed the '=' on my form, but also the whole form didn't display.  Once I fixed the controller issue, the form submitted and saved new entries ok without fixing the linter error.
  * The new post button on my homepage wasn't working, but I found out that it was due to the styling that was applied to it. I'm not quite sure why yet, but for now I have an unstyled (read: ugly) but working new post button.
  * Note that I'm following along with a [video by Mackenzie Child](https://www.youtube.com/watch?v=BI_VnnOLSKY&list=PL23ZvcdS3XPLNdRYB_QyomQsShx59tpc-&index=2)
  
  **Thoughts**:
  I was worried I wasn't going to make much progress on this today, but since I'm coding along with a [video](https://www.youtube.com/watch?v=BI_VnnOLSKY&list=PL23ZvcdS3XPLNdRYB_QyomQsShx59tpc-&index=2) I was able to reference the code by the original creator and see the issue with my controller.  The other two things I was able to figure out via trial and error.
  
Other exciting news for today is that I found out I'll get to attend RubyConf 2017 as an Opportunity Scholar!!  I'm so excited.  Yaaaay :D

**Link to work**:
Here are today's commits:
* https://github.com/twoesplease/personal_site_blog/commit/7c6915c156125caa10cf0a72b983c610abd7644d
* https://github.com/twoesplease/personal_site_blog/commit/4ded8e61403171ae1791e1534c7a9e4a88d66e8d


### Day 78: September 24th, 2017 ###
(8 - 10:33pm)

**Progress**:
* Did more work on basic blog app
  * Got some weird errors when creating new blog post & did troubleshooting on that for a while
   * Note that I'm following along with a [video by Mackenzie Child](https://www.youtube.com/watch?v=BI_VnnOLSKY&list=PL23ZvcdS3XPLNdRYB_QyomQsShx59tpc-&index=2)
  
  
**Thoughts**:
Got stuck on my new "easy" project.  I know I'll figure this one out and will have learned something on the other side of it, but it's still frustrating to have been stuck on something that feels like it should be easy.  Something changed in the process of creating and saving a new blog post today, and based on the error I was getting in my browser about the strong params I was using, it seemed like it may be in the form for creating a blog post.  I was getting a weird linter error in there about an unexpected ')' as well even though I wasn't using any '(' or ')', so it seemed like that was likley.  I did several tweaks, figuring that it may be due to a syntax mismatch between the Rails 4 the video I'm following along with is using vs. Rails 5 which is the version of Rails I'm using for this project but I haven't been able to narrow it down yet from referencing the docs and a few Stack Overflow responses.   I also did some peeking in my router, Posts Controller, and Posts Model but couldn't find the issue yet.

Tomorrow to keep troubleshooting I can roll back to a previous commit where this was working and track down what's changed.

**Link to work**: 
Here are today's commits:
* https://github.com/twoesplease/personal_site_blog/commit/2668c614b09d13450425f84aaaca4d594553f4f3
* https://github.com/twoesplease/personal_site_blog/commit/479850348f6e99e72c267ce14bc405a17afb3a04

### Day 77: September 23rd, 2017 ###
(9:26 - 10:40pm)

**Progress**:
* Updated cdoe connecting to Zendesk's Real-Time Chat API to stop returning a 500 error
* Started coding along with [a YouTube video by Mackenzie Child](https://www.youtube.com/watch?v=BI_VnnOLSKY&list=PL23ZvcdS3XPLNdRYB_QyomQsShx59tpc-&index=2) that goes through the process of creating a basic blog app

**Thoughts**: 
It's hard to tell if the code connecting to the Real-Time Chat API is working properly, because it's supposed to get data for chats and chats aren't turned on right now.  I set it to watch for a 30-minute period and it didn't automatically close after 30 minutes or give me any type of response other than a successful connection message, but I'm not sure if that's the expected behavior.  I can check again on Monday when chats are back on.

I also decided to give my brain a little bit of a Rails break and follow along with a fairly simple video so that I could build a simple app where the code was very likely to work (since it's already worked for the person creating the video.  I figuredc it'd be good practice but would be nice to have a mini-project where I wasn't having to do a ton of intense troubleshooting.

Sidenote: Glad that I'm getting into better habits with more frequent commits :)

**Link to work**:
Here are today's commits: 
* https://github.com/twoesplease/personal_site_blog/commit/eb09ef4c18fd792952bc9ad9ff8c2602b8039c72
* https://github.com/twoesplease/personal_site_blog/commit/8b7543c3c1eed3eaed0e22ca5456c6bfb73c182e
* https://github.com/twoesplease/personal_site_blog/commit/5c253b17ea72f17fc4c8248611f2fc3394f5a776
* https://github.com/twoesplease/pegacorn_project/commit/f8686b8b7b5b9c89f605a6b9422f5e787cef5559

### Day 76: September 22nd, 2017 ###
(9:18 - 10:38pm)

**Progress**:
* Successfully authenticated to Zendesk real-time chat API using faye-websockets gem instead of the original gem I had been using, but got 500 error

**Thoughts**:
So glad to finally be unstuck on both of my projects!  This one took quite a lot of tweaks, and I still have some progress to make but it's nice not to just be stuck on the same step I started at.

Not sure if the error I'm getting is because I'm not subscribing to a metric yet in the script (I wanted to focus on successfully connecting first), or because there's an issue with the Zendesk Real-Time Chat API.  I'll figure that out the next time I work on this project.

**Link to work**:
Here are today's commits:
* https://github.com/twoesplease/pegacorn_project/commit/f8686b8b7b5b9c89f605a6b9422f5e787cef5559
* https://github.com/twoesplease/pegacorn_project/commit/14eb645f6fb2fc7c9c8bed1f5715130bbce4fc6e

### Day 75: September 21st, 2017 ###
(5 - 6:30, 9:30 -10pm)

**Progress**:
* Used debugger with *.errors.full_messages* to fix the issue that was preventing the .valid? test from passing for my Budget model
* Continued work on Budget model tests
* Tried to fix an annoying linter highlight issue in my Vim setup
* Attended "Project Night" to discuss & work on projects with other folks at work

**Thoughts**:
Definitely did some learning today!  I got a recommendation from someone in a Slack channel to use *.errors.full_messages* to figure out why my test was failing, and I used debugger/byebug to freeze my Budget model test at the right spot to use that chained method.  It told me something about not having a properly-associated User object, and then I figured out that I needed to add one to my setup method.  That taught me a lot about the scope for tests and the setup method that informed the further work I did with my tests.  It feels good to be un-stuck on this project.

Another note: I keep getting issues with swapfiles (.swp extension) in Vim lately, and they're also creating errors with my merges back into master.  I wonder if I keep forgetting to save files before closing them?

I also spent a lot of time today tweaking Vim settings because the linter I use highlights issues it finds in a color that makes text in Vim difficult to see. I tried lots of different settings tweaks and color scheme changes, but none of them really worked well so I'm back to where I started.  Oh well, that can be a fight for another day.

**Link to work**:
Here are today's commits:
* https://github.com/twoesplease/budget-app/commit/1ee15928b65e3fdd8a2c71d3677019cc68a7a8ab
* https://github.com/twoesplease/budget-app/commit/16c3cb63d891174f4b4449e20fb38288d6432482

### Day 74: September 20th, 2017 ###
(9:17 - 10:40pm)

**Progress**: 
* Attempted to fix test failure (for the basic .*valid?* test) for budget model
  * Removed and recreated budget model 
  * Recreated associations between User, Budget, & Transactions models & generated corresponding migrations
  * Created objects in consoleto make sure that there were transactions that belonged to a budget and budgets that belonged to a user

**Thoughts**: 
I think I can call today's work a yak-shaving experience.  Last time I worked on this, I decided that my budget model was borked and that I needed to redo it to fix the associations between the budget model and the users model.  This was all in an attempt to get the basic validity model test for budgets to pass.  I recreated the budgets model today and found that I probably hadn't generated my migrations properly the first go-round to appropriately link the budgets and users models.  
TMYK: The associations for belongs_to and has_many are only added to the db schema file if you specify them when creating your models.  After all that work though, my budget model test still fails and it's still because of the line that specifies that a budget *belongs_to* a user.

I tested further today by making sure there were objects in the database that represnted all those associations, but that didn't make a change.  I also decided to test whether budget items that I created via the console returned true for the *.valid?* test -- and they did!  That could mean that there's an issue with the budget object I created in the test file's setup method -- but even specifying a user_id there didn't help.  I ended the night by asking for help in the Rails channel fo the CodeNewbies Slack team.  Hopefully I'll get some help there! 

I did remember to make lots of smaller commits today so that I'd have smaller bits of work to roll back to in the vent that I needed to.  That may very well come in handy, as I had a false start on my work at the beginning of today's hour that I rolled back.  Getting some good practice with those git skills.

**Link to work**:
Here are today's commits:
* https://github.com/twoesplease/budget-app/commit/e6455508710aea2bb91e1666116c250f1b498495
* https://github.com/twoesplease/budget-app/commit/1ba7d5db0d3b23608a439583656a57b5e095ff92
* https://github.com/twoesplease/budget-app/commit/136a32373aabbc6bd25f419681786b6b785c40ed
* https://github.com/twoesplease/budget-app/commit/2a038dbc2b660f75af11da3793316754d6f9deb8
* https://github.com/twoesplease/budget-app/commit/4eccf0f4817f05b2c67b65ce1e57bdde9d53e654
* https://github.com/twoesplease/budget-app/commit/e1ff0db5394f2ecf0911a81d81845d3dc785f993

### Day 73: September 19th, 2017 ###
(7:50 - 8:18pm, 9:22 - 10:19pm)

**Progress**:
* Switched up some syntax to try to make websockets connection to Zendesk Real-Time Chat API
* Tried [faye-websockets gem](https://github.com/faye/faye-websocket-ruby) to try to make websockets connection to Zendesk Real-Time Chat API also

**Thoughts**:
I asked for help on this in Slack yesterday, and got an answer today that suggested I try a different gem.  That one didn't look like it would work, but I did decide to give the Faye-Websockets gem a try in this case.  No luck :(

I also tried some more tweaks to the syntax in my original code, but didn't get any new results there either.

It's frustrating to be stuck on the two main projects I'm working on.  Perhaps my next steps for this one will be to make a checklist of things to try, and if I get really desperate to reach out to Zendesk's help team again (though I dread it).

**Link to work**: 
Here's today's commit:
* https://github.com/twoesplease/pegacorn_project/commit/5efe1a59b7580dd36f2f81a018e2971ce46bcbfe

### Day 72: September 18th, 2017 ###
(10 - 11:20pm)

**Progress**:
* Found possible source of failing Budget model validity test - Budget model doesn't have an ID column
  * Tried to fix association between User & Budgets models, but no luck

**Thoughts**:
Since I found out the last time I was testing this that the validations fail when adding belongs_to :user to my budget model, I figured that not having a unique ID identifier for budgets could be causing the issue.  However, when I attempted to add a new migration to create this column, I got an error that the ID column was a duplicate.  The weird thing was, the id column didn't appear in the db schema and I couldn't find other migrations that were adding it.

I even rolled back my database to version 0 and then attempted to migrate again, but I still got the error about the duplicate column.

Then, I decided to delete the 2 migrations relating to the budget model that were in addition to the migrate that created it.  I didn't get any feedback when I rain rails db:migrate and didn't see a budget ID column in the db schema.  Finally, I created migrations to delete any column mentioning budgets from any non-budget table, but that didn't work either.

Not sure what's going on, and I'm tempted to start over with my models & migrations.

**Link to work**: 
Here are today's commits: 
* https://github.com/twoesplease/budget-app/commit/23779f4b6c544502681143b9d32d56fd9c7b9e50
* https://github.com/twoesplease/budget-app/commit/4c50aaaf381db9fae86e3636a9f48ed32e770755 (hmm, why did this create a separate commit?)

### Day 71: September 17th, 2017 ###
(10:23 - 11:24pm)

**Progress**:
* Did some work on the Pegacorn Project to try to get my watch\_chat\_waits script to play nice with the Zendesk real-time chat API

**Thoughts**:
Not much luck today, unfortunately.  I couldn't find the sample JS code that Ionce had as a reference script for working with the real-time chat API, and mine was still returning zilcho.  After trying a couple of changes, I decided to double check that my Oauth creds were still working,but gotan error when attempting to make a cURL request to the REST chat API. This led me downa rabbitholeof regenerating my credentials, with several twists/turns/errors along the way - afew of them relatedto losing some of my history due to having a new machine.  

I finally got them regenerated and was able to make a successful cURL request to the REST chat API, but I think my original problem with that may have been a spacing/format issue - cURL seems so finicky!  Still no luck making a successsful connection to the real-time chat API via my script though.  Next I need to find that sample JS code from Zendesk to reference.  Some helpful error messaging sure would be nice too.

**Link to work**:
Here's today's commit:
* https://github.com/twoesplease/pegacorn_project/commit/dc31f07abd24e93bbf81ce8497de32429e284bcd

### Day 70: September 16th, 2017 ###
(10:20 - 11:20pm)

**Progress**:
* Continued trudging along with validations & tests for budget model, to try to get the .valid? method to work in a test
  * Narrowed down the validations one by one to see which ones caused that .valid? tests to fail, and did the most work on the validation belongs\_to :user since it was the first one creating an issue
  
  **Thoughts**: 
  Though I thought that my budget model's basic validation test was failing even with no validations previously, it seems  that today I was able to narrow the cause of that failure down to 2 separate validations when running the test a with a single validation at a time.

The first validation that caused it to fail was the belongs\_to :user validation, wo I did some work trying to update the relationship between the two so that it would be correct.  I didn't get it working, but I got super tired so decided to switch over to watching a video for my last 10 minutes or so.  This is a video that I've been watching in chunks for several days now, of someone building a Rails move ratings app.  I'll pay attention to how they link the users and review models to get them to play nicely together - should be helpful even though I haven't seen them run tests yet.

Things I can look into after watching the video - set a before\_action on budgets controller to :set\_user, & add to the budgets controller that the user\_id is the current_user.id of the user creating that budget

Side note, I keep forgetting to change over to my development-branch in git whenever I first start working, which leads to merge conflicts when it's time to merge my topic branch.  Today, I just switched back to my development branch after I made my commit so that I'll be in the right place when I get started tomorrow.

**Link to work**:
Here are today's commits:
* https://github.com/twoesplease/budget-app/commit/a071f3ad02444b999f0c9e7b2e053898f20af48c
* https://github.com/twoesplease/budget-app/commit/3b3d4d79401adcc81b1b7d10e43804cacfc0c64c

### Day 69: September 15th, 2017 ###
(9:45 - 11:45pm)

**Progress**:
* Continued work on validations & tests for Budget model
  * Did much googling about the best way to validate dates
  * Found a gem called [date\_validator](https://rubygems.org/gems/date_validator) designed to help validate dates
  * Updated tests to test valid dates
* Worked through issue that broke tests and caused them to return error messages instead of running: https://cl.ly/3o1V181N352o

**Thoughts**:
Working through today's tests issue was not fun, because after all that googling and implementing that gem I wasn't able to then test it out.

I spent an hour figuring out why my tests suddenly weren't working, and figured out that it was because I'd run `brew update && brew upgrade` earlier today just as a habit.  That updated Ruby.  After much googling without much success, plus messing with homebrew & rbenv for an hour, I just copied a file and renamed it to the name that Ruby was looking for and that fixed the test.

It passed, but my tests that are passingare asserting that @budget isn't valid, and I still haven't been able to get @budget.valid? to return true -- so they're not accurate ruight now.  Tomorrow I'll have to do more digging into why my basic validity check isn't working - I feel like it's something elementary.  Maybe I'll dig into using debugging tools - I tried 'debugger' earlier today with a few spare minutes but didn't get very far.

**Link to work**:
Here are today's commits:
* https://github.com/twoesplease/budget-app/commit/8332a2e27e9060c7b9cfd3f89baa3fcca24771ad 
* https://github.com/twoesplease/budget-app/commit/06ac0542c3eaa479f45fff81e0291ec879d91bf3

### Day 68: September 14th, 2017 ###
(8:48 - 10pm)

**Progress**:
* Continued work on validations & tests for Budget model
* Started using a few new shortcuts for vim: 
  * One to remove comments with [NERDCommenter](https://github.com/scrooloose/nerdcommenter)
  * One to open a file tree in a separate buffer with [NERDTree](https://github.com/scrooloose/nerdtree)
  * One to replace surrounding characters with [vim-surround](https://github.com/tpope/vim-surround)
  * One to open a new buffer
* Mistakenly deleted the wrong migration file and had to rollback my development branch to its most recent commit.  

**Thoughts**:
I spent a decent amount of time figuring out why the .valid? method in my first test woudln't pass, and still wasn't able to figure out after trying several troubleshooting steps.  Couldn't find much about it when Googling either.  I'll have to be persistent.  In the meantime, I flipped over to trying out some new tests.  When I start tomorrow I'll have to continue working on validating a date field so taht it's an actual date and isn't a date in the past.  

Re: Git, the different commands for rolling back changes and when to use each one is something I want to get mmore familiar with - as well as some of the commands in Git that I just haven't used yet.  I think that's something that I don't need to focus on too hardcore, and I have a cheatsheet bookmarked for that in the meantime.

Glad to be digging in a bit more each day and learning how to work more efficiently as well.

**Link to work**:
I should have made more than one commit today, but I just made one.  Here it is:
* https://github.com/twoesplease/budget-app/commit/9272a5ed4decc3e2324ac7467563c693d1e370aa

### Day 67: September 13th, 2017 ###
(1:10 - 2pm, 4:30 - 6:30pm)

**Progress**:
* Drafted some validations and tests for Budget model
* Attended a workshop on Event-Sourced Microservices

**Thoughts**:
For some reason, I couldn't get the basic check for the .valid? method to pass even without validations on the Budget model.  I got some more tests drafted, but I wanted to run them one at a time so that I could follow the model of
-write test
-run test so that it fails
-write code to pass test
-run test so that it passes

I wasn't able to get as much out of the workshop as I'd hoped, because my partner was messaging me during the workshop about an issue with one of my dogs.  Sometimes life happens! :shrug:

**Link to work**:
Here are today's commits:
* https://github.com/twoesplease/budget-app/commit/7f94d9c615d68d2e7d58dcf14e0e68125c52c3f2
* https://github.com/twoesplease/budget-app/commit/d64a492e26241de08a8bdd57a82c293b7d53e0ea

### Day 66: September 12th, 2017 ###
(5:50 - 6:57pm)

**Progress**: 
* Added new user and new budget creation forms to sample app
 * Added link to create new user on the app's home page
 * Add link to create new budget from a user's profile page
* Updated user model to reflect a has-many relationship to budgets, and updated the budget model to reflect a has-many relationship to transactions

**Thoughts**:
Feels good to know a little more about Rails today!  I still have a tone to learn, but the info is definitely coming together a little bit in my brain :)

Outside of my hour of coding time today, I installed the vim-surround plugin which I think will come in super handy once I get good at using it.  I also proposed the idea of doing a fun educational course on Sonic Pi (which I'm newly learning about but think is super cool) to a coworker, so I'm interested to see where that goes.

**Link to work**:
Here are today's commits: 
* https://github.com/twoesplease/budget-app/commit/183075cc37f6f4d14996fcd44f51055fa3b9fc6e
* https://github.com/twoesplease/budget-app/commit/183075cc37f6f4d14996fcd44f51055fa3b9fc6e 

### Day 65: September 11th, 2017 ###
(5:32 - 6:40pm)

**Progress**: 
* Worked on Pegacorn Project
 * Fixed a code error when constructing the end time of the window for counting ONC ticket updates
 * Fiddled with logic for making a websockets connection to the Zendesk Real-time Chat API using the [em-websocket gem](https://github.com/igrigorik/em-websocket), but wasn't able to get it working yet.
 
 **Thoughts**:
 After many emails and multiple chats with multiple Zendesk support agents, on Friday I was finally able to get a workaround for a bug that's been preventing me from getting an OAuth access token.  Now that I've got one, I've been able to connect to the Zendesk chat API which means that I can make progress with the Pegacorn Project.
 
 Today, I reinstalled the [em-websocket gem](https://github.com/igrigorik/em-websocket) on my new machine and worked on the code I'm tring to use to connect to the Real-Time Chat API using that gem -- but I wasn't able to make a successful connection yet.  I know that I'm able to connect to at least the REST portion of the real-time chat API though, because I made some sample cURL requests to verify that my OAuth token was working the other day.  I was worried that I wouldn't have a clue what my code was doing since it's been a while since I looked at it - but luckily, I remembered.  That means what I've been learning is sticking - yay!
 
 I'm a little bummed out that I wasn't able to get the connection working quite yet, but I don't have any Ruby code for the Zendesk API to reference so I'm having to work with the examples I have in the [em-websocket gem](https://github.com/igrigorik/em-websocket) and the [Zendesk Real-Time Chat API documentation](https://developer.zendesk.com/rest_api/docs/chat/apis).  I'll get it.
 
 I also committed some other small updates I've made on the Pegacorn Project outside of my 100 Days of Code work time.
 
 **Link to work**: 
 Here are today's commits:
 * https://github.com/twoesplease/pegacorn_project/commit/e456943863cdd3e1c4ff729206620138f6e6aa88
 * https://github.com/twoesplease/pegacorn_project/commit/eba083d9c0269851c3c506c99dd5007297da6844
 * https://github.com/twoesplease/pegacorn_project/commit/b19e22f734837e769e61ea475c73850db1a007d3

### Day 64: September 10th, 2017 ###
(9:50 - 10:40p) 

**Progress**:
* Got gem download working on new machine, as well as Rubocop in Vim.  
* Rewatched some Rails for Zombies videos.  

**Thoughts**:
Setting up a new machine is a pain.  Also, didn't make it through the hour because I was too tired and needed to sleep.

**Link to work**:
No commits today.

### Day 65: September 9th, 2017 ###
(Much of the day)

**Progress**: 
* Fixed some permissions issues on new machine (my user doesn't have privileges to do an.y.thing)
* Set up a [Kano]https://kano.me/ computer kit with my brother and showed him some cool stuff in [Scratch](https://scratch.mit.edu/) + explained a bit about the [Raspberry Pi](https://en.wikipedia.org/wiki/Raspberry_Pi) computer in the kit
* Also got to play around a bit with [Sonic Pi](http://sonic-pi.net/) - super neat!

**Thoughts**:
I went to visit my family for my dad and brother's birthdays, so I didn't have a ton of time to myself to code.  The time that I did have, I spent trying to resolve some weird permissions issues.

I did spend a good bit of time with my brother using [Scratch](https://scratch.mit.edu/) for the first time along with him.  I'd also never used [Sonic Pi](http://sonic-pi.net/) before, and had a blast doing that!

**Link to work**:
No commits today.

### Day 64: September 8th, 2017###
(Not sure)

**Progress**:
* Rewatched some Rails for Zombies videos.

**Thoughts**: 
I've been working on setting up a new machine I got at work today, and haven't been able to move over the files I've been working in during my 100 Days of Code, so I just did some review today.

**Link to work**:
No commits today.

### Day 61: September 7th, 2017 ###
(8 - 9:26pm)

**Progress**: 
* Removed weird extra "string" column from Users table
* Figured out how to create one-to-many relationships and did some data modeling, then:
  * Created Budget & Transaction models
* Created Budgets controller
* Then realized that I failed to plan descriptive titles for either of my new models when data modeling, so added a name field to Budgets table & a note field to Transactions table
 
 **Thoughts**: 
 I was distracted today because a friend was over at my house hanging out with my partner, and I was helping them make a batch of kombucha.
 
 I'm still feeling like I'm flailing around a bit and don't know which order to do things in - kind of like I'm grasping at straws of disparate info that I've seen somewhere, sometime.  I can feel myself really reaching for structure for this info in my brain though, so I'm hoping it wont' be too long before I get a rough outline down in my brain.
 
 I'm thinking I may re-watch some Rails for Zombies and/or Treehouse Rails videos in spare moments (haha!) to have another format/source to integrate this info into my brain.
 
 **Link to work**:
 Here are today's commits:
 * https://github.com/twoesplease/budget-app/commit/bd45186a70725cc417c015470a8b96e49d28e327
 * https://github.com/twoesplease/budget-app/commit/c88fabf9e90f8a4b714ac358877657920608a43f
 * https://github.com/twoesplease/budget-app/commit/6db4fc754860957ab520ffd2eca395da09c39eb6

### Day 60: September 6th, 2017 ###
(9:15 - 10:20pm)

**Progress**:
* Updated show & new methods in the User model of my Budget App
* Created skeleton User profile page
 * Added a user via Rails console so there'd be a user profile page to show
* Added private method with strong params for User model
* Bonus: Peeked in on CodeNewbie Wednesday chat & answered questions here and there - want to go back and look at replies to the questions from other folks though!

**Thoughts**:
I'm remembering vague pieces of info from the Hartl [Rails Tutorial](https://www.railstutorial.org/book/) book, but they're not as concrete in my mind as I'd like them to be and they don't always reappear at the times I need them.  

I can feel my brain leaning toward getting discouraged for not having memorized this info exactly and having to look things up or struggle through this process a bit, but I'm pushing that away because this is what my learning process is like & I know I'm going to get there.  The best way to do that is to keep building!

I also missed out on my usual lunch break habit of doing some review, which makes me feel a little bummed out but I'll get back at it tomorrow.

**Link to work**:
Here's today's commit: https://github.com/twoesplease/budget-app/commit/bccc361c8fe4f8e06ce1ece2598904803b883f06

### Day 59: September 5th, 2017 ###
(6:25 - 7:39pm)

**Progress**
* Completed a tutorial on Minitest: https://semaphoreci.com/community/tutorials/getting-started-with-minitest
* Troubleshot an issue where my test success/error/failure output was displaying twice

**Thoughts**
Thought I would complete this tutorial and have a bit more time to work on my Budget app, but I got sucked into researching an unforeseen issue - I should know to expect this by now :P

I didn't end up figuring out the issue with my doubled output, even after a stack overflow search, asking in CodeNewbie Slack, unisntalling & reinstalling the minitest gem & the minitest-happy gem, checking in the Exercism Github annals to see if it'd ever instructed me to change my Minitest config, editing the Gemfile for this test project, & peeking through one of the minitest config files saved to my computer.  Oh well, I'll have to keep digging at it another day.

Here are some other resources that I'd like to read through regarding minitest: 
* https://launchschool.com/blog/assert-yourself-an-introduction-to-minitest
* http://docs.seattlerb.org/minitest/

**Link to work**:
Didn't upload anything to Github today.

### Day 58: September 4th, 2017 ###
(8:15 - 9:17pm)

**Progress**
* Used what I've learned from the Hartl [Rails Tutorial](https://www.railstutorial.org/book/) book to add email address validation regex to my User model, as well as create tests for that
* Added a index to the User model's email column to prevent a full-table search when validating email uniqueness

**Thoughts**: 
Again, got stuck on typos here and there, but I also ran into a couple of other weird things that I had to work through and these prevented me from being able to get more done during this hour.  I definitely learned some things though!  

The first thing was that I was getting errors in my email validation tests, and adding custom error messages to those tests allowed me to determine which sample addresses were causing the issue.  I then had to tweak my regex a bit to accomodate some sample addresses from my tests that were, in fact either invalid or valid but weren't testing as such.

The other thing was that the first time I tried to migrate my addition of an index to the User email column in my database, I got an error about an undefined local variable or method "unique."  But I had a mention of uniqueness in my User model...When I googled, a Stack Overflow answer recommended that I re-generate the migration.  When I deleted the old one and created a new one, then tried to migrate it - it worked.  Not sure what was up with that.

**Link to work**:
Here are today's commits:
* https://github.com/twoesplease/budget-app/commit/1c209881b9e8c11f5e66f88484c72b22c70b6c85
* https://github.com/twoesplease/budget-app/commit/ab3d37beda73b0969c227176c9f405da6aaf6114

### Day 57: September 3rd, 2017 ###
(8:47 - 9:49pm)

**Progress**:
* Made some updates to the User model & its tests in my Budget app, heavily inspired/influenced by the process I've been going through in the Hartl tutorial
 * Added secure password requirement to user model
 * Added tests for password validation
 * Started on tests for email validation
 
 **Thoughts**:
I would have liked to have made more progress today, but I got hung up by a couple of typos.  I think it's ok that it's taking me a while because I'm getting used to the errors that I'm seeing, and honestly still have much to learn about how things fit together.  

Trying to dust the cobwebs off the information in my brain, and forcing me to call upon it and use it out of order from the Hartl Rails tutorial and not necessarily exactly in the way described there is going to be awkward at first and it's going to take me some practice to get right.  I'll get there!

I remembered to make separate commits per feature today, but I made them all on my master branch - oops!

**Link to work**:
Here are today's commits:
* https://github.com/twoesplease/budget-app/commit/85cdba353cbf2246eafe65891209fc9d956a223c
* https://github.com/twoesplease/budget-app/commit/b5175c628633a80c57f3b5725255c1a27471e267

### Day 56: September 2nd, 2017 ###
(10:04 - 11:15pm)

**Progress**:
* Finished chapter 7 in the Hartl [Rails Tutorial](https://www.railstutorial.org/book/) book
 * Made it through that test I was stuck on - testing that new user signups direct to the right URL
 * Added flash messages for successful & failed signups
 * Added test for valid user signups
 * Updated production app to use SSL & Puma (instead of WEBrick) webserver
 
**Thoughts**:
After that, all of today's changes felt really relevant and useful, and they're things that I haven't run into much before in other Rails tutorials I've been through.

All this functionality is definitely applicable to my budget app as well, so the next thing I'd like to do is make some updates to that.  I also don't like the fact that I just used a couple of tests out of the Hartl tutorial, so I want to go back through and make those original.

I also remembered to break up my commits today into feature-based ones, and I think that was a good move & a good habit to get into.

**Link to work**:
* https://github.com/twoesplease/sample_app_hartl/commit/fd0198284d22f2558775656576ff5d8aaba74927
* https://github.com/twoesplease/sample_app_hartl/commit/37b9cfa66f6c1824f8466a7d19da4167e4fc6766
* https://github.com/twoesplease/sample_app_hartl/commit/7b71a007d2d55f08c58022ff2f50e978c77d1ff4
* https://github.com/twoesplease/sample_app_hartl/commit/c98f615626efdc53492685413faaa3ca081e1b93
& And here's the link to my signup page live in production!: https://vast-savannah-43395.herokuapp.com/signup

### Day 55: September 1st, 2017 ###
(1:22 - 2:05pm)

**Progress**: 
* Last night, I got stuck on a test that was one of the exercises at the end of a section in the Hartl [Rails Tutorial](https://www.railstutorial.org/book/) book.  It's testing that the form action on the new users signup page is correct, but it keeps failing.
 * Today, I checked a bunch of my files and compared them to the sample code in the book, and they're right as far as I can see.  But when I View Source on the signup page in my browser, the form action URL is not even pointing to a URL that should exist in my app anymore.  I found a source on the form_for method I'm using to create the form, and read up a bit in it.
 
 **Thoughts**:
 Ok, I cheated today because I counted the time I spent during lunch as my coding time, which I don't usually do - but I was super tired when I got home, & chose to catch up a little on my sleep instead of coding more.  I feel a little bad, but I think doing a bit less to catch up on my rest is okay every once in a while.
 
 **Link to work**: No additions today :#

### Day 54: August 31st, 2017 ###
(8:15 - 9:15pm)

**Progress**:
* You guessed it!  Progress in the Hartl [Rails Tutorial](https://www.railstutorial.org/book/) book - today I added a signup form for new users, made it so that error messages display when invalid data is entered, and added tests to make sure that those errors show up and that invalid data can't be submitted. 
  * I also worked with private methods & required vs. permitted parameters, which I need a little review on.  Good thing I'll be re-reading this whole chapter when I go back through it to take notes. :)
* Something else that I did outside my hour today was finally complete a screensharing session with Zendesk support because I still haven't been able to get an Oauth token to use with their real-time chat API, regardless of which of the multiple sets of instructions I follow.  They finally got to see the errors I've been experiencing when I complete the process though, and while our session froze and I didn't get any path toward resolution just yet I plan to check back in with them tomorrow.  This is a small step to move the Pegacorn Project forward.
* Finally, I read a bit about Opal, a Ruby-to-JavaScript compiler, today by watching most of [this talk](https://www.youtube.com/watch?v=6Co0qmCvgq0), asking folks in one of my tech Slack channels about their thoughts on it (positive), and reading a bit about it on Opal's website. I put it at the end of my list of things to learn and/or research because I definitely want to look into it at some point.

  
**Thoughts**: 
I'm having so much fun working through this, and I feel like I'm learning a ton - even though I wish I could just memorize everyting with one pass through it :)

I'm so eager/impatient to work on my own personal projets and be able to have my very own original apps to point people to, but I'm just going to have to be patient and learn these fundamentals before I can do that.

I decided today that after I complete the Pegacorn Project, I want to complete the Pomodoro clock project described over on the [Odin Project website](https://www.theodinproject.com/), and then swap over to [FreeCodeCamp's back-end certification API & dynamic web application projects](https://www.freecodecamp.org/map-aside#nested-collapseDynamicWebApplicationProjects).  Even though FreeCodeCamp is designed to be completed using JavaScript, I'm sure that completing the projects will give me lots of good practice and help me build my portfolio.

I've noticed that my commits have long descriptions, which to me means I should be stopping & committing more often.  I think that each feature (controller udpate to achieve a particular functionality, adding new page, writing tests for a particular functionality) would be a good basis on which to create a commit.

**Link to work**: https://github.com/twoesplease/sample_app_hartl/commit/8d022794ec0aaf16e43bf2be7d48e3480559d4c9

### Day 53: August 30th, 2017 ###
(8:56 - 10:19pm)

**Progress**:
* Continued on my merry way through the Hartl [Rails Tutorial](https://www.railstutorial.org/book/) book - Added CRUD operations for Users to routes file, plus a new #show page to display user info & gravatar.
 * Learned that Rails has a built-in way to generate an MD5 hash - must be a pretty common & useful hashing function
 * Learned that adding a "debug" line to my view file functions the same way as the "byebug" functionality I saw in action for the first time on Monday
 
 **Thoughts**: 
It's so exciting to learn concepts that I can see immediately being applied to my sample budget app and also to pretty much any other Rails app I'll write.

The book noted that this chpater would increase in complexity and difficulty quite a bit, and I'm glad that everything is going smoothly and making sense to me so far.

Sidenote, I made some notes while reviewing a Medium article draft for someone in the Rails channel of the CodeNewbie Slack team, and someone else noted that my attention to detail will serve me well as a developer.  ^.^

**Link to work**:
https://github.com/twoesplease/sample_app_hartl/commit/ca197ecae2971ca087146f982fdcbffd4da81774

### Day 52: August 29th, 2017 ###
(8:50 - 10:30pm)

**Progress**: 
* Finished Chatper 6 in Hartl [Rails Tutorial](https://www.railstutorial.org/book/) book - tested out creating a new User object in database and trying out pasword authentication on it
 * As usual, took notes along the way
* In my personal app, I added tests for presence of name and email, that they're an appropriate length, & that the email is in the rigth format.  I wanted to come up with these tests on my own, but unfortunately I used the same exact tests from the Hartl book because I couldn't think of a way to iterate on them just yet.  I'm sure I'll get there.  One change I plan to make is to require the password validation to also include special characters.
* Also read for a couple of minutes about how to put dotfiles under source control.

**Thoughts**:
It doesn't feel like I wrote a lot up there, but it does feel like I got a good bit accomplished!

**Link to work**: 
Update to my personal budget app: https://github.com/twoesplease/budget-app/blob/master/test/models/user_test.rb
Update to Hartl saample project: https://github.com/twoesplease/sample_app_hartl/commit/cde12aea322a7d47cf14ff907a653db11c24308f

### Day 52: August 28th, 2017 ###
(7 - 9:30pm)

**Progress**:
* Attended Atlanta Ruby Users Group's "Ruby Hack" night, a once-monthly gathering where folks are encouraged to bring Ruby projects they're working on in order to share them and work on them alongside other folks.
 * Talked with the folks there, who were of varying experience levels
 * Introduced [Exercism.io](http://exercism.io/) to the folks there by explaining how it works and showing them examples
 * Observed and threw in suggestions of what I would do for someone who was working on a homework assignment for the Bootcamp they were in
 * Added a very basic model to my budget app
 
 **Thoughts**: 
I would have preferred there to be much more working on projects together than general chat about getting started as a Developer, Industry, and Tools - but the meetup mostly consisted of that.  Next time I'll be more assertive.  Of the five folks who were there (I thought there would be more - 15 RSVP'd), 3 of us were newbies and 2 of the folks were experienced/professional devs so this may have had to do with it.  I got a lot more advice than I necessarily asked for as well - I know folks were trying to be super helpful but it felt a bit condescending.  I want to think of a good way to address that too.

Toward the end, when we started working through the person's BootCamp homework, I thought about how I would solve the problems and was able to compare what I know to what that person knew, and I felt alright about my knowledge level.  I also learned a little about byebug (having never used it before), and I definitely want to read more!
 
**Link to work**: Here's the update to my personal budget app - https://github.com/twoesplease/budget-app/tree/user-model

### Day 51: August 27th, 2017 ###
(9:03 - 10:11pm)

**Progress**: 
* Still chipping away at the Hartl [Rails Tutorial](https://www.railstutorial.org/book/) book, and still on the chapter about updating the data model for Users. Today was about validating uniqueness of email address, updating the User table to have an index, and starting on updating the model to account for a (secure) password requirement.

**Thoughts**: 
I just got back home this evening, and am glad to be back in the realm of reliable internet and being able to push things to Github!  Today I feel like I covered some super important concepts, as well as a couple that seem like they'll take a bit of memorization and review to help stick - fixtures and what they're useful for, validating uniqueness in the database and not just in the model, adding a "before\_save" action in the user model, using Rubular to check regex, and the processes/tools for requiring secure passwords but obscuring them in the database.  

Important concepts that I feel like I picked up today were that you have to create a migration to update the model, the sample case under which duplicate addresses could sneak through the model validations (and therefore why database uniqueness validation should be added too), and an overview on how you can avoid storing a user's password but still check that they entered the right one.

The ATL Ruby Users Group "Hack" night is tomorrow night (where folks come to work on projects), and I'm tempted to go work on my personal Rails project but I'm also a bit apprehensive because I'm so new that I'm a bit embarrassed about all the silly mistakes I'll make and questions I'll have along the way.  We'll see if I venture out...

**Link to work**: https://github.com/twoesplease/sample_app_hartl/tree/modeling-users

### Day 49-50: August 25th - 26th, 2017 ###

**Progress**:
* Continued working through Hartl [Rails Tutorial](https://www.railstutorial.org/book/) book, specifically on the chapter about modeling users in the sample app, and adding validations and tests for presence, length, and uniqueness of the email address & name values.

**Thoughts**: 
I was out of town for a wedding these days without a reliable internet connection, so I didn't post an update.  The first evening I made it through about 40 minutes of coding before getting too tired to stay away, and only 20 minutes on the second night (from about 12:20 - 12:45 am, very late for me!).  While I'm not thrilled to say that I didn't spend very much time working, and I didn't make any progress on my personal app, I'm still learning a ton of valuable info that I know I'll be able to refer back to.  I find that spending time every day, even if it's just a little bit, helps me retain things better than going a long time without review too.  Nothing to be too proud of, but small wins nonetheless.

**Link to work**: Without an internet connection, I wasn't able to push anything to Github.

### Day 48: August 24th, 2017 ###
(1:20 - 1:55pm, 9:40-10:42pm)

**Today's Progress**:
* I usually don't include time spent at my lunch break in this log, but I spent the entirety of the time during my lunch break trying to figure out the testing issue from last night.  I visually compared my code line-by-line to the book's code, thought through how it all fit together, looked at it in the inspector in Chrome, and ran it through an HTML validator - no issues except a mention of a stylistic error in a comment from the validator.  So confusing, because all the links worked when I tried them out!

When I started my hour this evening, I took a look at it again and figured out that it was an extra exclamation point in an HTML comment.  I had them formatted like <!-- comment here --!> rather than \<!-- comment here -->\.  
* I meant to work on my personal app some this evening, but got carried away working through the Hartl book so I continued that this evening - I added an additional test for page titles and used a new test method as well as created the Users controller & corresponding user model.

* I also looked up how to delete branches locally and remotely from Git, which will definitely be a good skill going forward.

**Thoughts**: 
* Even though figuring out that test error helped me learn troubleshooting skills and get a review on how the pieces of a Rails app work together, and it felt GOOD to figure it out without any help, I wish I had been able to spend my time learning something of a bit more import.  I'm sure this won't be the last time this happens though, and it's just something I'll have to get used to.

**Link to work**: https://github.com/twoesplease/sample_app_hartl/commit/b8bc498f634323dfa64fd5e24a510ab93d45fd7d & https://github.com/twoesplease/sample_app_hartl/commit/82d754f2ede6cf364d0d9fa82c95d6fdc4a9e7cc (2 commits today)

### Day 47: August 23rd, 2017 ###
(6:10 - 8:10pm)

**Today's Progress**: 
* Continued reading the Hartl [Rails Tutorial](https://www.railstutorial.org/book/) book & adding code to sample app - today I learned about the elements of the asset pipeline, some benefits of Sass over CSS, updated my routes to named routes, & wrote my first integration tests.
* I also created the skeleton for the persona Rails project I've been wanting to start, a budget app, and wrote the outline for its home page.

**Thoughts**: 
Glad I was able to squeeze in a little extra time today since I didn't get in much time yesterday, and SUPER glad I finally got started on the code for my own personal project, even though it's just a tiny bit.  I felt more lost than I thought I would when I got started on it, but I know just a bit more practice on personal projects will have me feeling much more comfortable.

I'm also glad that I'm getting a taste of testing and seeing the differences between unit and integration tests in real life, because writing software with good test coverage is something I want to get into the habit of.  There is an issue with my first integration test, in that it's not finding the links included in my footer - only those in the header, even though all links work properly when I start a Rails server and visit the app  in my browser.  If I move the links to the header, the test runs fine.  I'll have to investigate that more tomorrow.

This bit of the book is focusing a bit more on front-end than I'm particularly interested in, but I know it will be good to have this more full-stack type experience, is helping me learn some terminology that I've seen floating around online, and having this know-how will allow me to have projects that aren't 100% hideous :P

**Link to work**: 
* Sample app for book: https://github.com/twoesplease/sample_app_hartl/tree/filling-in-layout
* Link to my budget app's repo: https://github.com/twoesplease/budget-app

### Day 46: August 22nd, 2017 ###
(12:30 - 1pm)

**Today's Progress**: 
* Continued reading the Hartl [Rails Tutorial](https://www.railstutorial.org/book/) book & adding code to sample app - today was a good refresher on partials.

**Thoughts**: 
Progress is still feeling slow & I didn't get a whole hour to work today, but I'm trying to focus on the positive that I'm just making progress.

**Link to work**: https://github.com/twoesplease/sample_app_hartl/tree/filling-in-layout


### Day 45: August 21st, 2017 ###
(8:34 - 9:55pm)

**Today's Progress**: 
* Continued reading the Hartl [Rails Tutorial](https://www.railstutorial.org/book/) book & adding code to sample app - today I added some HTML elements to my sample app's home page and styled them using Bootstrap.  Learned a bit about Bootstrap and Sass, which will definitely come in handy later.

**Thoughts**:
Reading while taking notes takes SO MUCH LONGER than just reading this book, but I'm hoping the notes will pay off in me retaining a lot more - as long as I use it, I should retain a fair bit (#crossingfingers).

I will have some code added to my own sample project by the end of this week.

**Link to work**: https://github.com/twoesplease/sample_app_hartl/tree/filling-in-layout

### Day 44: August 20th, 2017 ###
(9:27 - 10:32pm)

**Today's Progress**: 
* Continued reading the Hartl [Rails Tutorial](https://www.railstutorial.org/book/) book and adding code to sample projecdt when recommended
* Drafted page layout and data model for new Rails budget tracker app that I want to make

**Thoughts**: 
It felt good to finally do something that was related to a personal project and not just a tutorial.  Can't wait to start writing the code for this app.

The reading that I did today helped me understand some Rails syntax by showing how it's actually Ruby with some curly braces and parentheses ommitted, which is a big help to me understanding what the heck is going on when I look at Rails code.

**Link to work**: 
* The sample app that I'm working on for the book is live here: http://vast-savannah-43395.herokuapp.com/
* The github repo for the sample app (associated with the book) is here: https://github.com/twoesplease/sample_app_hartl

### Days 41 - 43: August 17th - 19th, 2017 ###

**Progress**: 
* I've been continuing my progress in the Hartl [Rails Tutorial](https://www.railstutorial.org/book/) book and following along by adding my sample code to Github when the book recommends that I do so.

**Thoughts**:
* I feel guilty whenever I spend more time reading than writing code, and I think I need to temper that.  As part of 100 Days of Code, I should be writing at least a bit of code every day.  A stickler for the rules would say that none of the hour of code should be spent on tutorials, but I'm bending them a bit so that I can have more of a variety of samples at the end of my 100 days.

**Link to work**: 
Sample app stays updated on Heroku at http://vast-savannah-43395.herokuapp.com/
### Day 40: August 16th, 2017 ###
(10:10 - 11pm)

**Today's Progress**: 
* Read about TDD in Rails from the Hartl [Rails Tutorial](https://www.railstutorial.org/book/) book and wrote first tests for the sample app I'm coding as part of the learning process for the book.

**Thoughts**:
I generally try to limit learning to my lunch break, but I was super exhausted today so I figured I'd read a bit to progress toward creating my own sample Rails app.

**Link to work**: https://github.com/twoesplease/sample_app_hartl/tree/static-pages

### Day 39: August 15th, 2017 ###
(8:03 - 9:03pm)

**Today's Progress**:
* Reviewed my original solution to [Exercism](http://exercism.io/) "Sieve" problem & found that it did not properly implement the algorith, so tweaked it a bit

**Thoughts**: 
* Glad I reviewed this one, & I feel like if I worked on it just a bit longer I could get it solved properly but alas, I need to prioritize getting  my rest.  Made a bit of progress in the Hartl [Rails Tutorial}(https://www.railstutorial.org/book/) book on my lunch break today, but not enough quite yet to strike out on my own Rails project.

**Link to work**: Didn't upload the problem yet.

### Day 38: August 14th, 2017 
(7:07 - 8:14pm)

**Today's Progress**:
* Completed [Exercism](http://exericsm.io/) "Sieve" problem and got all tests to pass.
 * Didn't submit yet because I want to double check that I implemented the algorithm ([Sieve of Erasthones](https://en.wikipedia.org/wiki/Sieve_of_Eratosthenes) properly.
 
 **Thoughts**: 
 I didn't get much of a lunch break today, so unfortunately didn't get to make any progress in reading the Hartl [Rails Tutorial](https://www.railstutorial.org/book/) book.
 
But I can tell my mind is getting some little Ruby grooves and connections in my neural net that is helping me to grab Ruby information a bit more quickly.  I'm doing alright with Vim too, which probably means I should challenge myself by learning a few new commands :P

**Link to work**: I didn't submit the problem just yet, but I will as soon as I double check it :)

### Day 37: August 13th, 2017 ###
(10:08 - 11:21pm)

**Today's Progress**:
* Read about connecting an [LED backpack](https://learn.adafruit.com/adafruit-led-backpack/0-dot-56-seven-segment-backpack) I got for my Raspberry Pi to the Pi, and took a peek at the Python library used to run it.
* Reviewed most recent comments on my [Exercism](http://exercism.io/) submissions

**Thoughts**:
Whoops, I meant to write some code today but reading about the LED backpack & took a bit, and it's going to be an adventure to figure out how to get it to work with the Pi because the libraries made to work with it are all in Python.  The idea behind getting it was to use it to display the count of whichever data from the Zendesk API is triggering the Pegacorn for the Pegacorn Project.

I also requested the newest Exercism exercise today, but decided to look into the LED backpack instead.

Wish I'd had more time this weekend to make progress in the Hartl book so that I could start on a Rails project.  We'll see if I can make it happen tomorrow.

**Link to work**: No work to link to today.

### Day 36: August 12th, 2017 ###
(8:15pm - 9:22pm)

**Today's Progress**: 
* Did my quickest completion on an [Exercism](http://exercism.io/) problem so far (26 minutes), but it was a very straightforward one (called "Pangram") and I already see ways I can improve it.  I think that's progress though - seeing some of them myself before someone points them out to me.  It's definitely thanks to the person who continually takes the time to comment on my submissions there and what I've learned from those comments.
* Completed the updates I started yesterday to two of my other [Exercism](http://exercism.io/) problems based on comments about them.  
  * For the "Difference of Squares" problem, I updated a method to be more aligned/cohesive with the other methods I used in the exercise & removed a data clump.
  * For the "Raindrops" problem, I removed magic numbers, made it less dense, fixed indentation, removed an unnecessary `#to_s`, & combined an `each` enumerator with separate accumulator to  `#map!`
 
 **Thoughts**: 
 I haven't forgotten that I want to start a Rails project soon, and the reason I haven't yet is because I don't feel I've made it far enough in Michael Hartl's [Rails Tutorial](https://www.railstutorial.org/book/) book to be able to make much progress in a Rails project on my own -- but I want to read more very soon!
 
 Other things that Exercism comments have taught me that I need to learn more about: Big O notation and how to reduce the complexity in my work, not using `#to_a` if I can help it (I keep doing it!!), data clumps and avoiding them, chaining methods to end, review on blocks/procs/lambads (here’s a resource: http://awaxman11.github.io/blog/2013/08/05/what-is-the-difference-between-a-block/ & here’s another: https://mixandgo.com/blog/mastering-ruby-blocks-in-less-than-5-minutes) + short lambda syntax which I used in one of my exercises, metaprogramming (resource: http://yehudakatz.com/2009/11/15/metaprogramming-in-ruby-its-all-about-the-self/), `#freeze` because Rubocop has recommended that I use it & I don’t fully understand why (resource: http://blog.honeybadger.io/when-to-use-freeze-and-frozen-in-ruby/), & \\ magic numbers and what constitutes one (here’s a resource: https://www.eliotsykes.com/magic-numbers).
 
I'm not progressing as quickly as I want to with my Ruby knowledge - though I don't know if anything apart from lightning speed will satisfy me, but I have definitely gotten much more comfortable using Vim.  I'm by no means a power user, but I can get around and do the things I need to do which was definitely holding me back a bit when I first started using it.
 
 **Link to work**:
 * "Pangram" problem: http://exercism.io/submissions/7386639180774e5a9a7c829a4e733436
 * Updated "Difference of Squares" problem: http://exercism.io/submissions/7386639180774e5a9a7c829a4e733436
 * Updated "Raindrops" problem: http://exercism.io/submissions/365f64caa5fa4851bd10cfa9de2b4033
 
### Day 35: August 11th, 2017 ###
(9:15 - 10:15pm)

**Today's Progress**: 
* Made a couple of updates to my "Raindrops" & "Difference of Squares" Exercism exercises based on comments made to my most recent iterations
* Started on the first CodeWars kata, whose instructions were to find the item in a string that differed based on evenness and return its idnex, where the index starts at 1 (rather than 0).  So as an example they gave ("2 4 7 8 10"), from which I should return 3 since the 3rd number is odd.
* I've been speaking with Zendesk support this week, as the steps they've provided in documentation & via email with 2 different reps to get an Oauth token for their real-time chat API (which I need to move forward with the Pegacorn Project) haven't worked for me.  They wanted to set up a remote access session today to watch me go through the process of attempting to get the token, but I felt too sketched out by that concept.  I should take a screencast video to show them my process (& so that I can blur out the appropriate API info as needed) instead.

**Thoughts**: 
Been feeling under the weather and having a hard time focusing today.  The one person who's commented on my Exercism exercises has been pointing out super helpful things like when I could be using a different enumerator method, various code smells they see, that I have a habit of using `#to_a` and separate accumulator and enumerator methods when I don't need to, and when I have data clumps and formatting issues.

With exercises, I'm noticing a trend that the problem seems like it'll be fairly straightforward to solve but gets tricker as I think about the implementation details.  For this one, knowing that I should avoid my habits of using `#to_a`, `#each`, and separate accumulator and enumartor methods made it tricky for me - especially since I'm not super familiar with alternatives to those yet.  That will get easier as I become more familiar with the Ruby documentation.  Wow, I've got a lot to learn!

I really want to get started on a Rails proejct soon, but I haven't made it far enough in the Rails Tutorial book I'm reading by Michael Hartl to really make any progress.  Hope to change that this weekend, but first I've got to rest up and get feeling better.

**Link to work**: None yet, it's all saved on my machine!

### Day 34: August 10th, 2017 ###
(8 - 9:43pm)

**Today's Progress**: 
* Got Rubocop working in & out of Vim by changing file permissions recursively for the necessary .cache directory with `chmod -R` - this allowed all the directories inside of it to have their permissions changed too
* Updated 3 of my previous Vim exercises based on comments from a reviewer as well as offenses found by Rubocop
 * Researched usage and syntax for blocks, procs, lambdas, and enumerators (specifically `#inject`) as part of this process
 * Replaced/removed a couple of unnecessary `#to_a` methods as part of this process as well
 * One submission (RNA Transcription) was too similar to the one before it, so Exercism wouldn't let me resubmit - but I can know in my heart that it's a bit better than it was before
* Installed tldr CLI tool, which is an alternative to man for quick reference
* Submitted request for Opportunity Scholarship to RubyConf 2017

**Thoughts**: 
I'm glad I'm getting a little bit of insight into when and why using certain methods isn't recommended, and which ones are better to use in those scenarios + why.  It's also nice to start getting some style advice to help my code look a little nicer and know what common practice in the Ruby community is.

Going to RubyConf would be super duper neat - looking forward to hearing back about the scholarship!

**Link to work**:
* http://exercism.io/submissions/f08f8bc81b2d4672bf33826528b55005  
* http://exercism.io/submissions/365f64caa5fa4851bd10cfa9de2b4033


### Day 33: August 9th, 2017 ###
(6:45 - 8pm, ~9:30 - 10:15pm)

**Today's Progress**: 
* Attended Atlanta Ruby Users Meetup Group & listened to presentation on CI/CD with Codeship
* Tried to set up Rubocop in Vim, realized it wouldn't work in Vim or in command line
* Reviewed #Exercism comments

**Thoughts**: 

* The presentation on CodeShip was pretty intensive, but it was good to hear a basic overview of how a CI/CD development process could go
* Attempted to install Rubocop since I've gotten comments a couple of times on Exercism exercises that it could help me out with some of the formatting recommendations that could help me
  * After figuring out how to customize the leader key in Vim & realizing I needed to install the rubocop gem *before* attempting to add the plugin in Vim, I realized I was getting the same error message ("Permission denied @ dir_s_mkdir") when attempting to use Rubocop in the CLI and inside Vim (I originally thought it was just a Vim issue).  After investigating on Stack Overflow and changing permissions on a bunch of different directories, I still didn't get it working.
* So thankful for the one same person who keeps commenting on my Exercism exercises with helpful feedback!

**Link to work**: None for today.

### Day 32: August 8th, 2017 ###
(6:01pm - 7:01pm)

**Today's Progress**:
* Emailed Zendesk support team to try to get more info on why the OAuth token I'm trying to use to connect to their Real-Time Chat API isn't working.  Figuring that out will allow me to move forward with the Pegacorn Project.
* Finished Exercism](http://exercism.io/) "Difference of Squares" problem

**Thoughts**
Adding up the time I spent on this Exercism problem yesterday and today, I think i comes very close to an hour.  It was a problem that seemed really straightforward and that I should finish pretty quickly.  Even though I didn't finish as quickly as I expected to and the problem was pretty simple, I'm glad to have finished one in about an hour.

The biggest problem I ran into was issues with scope & using instance variables.  I tried to use an attr_reader when I didn't really need one, which shows me that I really need to get a better grip on scope.  I feel frustrated that I don't understand it better, given how many times I've read about it.  It makes sense in the moment when I read about it, but then I don't remember what I've read.  I really want to find some videos on the topic to see people using it more in real life, but it sounds like I also need to either design some exercises for myself around it (which is difficult since I don't understand it properly) OR find some kind of exercises online, and/or read about them every day so that the info will stick in my brain.

I also used #to_a in one of my methods on the exercise, and the commenter on my "Raindrops" problem told me that #to_a can be a code smell.  I'm not sure what I could or should have used instead in that method, but I'm going to look at other peoples' answers to get some ideas.

**Link to work**: http://exercism.io/submissions/86d9dd70440b43bf888d1249c9831dd2

### Day 31: August 7th, 2017 ###
(8pm - ~9:30pm)

**Today's Progress**: 
* Spent waaay too much time tyring to install the Powerline plugin for vim and all its associated requirements
   * Couldn't end up getting it to work, and then I found the Airline plugin which I was able to get installed in about a minute
* Reviewed a couple of other folks' solutions to the "Raindrops" [Exercism](http://exercism.io/) problem
* Started on the next [Exercism](http://exercism.io/) problem, "Difference of Squares"

**Thoughts**: 
Shoudln't have spent so much time trying to install that darn plugin.  This time is for coding, not customizing my tools!

While I think the Exercism problems are a fantastic exercise, I want to be sure that I spend a good amount of my time working on project-based code too.  I think this will force me to think bigger-picture and in terms of the systems I'm designing and how they'll work together, and will force me to get familiar with other technologies as well.

Perhaps I should start on a Rails project as I'm reading through Michael Hartl's [Rails Tutorial](https://www.railstutorial.org/) book, and do what I can as I learn it.

**Link to work**: Haven't submitted the newest problem yet, so I don't have a link.

### Day 30: August 6th, 2017 ###
(9:34pm - 10:42pm)

**Today's Progress**:
* Finally got all the tests for this [Exercism](http://exercism.io/) "Raindrops" problem to pass, & submitted that problem.
* Also read other solutions to the problem.

**Thoughts**: 
I had my first time where I felt like I knew exactly what I needed to do to solve a small problem that was causing a test failure, and it worked the first time I tried it.  It was just a couple of simple lines that I needed to write to solve it, but I’m so excited to have more of that happen on a larger scale.

Looking through the solutions, I saw that one of them chained methods to end, which I didn’t know was possible.

I was also dismayed that my solution was longer than some of the others, but then I came across one from someone who critiques other solutions frequently (and who I therefore assume knows much more than I do about Ruby), and theirs is similarly long to mine.  I know that shorter isn’t always better because sometimes more verbose code is more human-readable, but I want to strike a good balance.

**Link to work**: http://exercism.io/submissions/779a4004d0484b7389392f6b09bf57e2

### Day 29: August 5th, 2017 ###
(9:54pm - 10:59pm)

**Today's Progress**:
* Continued work on the "Raindrops" [Exercism](http://exercism.io/) problem I've been working on, but fewer tests are passing now than before - whoopsie!  The reason is because I was originally returning prime factors rather than all factors, and since I've gotten that fixed I've broken something else.
* Did a bit more digging last night after I completed my log and came across the updated verion of my file after all, though I'm not sure how.  Vim was asking me if I wanted to use a recovered version, which I tried but none of them were the version I wanted.  When I finally gave up and said that no, I didn't want to use any recovered versions, and lo and behold there was my old version  ¯\\_(ツ)_/¯

**Thoughts**: Wish I was progressing much faster than I am, but I know I'm learning so I'll just keep at it.

One thing that's making me feel discouraged is that I was having trouble writing a method to determine the factors for an integer.  I made it this far:

`def self.find_factors(number)
   range = (1..number)
   range.each do |potential_factor|
     if potential_factor.to_i * range.each {|potential_factor| return potential_factor.to_i} == number
       factors.push(potential_factor)
     else
       puts “skip to the next value in the range”
     end
   end
   factors.uniq!
   puts factors
end`

But, when I looked it up online, I found that I could achieve my goal with just:

`factors = (1..number).select { |n| number % n == 0}
factors.uniq!`

I'm ready to be able to write simpler, more succinct code like that on the first go.

**Link to work**: None yet as I haven't submitted the problem.

### Day 28: August 4th, 2017 ###
(8 - 9:20 pm)

**Today's Progress**: 
* Updated crontab again because yesterday's fix didn't work
 * Today, I specified my full path (including the rbenv shims) before the cron job & that fixed it - now it can find the pi_piper gem
* Continued work on the "Raindrops" [Exercism](http://exercism.io/) problem I've been working on, now 5 out of 19 tests are passing
 * Some of my work from yesterday didn't save so I had to redo it
* Worked a bit more quickly in Vim today

**Thoughts**: 
Wow, I'm shocked how long this problem is taking me to have seemed so simple at first.  I clearly have a lot to learn.  One of the big things that was holding me up today was that the correct output was printing in the middle of the minitest results (like 

SSS.SS.S"Pling"FSSSS

)
& I was confused about why - but it turns out that I wasn't understanding how implicit returns work (though I thought I had a bit of a grasp on it)  & it was creating some funkiness, so I need to review that.  Have an idea about what to fix for the next test that failed.

Also, I just opened Vim back up and none of my work from today saved :( :( :( - good practice for remembering how to do things properly and for practicing Vim as well.  I'm not sure why this keeps happening as I've definitely been saving along the way (and I know I am because my tests are passing after I make changes), but I think I'm forgetting to save one last time before closing and that's messing everything up somehow.

**Link to work**: Haven't uploaded my problem yet.  One day!

### Day 27: August 3rd, 2017 ###
(7:30 - 8:37 pm)

**Today's Progress**:
* Updated crontab because my daily cron to run the count_good_ratings script for the Pegacorn Project hasn't been working since I required the ['pi_piper'](https://github.com/jwhitehorn/pi_piper) gem in it
 * I'd previously tried adding "SHELL=/bin/bash" to have it use the same shell I was working with in Terminal, but that didn't work
 * I found a new solution that recommended I use the same settings as my Ruby version manager, which in my case is RBenv, so I found [this blog post](http://benscheirman.com/2013/12/using-rbenv-in-cron-jobs/) with some steps, but unfortunately that didn't work either so I'll have to do more googling on that
* Continued with the "Raindrops" [Exercism](http://exercism.io/) problem I'm working on while also using 

**Thoughts**: I tried to make my code clean for this problem by putting it in three different methods (in addition to the initialize method) that cascaded from one to another (I wonder if this is a good or bad practice?).  But, the name that the Exercism tests required for the method doing the converting didn't match the method that should run first and I didn't notice that right away so my tests were failing for a silly reason.

I made a small bit of progress today by getting the first test passing but did that by moving everything back into a single method, and boy does it look messy.  I was also working slower than usual again today because I've been continuing to use Vim.

I also watched people solving a couple of Ruby katas on YouTube today, and that was definitely a good idea.  Seeing rspec in action is helpful, as is seeing other peoples' thought processes and ways they go about solving the problems.  Plus, there are other tidbits of knowledge sprinkled about in there as well (like seeing someone use Pry, for example).

### Day 26: August 2nd, 2017 ###
(6:44 - 7:47 pm) 

**Today's Progress**: 
* Continued work on the Raindrops [Exercism](http://exercism.io/)  problem I'm working on

**Thoughts**: Definitely thinking that watching some livecoding videos will help me.  I was using Vim again today, so it held me up a good bit since I'm learning so many shortcuts and a new way of doing things.  But, I also ran into trouble with running my own tests inside my main file of test code than I did with running the suite of tests that come with the problme against the file.  This is because testing in my own file required instantiating objects of the class I created, and I wasn't quite sure how to make a single numeric value available to all 3 of the methods I wrote to solve the problem.  I ended up writing an initialize method containing a class variable and tried to include that class variable as an argument in my other methods, but found out I couldn't do that -- so again, a scope issue I'm running into here that I feel like I should have a grasp on by now.  So excited to feel like I'm finally starting to 'get it' with scope, but I think it may just continue to be an uphill battle hehe.

**Link to work**: Haven't uploaded the problem yet, so nothing to link.

### Day 25: August 1st, 2017 ###
(7:30 - 8:30 pm)

**Today's Progress**:
* Searched for Ruby livecoding streams and ended up watching one about using Sonic Pi with Ruby: https://www.youtube.com/watch?v=r2xMo3J8-CA
* Worked on [Exercism](http://exercism.io/) "Raindrops" problem
* Used Vim for the first time

**Thoughts**:  While the livecoding stream I watched was cool, I didn't learn much about Ruby -- and to be fair that's not what the talk was really intended for, so it was just not the best choice of video that I made for my purposes.  What I was hoping to come across was real-life manipulation of class variables, instance variables, local variables, using the initialize method, and similar scope-related stuff that's been tripping me up.  That's part of why I've been running into trouble with these Exercism exercises, and I feel like I have some sort of block - like I really should be getting it by now.  So I'm thinking seeing folks use them in real life and explain what they're doing will help it click.  

I also didn't get much code written today because I was using Vim for the first time, so it took me MUCH longer than usual to get anything done.

**Link to work:** Haven't submitted the problem yet, so I don't have one.

### Day 24: July 31st, 2017 ###
(7:30 - 8:45pm)

**Today's Progress**: 
* Updated crontab to use bash instead of sh so that it could see the pi_piper gem I added to the count_good_ratings file for the Pegacorn project
* Updated count_onc_ticket_updates & count_good_ratings files in Pegacorn project to have comments be more descriptive
  * Ran into some git issues when trying to merge my development branch with master
  * Thought about consolidating repeated bits of code from count_onc_ticket_updates & count_good_ratings but realized there is only a small bit of repeated code - a lot of it is quite similar, but not exactly the same
* Updated [Exercism](http://exercism.io/) "Convert DNA to RNA" problem based on a comment suggesting that I update a name and an indent
* Started work on [Exercism](http://exercism.io/) "Raindrops" problem and made a good amount of progress

**Thoughts**: I noticed that I felt a little faster when working the Raindrops problem, but I'm nowhere near where I should be - especially given that it is extremely similar to the popular "FizzBuzz" interview question.  I'm still running into issues where I don't have the grasp of scope that I should, so I want to read more code to get myself more familiar with that.  

I also really need to read up on Git because I have a whole heck of a lot to learn there as well.'

**Link to work**: 
* Haven't submitted the "Raindrops" [Exercism](http://exercism.io/) problem yet, so I don't have a link for it
* "Convert DNA to RNA" [Exercism](http://exercism.io/) problem update: http://exercism.io/submissions/47e0e79a67de43f1a3975e31a9866e79
* Update to count_good_ratings in Pegacorn Project: https://github.com/twoesplease/pegacorn_project/blob/master/count_good_ratings.rb
* Update to count_onc_ticket_updates in Pegacorn Project: https://github.com/twoesplease/pegacorn_project/blob/master/count_onc_ticket_updates.rb

### Day 23: July 30th, 2017 ###
(6pm - 7:17pm)

**Today's Progress**: So, I've spent a lot of this afternoon on Raspberry Pi stuff, but I'm only counting a bit of it for my hours of code.  Today I first followed a [YouTube tutorial](https://www.youtube.com/watch?v=UApKArED3JU) on how to light an LED with my Raspberry Pi, and then I used some information from [another tutorial](https://thepihut.com/blogs/raspberry-pi-tutorials/27968772-turning-on-an-led-with-your-raspberry-pis-gpio-pins) along with code from the [Pi_Piper repo](https://github.com/jwhitehorn/pi_piper) to light up and LED using one of the Pi's GPIO pins according to user input and using morse code!

I tried to also move that code to a class and call it on an instantiated object of the class, but I didn't get that working just yet.

Then, I added code to light up the LED for 15 seconds according to the logic in the count_onc_ratings & count_good_ratings files from the Pegacorn Project.  The conditions weren't being met based on the data from the API, so I threw in some fake conditions just to test that the code worked to light up the Pi - it does!  I had to comment it out though because the cron that the one file is running on is running from my laptop rather than the Raspberry Pi.

**Thoughts**: There was a lot of learning going on today, as well as a good bit of waiting for things to download to the Pi (and putting a fan on it so it didn't overheat).  I'd never used a breaboard or read about how to build a circuit before, so I was starting from level zero there and was glad that there were so many online tutorials to choose from.

I updated the code from the [Pi Piper repo's Morse Code example](https://github.com/jwhitehorn/pi_piper/tree/develop/examples/morse_code) a bit so that the block requesting input didn't loop forever, and so that it would work with the newest version of Ruby -- one of the data types didn't respond to the method being applied to it any longer.  I hope I didn't create a forking disaster, because I've never done that before either.

I also don't have alligator clips or M/F jumper cables, so I had to make sure that the cables I was using made contact just right.  Overall, I feel like I made some good progress on the Pegacorn Project today!

Future steps for the Pegacorn Project are to refactor the ount_good_ratings and count_onc_ticket_updates files to remove duplicated code, get jumper cables that will stay connected or alligator clips for the Pi, get the watch_chat_waits code working with the Streaming Chat API, add crons to the Pi to run each script, and figure out how to update my hardware and code to work with the voltage for th Pegacorn.

I'd also like to get the Pi Piper morse code project to work when calling it from an instantiated object of a class.

**Link to work**: 
* Fork to Pi Piper repo: https://github.com/twoesplease/pi_piper/commit/c8c3f003e3cb527eec4213e3f50daa0d8ff6245f
* Update to count_good_ratings in Pegacorn Project: https://github.com/twoesplease/pegacorn_project/blob/master/count_good_ratings.rb
* Update to count_onc_ticket_updates in Pegacorn Project: https://github.com/twoesplease/pegacorn_project/blob/master/count_onc_ticket_updates.rb

### Day 22: July 29th, 2017 ###
(10:20 - 11:30pm)

**Today's Progress**: I refactored the my code from yesterday's Exercism problem based on some detailed feedback I received from a commenter.  I also peeked at one other person's solution to compare it to mine.

**Thoughts**: I didn't want to steal ideas from the other submitter's code in refactoring my own, though I know that reading other peoples' code is one of the best ways to learn.  I'm really thankful for the suggestions from the person who commented on my code, though one thing that's bothering me is that they said there was a bug in my original code and I'm not sure what it was.  There were a couple of small things that I thought it might be, but they seemed more formatting-related than logical issues - so I'm worried I didn't get it.  The code still passes all the tests though and I think is cleaner for the edits that I made.  There was also an example of good code that the commenter included that I didn't think was fantastic, because it was an if statement that didn't use an 'else' in the last line of the clause.  I thought that made it a bit confusing and more difficult to read, but perhaps writing the statements that way is a Ruby convention?  I'll find out with more code.

Now that I've made another submission, I'd like to go through and look at other peoples' solutions before I review my own again.

**Link to work**: http://exercism.io/submissions/47e0e79a67de43f1a3975e31a9866e79

### Day 21: July 28th, 2017 ###
(9:28 - 10:28pm)

**Today's Progress**: I took a sick day from work today, but I still go my hour in.  It took me the whole hour, but I did finish the [Exercism](http://exercism.io/) "Convert DNA to RNA" problem.

**Thoughts**: Still feeling like I should have finished this one much faster, but I picked up a lot that I hope I retain along the way.  Issues that I remember running into over the few sessions I've worked on this, or things that I have learned:

* Not being able to access a hash defined within a class from a method inside that class
* Figuring out how to compare each character in a string with all the keys in an array was tricky
* I ran into issues with invalid arguments that were more than one character in length, I believe because I needed to use #all? rather than .each or #any?
* The #any? method is in the Array class documentation, but the #all? method is in the Enumerable mixin documentation
* I had to look up how to implement the RegEx I needed in order to use the #gsub! method
* My code was pretty long and included nested if statements within if/case statements at one point, but I found a way to shorten it without making it too hard to read #phew -- I was checking the length of a string and applying different rules based on that, but then I found out that the #split method works even on a 1-character string so I didn't need to do that any longer
* I had to remind myself how to properly include the BookKeeping module and how to submit the problem

I haven't yet compared my answer to others', but I plan to tomorrow.

**Link to work**: http://exercism.io/submissions/a594707099534bf7a17a9766122643d1

### Day 20: July 27th, 2017 ###
(8:43 - 8:58pm)

**Today's Progress**: Yesterday I heard back from the Websockets API developers about a bug I reported yesterday that was preventing me from getting an OAuth token that I could use to authenticate against the API.  Today they emailed me back to tell me how to resolve that issue, but I wasn't able to successfully authenticate via cURL or a Ruby script with the client secret I got.  Going to see if someone at work runs into the same problem as me and if so, I'll email the API developers again.

During my project-related coding time I continued work on the [Exercism](http://exercism.io/) "Convert DNA to RNA" problem.  I got 5/8 of the tests to pass, and now have to get my code to respond properly to invalid input.

**Thoughts**: Was too tired today to do 2 hours of project-related coding, so I'll have to catch up this weekend.  Feeling discouraged because I feel like this exercise should be really simple, but I'm getting hung up.  I'm gaining more familiarity now with common hash and string methods though, as well as scope-related errors and testing methods - so this struggling is positive overall.

**Link to work**: I'll have it once I submit the problem.

### Day 19: July 26th, 2017 ###
(6:30 - 9:30pm)

**Today's Progress**: Attended a Rails Meetup and watched a presentation called "Starting a Career with a Mindset of Testing," then mob programmed tests for a sample Rails app as a group.  I plan to do 2 hours of project-related coding tomorrow since I didn't do that today.

**Thoughts**: I wrote my first-ever test, volunteered to be the first participant to "drive" during the mob programming session, and participated by describing what to code next to other "drivers" as well.  One of the organizers was describing the MVC model to someone who asked a question, and when I offered a diagram to help them explain, they asked me to try explaining instead.  I did, and got the general message across - which felt good!  Definitely could use some polishing but explaining things to others truly is a good (though scary) way to learn.

So glad I got my learning about testing in general and RSpec specifically started, because I want to get into good habits with that by using TDD/BDD as a general rule.  I'd like to add some tests to my Pegacorn Project code soon!

**Link to work**: Don't have one for today.

### Day 18: July 25th, 2017 ###
(9:43 - 11pm)

**Today's Progress**: Before my hour, I learned that there is a whole separate workflow I need to go through in order to generate OAuth creds for the Zendesk Real-time chat API, which uses Websockets, than for the Zendesk core API.  I wasn't able to login to the right place to get that process started and didn't receive a password reset when I requested one, so I chatted with support.  They weren't sure what was going on and asked me to keep trying and come back tomorrow.

During my hour, I worked on the [Exercism](http://exercism.io/) "Convert DNA to RNA" problem.  I started working again in Spacemacs today, so I admittedly spent some of my hour configuring Spacemacs settings since I've recently uninstalled and reinstalled it.

**Thoughts**: I was initially excited about the "Convert DNA to RNA" problem because it looked like something I'd be able to knock out quickly and without much trouble.  However, I ran into issues in implementation with scope and syntax that have me feeling discouraged because I should definitely be able to solve them.  Those are pretty motivating for me to switch up my approach though so that I'm practicing problems like this at some point every day to avoid getting rusty.  Perhaps I can start spending a few minutes per day on a break at work on them.

**Link to work**: Didn't upload my exercise yet so I don't have a link to it.

### Day 17: July 24th, 2017 ###
(8:03 - 8:46pm, 9:25 - 10:07pm)

**Today's Progress**: Asked for help from someone at work and from my mentor (who I had a scheduled meeting with today), and got some tips that the OAuth flow likely involves 2 or 3 more steps.  I dug around in the documentation and found a description of those steps for one of the APIs I'm working with, and got those creds to work.  

For the Real-Time-Chat/WebSockets API I'm working with though, I haven't been able to get those same steps to work.  It also gives much less helpful (read: largely nonexistent) error messages.

Asked a third person for help with an electrical question I had about the wiring I need to use, and got the info I needed from them as well.

Also ran into some Git trickiness today (always when trying to merge my two branches), and ended up trying out a git stash which did not work out as easily as I wanted it to.  That created a few extra minutes of work but is all good learning for me in the end.

**Thoughts**: I've pushed myself to ask for help much more frequently than I feel comfortable with (especially today), and overall it's been moving me in the right direction.  Sometimes it made me feel silly for not already knowing what I was asking about, and feeling like I should have just checked that one last online resource.  When I asked my mentor for help, I felt validated because she told me OAuth was a notoriously tricky process to deal with.  When I asked for electrical help, I felt silly for asking but the right answer was the one I was guessing so it wasn't so bad.

All in all, asking for help is giving me new avenues and ideas to look for and moving me forward in this project and in my knowledge overall.  Sometimes people are super nice, and sometimes less so, but so far no one has refused to give me info.  One day someone might scold me for not knowing what I'm asking them about, and I'm going to go ahead and tell myself now that either that will be a good tip for info I should review -- or perhaps I'll just have to let it roll off my back because I know what I need to know better than that person does.

**Link to work**: (Not much of an update here today because most of my work was done making cURL requests to various endpoints and copying the data they returned into temporary text files): https://github.com/twoesplease/pegacorn_project/blob/master/watch_chat_waits.rb

### Day 16: July 23rd, 2017 ###
(10:15 - 11:23pm)

**Today's Progress**: Made a cURL request with my auth creds for the WebSockets (WS) bit of my project today and found that I don't have authorization to access the WS server.  Regenerated my creds, but got the same result.  I think I tried this right after generating the creds, but the cURL request didn't work -- can't remember why exactly, but perhaps it was because it was so shortly after I'd generated them.

Since I was stuck without being able to use my auth creds, I pulled up the [Exercism](http://exercism.io/) Gigasecond exercise that I'd started long ago and worked on that until my hour was over.

**Thoughts**: I wish I'd tried this basic step again sooner.  I know I've been learning a bit from fiddling around with the code and wondering whether slight changes would work and why, but I could've probably moved a lot further by now.  I can do a bit more research to see if there's a way to update the permissions on my auth creds, and in the meantime can work on adding code to my first two files that are working to light up an LED on my Raspberry Pi. 

**Link to work**: (Link to [Exercism](http://exercism.io/) Hamming Exercise not included, only today's updates to the WebSockets-related file) https://github.com/twoesplease/pegacorn_project/blob/master/watch_chat_waits.rb 

### Day 15: July 22nd, 2017 ###
(8 - 9:50pm)

**Today's Progress**: Today I got my Raspberry Pi up and running, and I'm typing today's update on it right now!  I installed Ruby, rvm, updated the keyboard layout, and worked through some display issues.  I cloned my Pegacorn Github repo, and had to create a local file for my secrets on the pi and then update the code to point to it - but, I got one of the scripts working and talking to the Zendesk API!

Next, I looked up a project for lighting an LED on RPi using Ruby code, since I eventually want the output I'm getting from the Zendesk API to trigger a light.  I found one using the gem pi_piper (which is, as the name indicates, designed for use with Raspberry Pi), and decided to copy the Morse Code example in the pi_piper Github repo: https://github.com/jwhitehorn/pi_piper/tree/develop/examples/morse_code

I ran into an error when attempting to install the pi_piper gem (something about not being able to find headers), and found a StackOverflow answer that recommended I run 'sudo apt-get install ruby-dev' first, which worked.   

I typed up the code (rather than copy pasting) from the morse code example project above so that I could be sure I understood what it was doing, but since I don't have any experience with electrical engineering of any sort, I've been doing research online about how to set up the circuit since then.  I'm thinking I'll look back into that tomorrow - I know I have all the parts I need except I'm not sure whether I truly need male/female wires or can just use plain old jumper wires without extra stuff added to each end.  I may watch a YouTube video or two on that before going to sleep tonight.

**Thoughts**: So much more to learn as far as electrical engineering goes, but it's good to know a bit about the topic in general, and it will help me with future projects that I'm interested in taking on around the house, like building a water system that checks the soil mositure to deliver the right amount of water or an automatic chicken pen door opener/closer.  I just want to be sure that I keep my main focus on coding and remember that the electrical engineering learning is secondary.

**Link to work**: I haven't uploaded anything to Github yet, but hopefully I'll be able to add some code that talks to my Pi soon!

### Day 14: July 21st, 2017 ###
(9:55 - 11pm)

**Today's Progress**: Today I compared the example Node.js code in the Zendesk documentation with mine to look for differences and see why it might not be working, but didn't find anything.  Next, I copied that Node.js code into my own file, spent some time setting up my machine to run it, and found that I got very similar results to when I ran my own code.

I asked the only other person at work today who I can see has generated an OAuth token, but they haven't connected to the Real-time Chat API so I'm not able to see how they did it.  My hypotheses for why my code might not be working are that either my OAuth token doesn't work (though I would expect an error message noting that I wasn't authorized), the whole real-time chat API is broken, or I'm not subscribing to the metrics I want properly (aka something is wrong in my code).

Next steps to troubleshoot this: 
* Double check OAuth requirements to see if simply generating a token isn't enough
* See if I can find a status indicator for the real-time chat API, look again in Zendesk help forums to see if anyone is experiencing a similar problem
* Make a websockets connection to another service to see if I'm able to do so successfully

**Thoughts**: Annoyed that I'm stuck here, but I have the necessary equipment to work on the Raspberry Pi now so I can switch over to working on that if I need a break from this.  I'd like to make some progress on that this weekend anyway.

**Link to work**: I haven't uploaded anything to Github today.

### Day 13: July 20th, 2017 ###
(7:55 - 8:55pm)

**Today's Progress**: Updated the type of authentication I was using and tried many variations of the couple of options hashes (based on example code from the Github repo for the EventMachine-HTTP-Request gem I'm using), but still wasn't able to get anything back from the WebSockets server but a response code of 0 and an empty header. 

**Thoughts**: Hitting a low-level frustration at being stuck on the same step for a few days now, and I'm not getting any helpful error messages back from the WebSocket server to point me in the right direction.  My plan for tomorrow is to rubber duck my way through the node.js example code in the Zendesk documentation and compare it to mine to see what might be different.  If that doesn't work, I'm going to copy/paste & run it from my machine to determine if it's maybe just my OAuth token that's busted.  At least I've got a plan.

Also got a new keyboard and mouse today so taht I can connect to and work on my Raspberry Pi this weekend!

**Link to work**: https://github.com/twoesplease/pegacorn_project/blob/master/watch_chat_waits.rb

### Day 12: July 19th, 2017 ###
(7:06 - 7:23pm, 7:46 - 8:39pm)

**Today's Progress**: Switched it up and watched an old *webcast* about WebSockets today.  Updated code to attempt to push a request to the WebSockets server and parse errors, but am getting an error code of 0 and nothing in the response headers so it seems like I'm not making it as far as a connection to the WebSockets server.  I copied the example code fro mteh screencast though and was able to successfully make a WebSockets connection to google.com, but not to the server I need to connect to for my project.  

Ran into more Git merge coflicts when attmepting to commit my changes, so I'm learning about Git that way.

Outside of my hour, I made some CSS updates to my page at toneeyoung.com.  I don't have any code-related forté at the moment, but front-end definitely aint' it.

**Thoughts**: Well, I still don't understand much of WebSockets at all but it feels like I've made the tiniest bit of progress.  I aws feeling sicky today, so I'm glad I stuck it out and did my hour of code anyway.

**Link to work**: https://github.com/twoesplease/pegacorn_project/blob/master/watch_chat_waits.rb

### Day 11: July 18th, 2017 ###
(10 - 11:13pm)

**Today's Progress**: Did still more reading on how to set up a streaming WebSockets connection in Ruby, and updated code to add the basic steps for establishing a connection.  Wrote pseudocode for how to subscribe to the particular Zendesk chat metric I want to monitor, and added TODOs as comments to my file.  When attempting to merge all my updates, I ran into a merge conflict caused by me not switching to my development branch at the beginning of my hour.

**Thoughts**: Kind of dismayed that I spent so much time reading again, but I feel like I've found a request structure that will work and have a good next step or two to go off of when I sit down for my hour of code tomorrow.  Also glad I was forced to resolve a merge conflict in Git - this doesn't see like the last time I'll run into that!

**Link to work**: https://github.com/twoesplease/pegacorn_project/blob/master/watch_chat_waits.rb

### Day 10: July 17th, 2017 ###
(9:55 - 11:10pm)

**Today's Progress**: Fixed bug in date params for ONC counter, so I believe it's finished until I figure out how to connect it to the Raspberry Pi.  Read more on Websockets and changed my chat waits watcher to use EventMachine libraries based on this tutorial: https://github.com/pusher/websockets-from-scratch-tutorial.  Tried out the small bit of code I copy pasted but didn't get any sort of reply from the server - not even an authentication error, which I should get since I haven't entered any credentials yet.  

**Thoughts**: There are so many short getting started guides on Websockets, and they all use different libraries.  I don't want to build a Rails or Sinatra app just to grab chat wait times, so that cuts down on the resources a bit.  Ideally I'd like to be able to do this using just the Ruby core library, but perhaps these EventMachine libraries can help me get going a bit faster.

**Link to work**: https://github.com/pusher/websockets-from-scratch-tutorial


### Day 9: July 16th, 2017 ###
(4:35 - 5:40pm)

**Today's Progress**: Added date to ONC counter API call params (but it doesn't seem to be working), started on the streaming API portion of this project that needs to use Websockets + read several articles about that.

**Thoughts**: I felt bad spending so much of my time reading about how to use Websockets, but I imagine that much of a professional dev's time is spent reading documentation as well sso I'm trying not to be too hard on myself about that. Doing some noodling on how to troubleshooting the API params that aren't working for the ONC counter.

**Link to work**: https://github.com/twoesplease/pegacorn_project/blob/master/watch_chat_waits.rb

### Day 8: July 15th, 2017 ###
(9 - 10:17pm)

**Today's Progress**: Made some formatting changes, wrote methods to generate ISO-formatted times for today at 8pm & tomorrow at 6am, and wrote some descriptive comments to help with understanding those methods.  Looked up and used the map method on an array for the first time.

Outside of my hour, I udpated my Terminal prompt to show my current git branch in a contrasting color.

**Thoughts**: Digging in to the slightly-tricky logic of converting today's ISO date to tomorrow has been fun, and I'm glad that I got most of that done within a single hour.  The API call isn't returning the results I thought it would when I interpolate the timestamps I generated into the params, so I'd like to do more testing on that sometime soon.

I'm at the point now where I'm ready to hook up the Raspberry Pi and start figuring out how to get my code onto it and working, so I ordered a separate keyboard for it today.  I also need to go ahead and order a USB adapter so that I can connect an external monitor to it.

**Link to work**: https://github.com/twoesplease/pegacorn_project/blob/master/count_onc_ticket_updates.rb

### Day 7: July 14th, 2017 ###
(10:20 - 11:23pm)

**Today's Progress**: My cron didn't run properly today due to a relative filepath, so I hardcoded that today.  I also updated the required # of good ratings to 300 rather than 400, and did some fighting with the Zendesk search API.  I was getting a 422: Unprocessable Entity error for a while but finally got some params that I know will work for the search API.  I haven't been able to interpolate in a date param stored in a variable yet, and that's what I've gotta figure out next.

**Thoughts**: Outside of my hour of code today, I watched a bit of a livecoding stream and I really enjoyed seeing a well-versed developer work and describe her work, especially the debugging portion.  I also updated my prompt in iTerm to 👾 👻, which is fun.  Ready to make more substantial progress on this search endpoint.  I'm also excited to get the raspberry pi hooked up and figure out how to trigger a small light before I go for the pegacorn.

**Link to work**: https://github.com/twoesplease/pegacorn_project/blob/master/count_onc_ticket_updates.rb

### Day 6: July 13th, 2017 ###
(9:41 - 10:52pm)

**Today's Progress**: Got my API credentials hidden in my files, moved them to a new directory with an empty Git history, and got them added to a repo on Github.  Learned that my Ruby files aren't in the mood to allow me to require YAML files today, as well as the syntax for including variables from another file as basic_auth arguments for a net/http request.  Updated my cron job to point to the new directory.

**Thoughts**: Kind of surprised that it took me the whole of another hour to get this working, so I hope I retain what I learned.  I'm positive that including variables from another file will come up again in the future.

**Link to work**: (It's currently a mess, but I'm glad I can include this now) https://github.com/twoesplease/pegacorn_project

### Day 5: July 12th, 2017 ###
(9:30 - 10:47pm)

**Today's Progress**: Updated my cron job earlier today so that it appends to the log file rather than overwriting it each time.  Spent most of my hour today working on setting up environment variables to hide my API creds, but couldn't get them working right and none of the stack overflow answers I read was helpful.  And this one seemed like such a simple one!  But I guess the $PATH never is.  May just move them to a .gitignored config file instead.

**Thoughts**: Not surprisingly, researching one of the things that I thought would be most straightforward led to my least productive day (in terms of lines of code written) of the challenge thus far.  Aside from that, I attended my first Ruby users' Meetup today and actually had a good idea of what was going on + got some good info out of it.  One of the talks was even directly relevant to the DateTime issues I'm working through on the Pegacorn Project right now.

**Link to work**: Alas, it's still on my machine.

### Day 4: July 11th, 2017 ###
(8:10 - 9:10pm)

**Today's Progress**: Got my cron from yesterday working.  It's been running today, but outputting errors to the log - apparently Ruby syntax that runs in Terminal doesn't necessarily fly for cron jobs, so I had to make a quick syntactical update to get the cron working.  I also started work on the next endpoint I need to hit, and started on formatting my params properly for that.  Finished off my hour in the middle of trying to figure out how to format a DateTime object with a proper offset for my timezone in order to interpolate it into a param.

**Thoughts**: Was surprised about that syntax thing with the cron - making a note on my Learning List to look that up.  Timezones are indeed fiddly, so I'll be glad to figure this bit out.

**Link to work**: Need to do a bit more research on environment variables so I can hide my API creds and upload my work to Github.

### Day 3: July 10th, 2017 ###
(9:35 - 10:40pm)

**Today's Progress**: Finished the logic dealing directly with the API and data it returns from one of the four endpoints I need to access and started my first foray into dealing cron jobs and the cron tab.  Learned enough to be dangerous, and found out that sometimes Terminal will tell me that I have mail ("You have mail in /var/mail/user")!  We'll see tomorrow when I log on if my scheduled task works.

**Thoughts**: Learning about crontabs and cron jobs is cool because they're something that I've heard about for so long but not exactly understood.  I certainly don't know the whole of them now, but I know enough to use them and be dangerous!  It's also interesting to find out how simple some concepts are once you find someone (or a blog) willing to explain them to you without using tons of opaque terminology or shrugging you off by saying "it's complicated."

**Link to work**: This project is still saved on my machine.

### Day 2: July 9th, 2017 ###
(3:05 - 4:05pm)

**Today's Progress**: Figured out how adjust the current date to an Epoch timestamp, then add a fixed value to it so that the date in the params is always today's date at 5am EST.  Also determined how to accurately count the number of ratings and create a conditional based on that count.

**Thoughts**: Got stuck on some scoping issues, which I was already aware I need to read up more on.  I skipped around them for now.  This bit of work that I've gotten done so far is small, but I'm still proud of my progress.  I think it's a solid start for this project, and a good start for my daily coding practice.

**Link to work**: The work is saved on my machine.

### Day 1: July 8th, 2017 ###
(10:05 - 11:10pm)

**Today's Progress**: Continued work on Pegacorn Project.  I figured out how to get my url params working (it had to do with the allowed filters for the particular endpoint I'm working with), and created a method using DateTime that I plan to use to update the params for the API call I'm making with the current day's date.

**Thoughts**: Earlier today and at the start of my hour of coding I was feeling overwhelmed at how much there is to learn.  Even though that's still true, I have a better handle on what I want my learning plan to be after some research I did earlier.  Also, even working through the small issues I'm running into now give me a boost of confidence that makes me feel excited and hopeful about my ability to keep learning and get proficient with this stuff.

**Link to work**: Don't have one as it contains my auth credentials for the API I'm accessing.  It's stored in a directory on my machine.

### Day 0: July 7th, 2017 ###
(9:15 - 10:15pm)

 **Today's Progress**: Started Ruby code for Pegacorn Project & put it under local source control with Git.  Successfully communicated with and parsed outcome from a REST API.

**Thoughts:** So glad I was able to get my gems, homebrew, and rbenv to play nice with each other this morning before starting the challenge.  Looking forward to to the days when I'll be able to do this kind of task on autopilot, and hoping they won't be too long from now.

**Link to work:** Don't have one as it contains my auth credentials for the API I'm accessing.  It's stored in a directory on my machine.
