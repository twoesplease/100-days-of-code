# 100 Days Of Code - Log

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
