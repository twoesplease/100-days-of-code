# 100 Days Of Code - Log

### Day 27: August 3rd, 2017 ###
(7:30 - 8:37 pm)

**Today's Progress**:
* Updated crontab because my daily cron to run the count_good_ratings script for the Pegacorn Project hasn't been working since I required the ['pi_piper'](https://github.com/jwhitehorn/pi_piper) gem in it
 * I'd previously tried adding "SHELL=/bin/bash" to have it use the same shell I was working with in Terminal, but that didn't work
 * I found a new solution that recommended I use the same settings as my Ruby version manager, which in my case is RBenv, so I found [this blog post](http://benscheirman.com/2013/12/using-rbenv-in-cron-jobs/) with some steps, but unfortunately that didn't work either so I'll have to do more googling on that
* Continued with the Raindrops [Exercism](http://exercism.io/)problem I'm working on while also using 

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
