---
title: What I Learned from Big Data for Social Problems
author: ~
date: '2020-05-14'
slug: big-data-for-econ-social-problems
categories: []  
tags: []
type: ''
subtitle: ''
image: ''
---
Recently  I've been auditing a Harvard course by [Raj Chetty](http://www.rajchetty.com/), "Using Big Data to Solve Economic and Social Problems."

It's the kind of economics class I think everyone should start with, and addresses the biggest complaint on the subject I hear from new students to econ majors alike: too much theory and not enough impact on or connection to the real world. Chetty jumps straight into the impact and motivates learning the methods and theory of the course by offering them as tools to solve the biggest problems of our time: economic inequality and mobility, climate change, health, and so on. 

Hooking students with the fun part first reminds me of [Hadley's](http://hadley.nz/) and [Garret Grolemund's](https://rstudio.com/speakers/garrett-grolemund/) approach to teaching [data science](https://r4ds.had.co.nz/). They start with data exploration (`ggplot2`) first, jumping right into visualization to pique students' interest and build up motivation for the course. [David Robinson](http://varianceexplained.org/about/) summarizes the merits of this approach in [this great piece](http://varianceexplained.org/r/teach-tidyverse/).

At first, I was hesitant about Chetty's use of the "big data" buzzword. But his use of the term is instructive. He explains how the advent of digitized broad datasets have enabled researchers to ask questions in new ways. The tour of methods is also a gentle introduction to causal inference via quasi-experiments, regression discontinuity, and (I expect though haven't seen yet) instrumental variables.

As I'm going through the course, I'll be creating a [bookdown here](https://seamus-mckinsey.github.io/data_solve_econ_social_problems/) with my notes from lectures and in exploring the data made available by the Opportunity Insights team. I was inspired by this [fantastic gitbook for ISLR](https://beaulucas.github.io/tidy_islr/) with chapter notes and solutions to exercises using the `tidyverse`.

Brief notes on some key things the course has highlighted (I'll expand on these more in the gitbook in the next few weeks):
- identification - how to tell if the quantities you're observing in the data actually relate to the phenomena of interest
- intuition for how to use methods for (I see promise for using [list-cols](https://r4ds.had.co.nz/many-models.html) and `purrr` for this )
- we need effects to hold on average (i.e., the error term not correlated), not for everyone
- how to interpret statistically insignificant results (i.e., we don't have the precision or amount of data needed to make a statement, not that there is no effect)
