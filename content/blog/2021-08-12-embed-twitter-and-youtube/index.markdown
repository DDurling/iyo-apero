---
title: "Embed twitter and youtube"
author: "Daniel Durling"
date: '2021-08-12'
slug: embed-twitter-and-youtube
layout: single-sidebar
draft: false
summary: how to embed tweets and youtube videos in your blog posts.
categories: 
- R
- Website
tags: 
- personal
---

# POC on how to emed youtube and twitter

Here is a short example of how to embed a YouTube into your blogdown & Hugo blog.

## YouTube

To embed a YouTube video in an R Markdown document you need to write this:

I will be embedding this [video](https://www.youtube.com/watch?v=vYwXMnC03I4) of Hadley Wickham talking at UCL (which I was lucky enough to attend). 

All you need to do is use Hugo short code and then the video name:

{{\< youtube vYwXMnC03I4 \>}}

(in order to display the above rather than call the shortcode I had to add a `\` before the `<` and then `>` to stop them being special characters.).

Here is what it looks like when we call the shortcode:


{{< youtube vYwXMnC03I4 >}}

In the [blog](http://estebanmoro.org/post/2019-02-01-setting-up-your-blog-with-rstudio-and-blogdown/) I was following it said you needed to use %...% rather than <...> but I found that both worked so I have two copies of the video embedded in my site.

## Twitter

To embed a tweet is very similar, use the same Hugo short code but replace YouTube with tweet. This [tweet](https://twitter.com/hadleywickham/status/1387819502948306944) from Hadley Wickham about his new book on mastering shiny seems like a good candidate:

{{< tweet 1387819502948306944 >}}


There we go! 

The full list of available Hugo short-codes are [here](https://gohugo.io/content-management/shortcodes/) and you can also add your own custom ones too 9I need to look into that, the blog I linked to above has a post on it I think).


