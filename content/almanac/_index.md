---
categories:
- Projects
date: "2019-9-1"
description: Almanac
tags:
- projects
title: Almanac
---

{{< figure src="screenshot.png">}}

Autograph is a tool for life journaling that I wrote. I Wanted a journaling tool that was light weight and not web based as I wanted to keep my log on my local machine instead of on the web for everyone to see. All it had to do was the following:

* Create entries in a log with a subject field
* Be able to search and display the log by date or subject
* Count how many posts each subject had
* Linux (and os x)

The CLI was perfect for this kind of task as it doesn't need a fancy UI to work. It seemed like shell script also seemed like a sensible option for this, all i was going to be doing was appending text to a log file so writing a script to do it seemed easier than bothering to put something together in C. I ended up finding the tool quite handy so decided to share it.

View the source and download on [Github](https://github.com/jameschip/Almanac)

