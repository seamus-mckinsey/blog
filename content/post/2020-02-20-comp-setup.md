---
title: Computer setup
author: ~
date: '2020-02-20'
slug: comp-setup
categories: []
tags: [setup]
type: ''
subtitle: ''
image: ''
---

After recently setting up a new personal laptop, I figured I'd collect a guide to the data science toolkit setup for the next time I need to set up a machine. But of course I didn't actually do so. 

_Update 5/20/20:_ Well, that time has come [earlier than expected](https://www.linkedin.com/feed/update/urn:li:activity:6668310718225489920/), and I'm now setting up my old work computer as my personal computer (#thanksuber). I figured this time I might as well make a guide for myself while it's fresh in my mind.

## Xcode
Install 
```sh
xcode-select --install
```
## Homebrew
Get Homebrew (https://brew.sh/) installed:

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```
## Tidyverse & friends

Now that blogdown and friends are installed, let's make sure to get hugo since we use the [Beautiful Hugo theme](https://themes.gohugo.io/beautifulhugo/):
```r 
blogdown::install_hugo()
```
## Credits
I was guided by and borrowed content from these excellent guides:
- [Macbook Pro Setup for Data Science at EnvReportBC](https://github.com/bcgov/envreportutils/wiki/Macbook-Pro-Setup-for-Data-Science-at-EnvReportBC)
- 