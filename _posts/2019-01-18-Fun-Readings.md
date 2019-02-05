---
layout: post
title: Fun Readings (updating)
categories: [read]
---
This post is used as my notebook for fun readings I recently found on LinkedIn, Medium, and many other places. I will continue to update and add more links!

- [Web-Design](#web-design)
- [Machine-Learning](#machine-learning)
- [Software-Companies](#software-companies)

## Web-Design
**Sept 11, 2018** [A comparison between Angular and React and their core languages](https://medium.freecodecamp.org/a-comparison-between-angular-and-react-and-their-core-languages-9de52f485a76). This is a good summary for Angular and React comparison. Both technologies are very popular now. React is released earlier and there has gained more popularity. Angular is also growing and has strong supporter like Google. React's virtual DOM gives the advantage of better performance, while Angular is based on TypeScript which is statically-typed and has higher readability and is easier to maintain.

**Sept 1, 2018** [What’s Server Side Rendering and do I need it?](https://medium.com/@baphemot/whats-server-side-rendering-and-do-i-need-it-cb42dc059b38) Server-side rendering has become more and more popular as it tackles a few common issues happen when rendering on client-side. First, rendering can take long time if the internet connection is slow or if the device is old. Also, most search engines do not render a site before indexing it. The easiest way to do server-side rendering is to use ```renderToString```
provided by ```react-dom``` package, and then set up the server to first render the site as an string, before serving it to the client. In the practice, developer can choose popular framework such as *next.js* or *Gatsby.js*.

**May 3, 2018** [Building your startup with Python, React, React Native and AWS](https://medium.com/proximistyle/building-your-startup-with-python-react-react-native-and-aws-286afd94a29c) This article briefly introduces the tech stack the author used to build her startup. The combination of React and Python back-end is what I am going to use in my small project at work. Because I am going to use internal data of my company, I am not going to use commercial server provide like AWS, but it is interesting to learn about the basic structure of AWS, S3 buckets, and AWS lambda.

## Machine-Learning
**Jan 15, 2019** [Looking Back at Google’s Research Efforts in 2018](https://ai.googleblog.com/2019/01/looking-back-at-googles-research.html) by Google AI. A highlight of Google research team's works on various area.

**Jan 15, 2019** [AutoML: Automating the design of machine learning models for autonomous driving](https://medium.com/waymo/automl-automating-the-design-of-machine-learning-models-for-autonomous-driving-141a5583ec2a) by Waymo. This article is a good summary of challenges for self-driving car's machine learning technology and how Google AI's AutoML can help. For self-driving cars, the goal of machine learning is to achieve (1) high quality and (2) low latency. Higher quality implies more safe drives, while low latency is required because mostly self-driving cars are expected to react in real-time. In practice, the existing neural nets show trade-offs between quality and latency. Waymo researchers cooperated with Google AI to use AutoML algorithm to search through thousands of neural cells, and found the best ones which improve their CNN performance for identifying object, detection and localization of traffic lanes. They went further to use AutoML to explore more architectures, instead of just cells. Exploring new architectures is expected to be very computation-heavy, so Waymo's team carefully designed a proxy task to reduce the runtime of evaluating an architecture. One of the result neural net is able to improve latency by 20%-30%.

**Oct 24, 2018:** [Curiosity and Procrastination](https://ai.googleblog.com/2018/10/curiosity-and-procrastination-in.html) by Google AI. This article briefly introduced Google AI's work on curiosity-driven exploration, where while continuing on predicting the future, the agent tends to be "curious" and rewards "surprise," which means when the agent sees something different from their prediction, it tends to go further and explore it. This is very helpful when working on task such as escaping from a maze. One side-effect is "procrastination," where the agent at the same time tends to be attracted by randomly changing object. I really like the example of a TV randomly switching channels. Even if the there is only small number of channels, the randomness will mostly cause surprise to the agent and attract it away from exploring the other parts of world. This effect can pretty much be seen in real world, on each of us human!


## Software-Companies
**Jan 05, 2019** [44 enterprise startups to bet your career on in 2019](https://www.businessinsider.com/44-enterprise-startups-to-bet-your-career-on-in-2019-2018-12). It is always lots of fun to know what (cool) things other people are doing. In this article, a large portion of the "hot" companies are working on network security and devOp. It is impressive to see how valuable it is to invest time and work on technology to make other companies better in terms of safety, efficiency, and scalability.

**Dec 03, 2018:** [An exclusive look inside Google’s in-house incubator Area 120](https://www.fastcompany.com/90262791/an-exclusive-look-inside-googles-in-house-incubator-area-120). Google had been having well-known cultural code of encouraging employees to "spend 20% of time a week to work on new things not related to their daily job." However as the company expanding and employees are devoting 100% of time on their routine engineering works, the idea of 20% time has become "120% time."
This is why Google created "Area 120," an Google internal incubator where employees can leave their original job to start fully engaged in new projects they come up with, after they pitch to Area 120 staff and get green-light. I especially love this idea, because I have heard about how difficult and frustrating the process is for a general startup team to search for seed money. With Area 120, the person you pitch to is your fellow Googlers and it is easier for them to understand your idea. You can even hire other smart Google engineers to work together in the incubator. And finally, it is just easy to get bored working on day-to-day job. Why not brainstorm with friends in the same company for new idea, and spend 100% to achieve it? (although it's named Area 120, you don't really need to spend 120% of time a week:) )

**Nov 30, 2018:** [An Inside Look at Reddit's Video Infrastructure](https://www.linkedin.com/pulse/inside-look-reddits-video-infrastructure-chris-slowe/) by Chris Slowe, CTO of Reddit. It is interesting to see the idea of temporary and permanent buckets, and how Reddit uses them to handle large amount of video uploads and prevent from failed upload to mess up their database. Once videos moved to permanent buckets, transcoding task will then started by AWS Lambda. 


