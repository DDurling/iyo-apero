---
title: Building this website
author: Daniel Durling
date: '2021-08-10'
layout: single-sidebar
draft: false
summary: "How I built this website, and the workshops / blogposts that helped me."
slug: []
categories: 
- R
- Website
tags: 
- personal
---

## How I made this website

> good artists borrow, great artists steal - _Picasso_
 
This feels like a good excuse to use the above quote. I built this website by following the work of others, and only when I ran into issues did I have to do anything original. So if you wish to build a website using blogdown (and if you use R you should!) then I would recommend reading this two day[introduce yourself online workshop](https://iyo-rstudio-global.netlify.app/collection/). This two day workshop was run by [Alison HIll](https://alison.rbind.io/) and there is a [YouTube Video](https://www.youtube.com/watch?v=RksaNh5Ywbo&list=WL&index=10&t=1s) of it too (although I did not watch it I just followed the site).

If you are interested in why you should have a website check out this [Ali Abdaal video on making a website](https://www.youtube.com/watch?v=acBJsjCqgtM).

## Following the course

So I went through each of the sections on the above linked site, and there wasn't really much more to it! I will make another post in a months or two's time to see if I have learnt anything else, but everything you need to get going is there for you. 

### Pre day

I did all of my work on my laptop rather than on RStudio Cloud. The [markdown site](https://commonmark.org/) was a useful refresh on some bits of markdown.

### Day 1

Day 1 sets the scene for having a place to call your own online, in fact if you are not wedded to using blogdown this might be enough for you. For me I found the way of having a readme.md file for my GitHub profile really useful and not something I think I would have found on my own.

Even though I wasn't going to use the postcards and distill pages they go over in Day 1, it made me dust off my GitHub and get used to using my current laptop so I still found it really useful and I wouldn't skip it.

### Day 2

This is where things start ramping up, and where I nearly fell at the first hurdle, I could not see the "deploy to netlify" button :| (I know I know...) but after I found it (it is right at the top under the first heading in the README.md).

After that _slight_ issue then everything worked fine. I had already signed up to netlify and so everything really did "just work" and I had my own copy of the repo stored under my GitHub page and every time I pushed a change it reflected on my website! Every commit was a moment of joy (except when I broke the talks page (see below)).

At this point it was just a matter of going through the code and following the suggestions on the site, and slowly making small changes to make the site look like how I wanted.

## Issues I encountered

### Layout

So I could reference all the example posts but them not be seen on my blog I marked them all as `draft: true` in the YAML header of each post.

I also managed to break the "talks" section which comes as standard (at some point the website would not deploy). I think need to look into why / how that happened but in the short term I have decided to just remove it for now.

If you add a `summary: ` into the YAML section of a post. that summary is the text that appears on the "Blog" page. I think this is worth adding to every blog post.

### buying a domain & setting it up

Once I had deployed to netlify as the guide suggested and had played around with some of the options I knew I wanted my own domain so I bought [This site](https://danieldurling.com) from [Google domains](https://domains.google.com/).

Then I headed back to netlify to add in a custom URL. Once I added it I needed to add in some netlify DNS to my google domain to stop there being a security warning when I accessed my website. In order to do that I followed this [guide](https://dev.to/lost_semicolon/netlify-and-google-domains-hm3).

### Getting rid of stock pictures

When I my [website](https://www.danieldurling.com/) an image will also appear in social media. However the images associated with each page wasn't what I wanted. I found that the main page was displaying an image in the static/img folder called arbre.jpg, and other pages were displaying other images from that folder. 

As I couldn't see anywhere that referenced arbre.jpg I simply replaced it with an image I wanted with the same name (I know it isn't ideal but...) which fixed it for some pages but not others.

I then realised that in the config.toml file there was a "sharing_image" defined, which edited to be the image I have on my home page.

Finally I had to wait for some caching to catch up with my changes (I was doing lots of my testing in telegram and they have a dedicated bot for clearing that sort of thing [here](https://t.me/WebpageBot). 

## Still to do

 - Fix talks section
 - Dig into YAML options (Think I will add a draft: true as default so I can work on posts before deploying)
 - Decide on if I want to use .md, .markdown, .Rmd or .Rmarkdown as default (and what the advantages are if... if any)
 - move / rename repo on GitHub (so it is obvious which one is for my website)
 - add the contact form back in
 = what other options() do I want to add to the .Rprofile?
 - remember to use slugs to lock down the URL even if the title of the post changes
 
