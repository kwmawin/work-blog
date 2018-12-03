---
layout: post
title: Test Your Blog Pages Locally
categories: [blog]
---
In this blog, I will show how to test the blog pages locally, so we can take a look of what our post looks like before we publish it.

In the [Last post](https://kwmawin.github.io/work-blog/blog/2018/11/23/Five-steps-to-start-blogging-on-Github.html), I demonstrated how to create a blog with Minima theme. After you wrote some content, you may want to start to look into how to change the style of your blog, and it is better if we can take a look at our pages locally.

Since we are writing post using Github pages built by Jekyll, we need to have Jekyll available locally. To me this was the boring part where I had to follow the install instruction, but also spent much more time debugging why some steps were not working. It depends on the system and OS version you use, but basically, [these](https://jekyllrb.com/docs/installation/macos) are the steps you need to follow.

At this point you should have the `jekyll` command available in your terminal. Next, clone the repository of your blog to your machine, and then cd into the repository root directory. You can now run `jekyll serve` which builds your site and starts a local server, and then open [http://localhost:4000](http://localhost:4000) in your browser to see your site locally. 

Now you can start to change the look of your page layout. One thing you (and so did I) might wonder is that, how do we actually change it, when we are using the Minima style with `theme: minima`? The answer if surprisingly simple: just copy the file to your repository and change there! 

So here is what I did. I found the "subscribe via RSS" link not useful at this moment, so I create a local file `_layouts/home.html`, and removed the `<p class="feed-subscribe">` line. The I verified the change with `jekyll serve` and go to the local page to make suer the line is gone.

You should now be able to play around with the page layout and style, and take a look on your machine. Keep in mind that many of the changes you want to do to make your site look fancier might be easily achievable with Markdown syntax and Jekyll features. Check out [Jekyll docs](https://jekyllrb.com/docs/) to get some ideas. Enjoy!