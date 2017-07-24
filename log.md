# 100 Days Of Code - Log

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
