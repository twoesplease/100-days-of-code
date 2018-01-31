# 100 Days Of Code, Round 2 - Log

## Going forward, I'll be tracking my progress on my [personal blog](http://toneeyoung.com).

### Day 4: November 26th, 2017 ###
(6:45pm - 8:05pm)

**Progress**:
* Figured out local config issue that was holding me up
* Worked on showing remaining amount left to save in Budget app
  
**Thoughts**:
Here's how I figured out the local config issue: Ruby has upgraded to 2.4.2, but my Rails server was looking in a nonexistent folder whose name included ruby 2.4.1 for gem-related info.  When I created a symbolic link from the nonexistent 2.4.1 folder to the 2.4.2 folder that was on my machine, the Rails server started.

I added a couple of fields to my Transactions and Budget tables and attempted to do some math in the models so that I could sum the amount of all the transactions for a budget and then subtract that from the goal total for the budget to get the remaining amount.  I haven't got everything tweaked right just yet, but I learned some Rails commands for doing calculations on database contents, which is pretty cool.

**Link to work**:
* https://github.com/twoesplease/budget-app/commit/70270e175fe6d238ba7d25768ebbfeaad7b7156f

## Note - Skipped 11/23 because I was at Harry Potter World with my family and we didn't get in until close to midnight.  I needed sleep!

### Day 3: November 24th, 2017 ###
(8:45pm - 9:47pm)

**Progress**:
* Fought with local config issues the whole time
  
**Thoughts**:
Local config issues are such a bummer!  It seems like I've run into this one before but I can't remember what I did to fix it.  When I try to start Rails server, I get an error message that Rails can't fin the gems it needs.  Uninstalling and reinstalling the first couple of gems worked, but for the third one it didn't.

**Link to work**:
No link to speak of :(

## Note - Skipped 11/23 because I was at Harry Potter World with my family and we didn't get in until close to midnight.  I needed sleep!

### Day 2: November 22nd, 2017 ###
(1:07 - 2pm)

**Progress**:
* Only completed 1 kata on CodeWars and started on another one.
  
**Thoughts**:
While the first kata took me waaay too long to solve (it seems like I generally try to make things into more steps than they need to be), I felt like I knew what to do on the second one right away.  Unfotunately, that wasn't quite the thing I needed to do.  I feel like I got close to solving it, but then it was time for my lunch break to be over so I had to quit.

**Link to work**:
No commits for the day, but here is a link to the kata that I've completed on CodeWars: https://www.codewars.com/users/twoesplease/completed

### Day 1: November 21st, 2017 ###
(1:30 - 2pm, 9:25 - 10:23 pm)

**Progress**:
* Completed 4 kata on CodeWars today
  
**Thoughts**:
Wow, I felt a little rustydoing this even though it seems like it hasn't been very long since I was coding daily.  There's certainly something to be said for daily practice.

**Link to work**:
No commits for the day, but here is a link to the kata that I've completed on CodeWars: https://www.codewars.com/users/twoesplease/completed
