---
layout: post
title:  "My introduction to Jekyll"
date:   2024-05-23 21:00:00 -0700
---

Seems only fitting that the first post on here should be about the thing used to create the site! Although peripherally aware of Jekyll through various GitHub docs, I hadn't used it myself. All in, it took about 30 minutes to set up.

## What is Jekyll?

When learning a new tool, one of the most important questions I like to get to grips with is: what problem is it solving? Often, this can be surprisingly difficult to pin down. A given piece of software frequently has much more functionality than you need, so it's important to pin down the key reason why it's important *for you*.

*My* challenge was creating a personal website for blogging. I had a reasonable idea of what I wanted the solution to look like:

* I could write in Markdown.
* I could do version control in Git / GitHub
* It should be hackable and extensible (no silly proprietary stuff).
* Could easily deploy generated sites to GitHub.

A quick search for such requirements will quickly surface Jekyll (with Hugo as another alternative). These are 'static site generators'. The core functionality is taking in blog posts in the form of Markdown (or HTML), and blending them with templates and other configurations to make a blog website.

## The setup experience

Sometimes you want to learn how something works. Sometimes, you know that you don't care. For me, this was the latter scenario.

Setting up Jekyll involved:

1. Working out how to reset the password for my Windows Subsystem for Linux (WSL) user, that I'd forgotten🤦‍♂️
2. [Installing Ruby](https://www.ruby-lang.org/en/documentation/installation/)
3. [Installing Jekyll](https://jekyllrb.com/docs/installation/ubuntu/) (along with some pre-requisites like gcc that weren't on my WSL)
4. Following the [instructions on setting up a GitHub pages site with Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll)

Once there, it was just a matter of changing some .markdown files!

## Summary

I envisage that my typical blog will go much more into conceptual understanding. However, I think it's good to reflect that there are certain situations in which this is unnecessary. There are situations where you just want to get something done, and that had been my experience with Jekyll! No need to learn about Ruby today - those gems can be saved for another time.