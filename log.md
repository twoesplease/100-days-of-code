# 100 Days Of Code - Log

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
