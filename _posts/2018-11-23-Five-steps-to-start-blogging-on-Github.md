---
layout: post
title: Five Steps to Start Blogging on Github
categories: [blog]
---

Welcome to my first blog! As the starting point of work blog, I am going to demostrate how I actually started this blog, which is itself as easy as 5 steps!

There are two reasons for me to come across this idea of writing blogs about my works. First, it helps me memorize the result I spent a lot of time and try-and-error to get, which can also help other people save their time. Second, I recently worked with my wife, Anne, to refresh the look of her blog site on [Pixnet](http://anne0313.pixnet.net/blog), which motivated me to find a blog platform easier to use.

Pixnet is one of the most popular blog platform that Taiwanese bloggers use. It is easy for the bloggers to write posts, get statistics, and manage ads and followers. The downside of Pixnet is that, even though it allows blogger to choose theme or even write custom CSS, the layout is still restricted by the fixed [html structure](http://pic.pimg.tw/pixnetvisual/1187010393.gif). After we finished updating the CSS for Anne's Pixnet blog, I decided to search for a more flexible platform for my own blog. Altough there are a lot of applications which offer this capability, I would rather make the step of writing blog even more simple. What is the simplest way for me to write a blog? When asking myself, the answer is to edit a text file and commit to Git!

This is where I started to look into Github pages. The first thing I learned is Github pages are deeply integrated with [Jekyll](https://jekyllrb.com/). I spent some time reading through [Github's doc](https://help.github.com/articles/using-jekyll-as-a-static-site-generator-with-github-pages/) and the Jekyll docs, but wasn't clear enough. I turned to use the engineers' favorite approach -- copying the template and modifying. So here are the 5 steps for you to start your own blog:

```
1. Create a repo with Github pages enabled:
To enable the pages, go to the settings of the repo and scroll to **GitHub Pages**, and then choose a theme. Github will automatically build the pages using Jekyll. All you get here is a \_config.yml file.

2. To make things simple, I changed the theme to [minima](https://github.com/jekyll/minima):
minima is the default theme of Jekyll. This is done by overwrite your \_config.yml file with [the one from minima](https://github.com/jekyll/minima/blob/master/_config.yml). Below line changes the theme:
 theme: minima

3. Creat index page with markdown.
To do this, simply copy the [index.md file](https://github.com/jekyll/minima/blob/master/index.md) to your repo. You might notice that this is just setting the layout to **post**. The actual layout is determined by the theme minima.

4. Write your first post.
Create a sub-dir named \_posts. In the \_posts directory, create your first post with the format YYYY-MM-DD-Your-Title.md.

5. Commit and push to Github.
There you go. The pages will be automatically built, and you will get a site looks exactly like [this](https://jekyll.github.io/minima/)
```

I have just started to learn front-end development, but with Github pages, I can also start to write blogs at the same time. If you read through this point, you are probably also a beginner like me, and I hope you find this post helpful! 