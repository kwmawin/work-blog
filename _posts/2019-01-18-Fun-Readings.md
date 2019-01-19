---
layout: post
title: Fun Readings (updating)
categories: [read]
---
This post is used as my notebook for fun readings I recently found on LinkedIn, Medium, and many other places. I will continue to update and add more links!

**Oct 24, 2018:** [Curiosity and Procrastination](https://ai.googleblog.com/2018/10/curiosity-and-procrastination-in.html) by Google AI. This article briefly introduced Google AI's work on curiosity-driven exploration, where while continuing on predicting the future, the agent tends to be "curious" and rewards "surprise," which means when the agent sees something different from their prediction, it tends to go further and explore it. This is very helpful when working on task such as escaping from a maze. One side-effect is "procrastination," where the agent at the same time tends to be attracted by randomly changing object. I really like the example of a TV randomly switching channels. Even if the there is only small number of channels, the randomness will mostly cause surprise to the agent and attract it away from exploring the other parts of world. This effect can pretty much be seen in real world, on each of us human!

**Nov 30, 2018:** [An Inside Look at Reddit's Video Infrastructure](https://www.linkedin.com/pulse/inside-look-reddits-video-infrastructure-chris-slowe/) by Chris Slowe, CTO of Reddit. It is interesting to see the idea of temporary and permanent buckets, and how Reddit uses them to handle large amount of video uploads and prevent from failed upload to mess up their database. Once videos moved to permanent buckets, transcoding task will then started by AWS Lambda. 