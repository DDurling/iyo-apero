---
title: Router and WiFi setup
author: Daniel Durling
date: '2021-08-24'
slug: router-and-WiFi-setup
layout: single-sidebar
summary: quick .md post on my wifi setup so I can link people to it.
draft: false
categories: []
tags:
  - personal
---

# Purpose of this page

These are just my personal notes on our home WiFi setup, to make it easier to share with people if / when they ask.

## Our WiFi and router setup (Aug 2021)

 - [Our Router](https://www.amazon.co.uk/ASUS-RT-AX82U-Compatible-Lifetime-Internet/dp/B08CBC2WH2) - cheapest WiFi 6 router at the time

 - [Our Modem](https://www.ebay.co.uk/sch/i.html?_from=R40&_trksid=p2047675.m570.l1313&_nkw=+BT+Openreach+Huawei+EchoLife+HG612+3B&_sacat=0) - any 2nd hand  bt openreach huawei echolife hg612 3B will do

 - [Pi hole](https://pi-hole.net/) - I set this up as a DNS sink, so that I do not have to see as many web page adverts

 - [Our ISP](https://www.plus.net/refer.php?strReferralsUid=80e973b8cf006000e110b20a1138532786910c1a5c77943b06375abecdfc8c91) - plusnet

## Why I went for this set up

I wanted to be able to get access to the linestats from the modem, and I also wanted a WiFi 6 capable router. It turns out that the modem & router combo you get when you sign up for plusnet isn't capable of being _just_ a modem, so we needed to replace it with the openreach one. I followed the info on [this](https://kitz.co.uk/) website to set up the modem, then connected the router to the modem. All the info needed for the modem is available in your account page on plus.net.

Also, by separating the modem and the router, it makes it easier to upgrade either part (so if you modem to fibre and need a different modem then you can still use the functionality of your router), or if you want / need a better WiFi router you do not have to reset all your modem settings.  


