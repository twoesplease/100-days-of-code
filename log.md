# 100 Days Of Code - Log

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
