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
Recently  I've been auditing a Harvard course by [Raj Chetty](http://www.rajchetty.com/), "Using Big Data to Solve Economic and Social Problems", freely available [here](https://opportunityinsights.org/course/).

It's given me a lot to think about, both in the content of the lectures as well as how Chetty organizes the course and delivers the material.

### Motivation

It's the kind of economics class I think everyone should start with, and addresses the biggest complaint on the subject I have heard from new students to former econ majors like myself: too much theory and not enough impact on or connection to the real world. Chetty jumps straight into the impact and motivates learning the methods and theory of the course by offering them as tools to solve the biggest problems of our time: economic inequality and mobility, climate change, health, and so on. 

Hooking students with the fun part first reminds me of [Hadley's](http://hadley.nz/) and [Garret Grolemund's](https://rstudio.com/speakers/garrett-grolemund/) approach to teaching [data science](https://r4ds.had.co.nz/). They start with data exploration (`ggplot2`) first, jumping right into visualization to pique students' interest and build up motivation for the course. [David Robinson](http://varianceexplained.org/about/) summarizes the merits of this approach in [this great piece](http://varianceexplained.org/r/teach-tidyverse/).

### Big data
When I first started the course, I was unsure about Chetty's use of the "big data" buzzword. In industry it's often more of a marketing term than anything substantive. But his use of the term is instructive. He explains how the advent of digitized broad datasets have enabled researchers to ask questions in new ways. In particular, I appreciate the way he . 

Chetty focuses on how big data provide two benefits: 

1. high precision due to large sample sizes 
2. ability to zoom into subgroups-specific effects and interaction effects

Given that most of the data in the course is observational, the course also gently introduces causal inference. Rather than provide an introduction to the field as a whole, the course proceeds method by method (e.g., regression discontinuity, instrumental variables), focusing on application, intuition, and results rather than implementation details. The implementation details are absolutely important, but grounding them in makes the process of learning the drier material much more palatable. 

On the larger point of correlation vs. causation, Chetty takes the student through the researcher's thought process in building a body of evidence, of identifying important factors that may contribute to your outcome of interest, and then designing additional experiments or quasi-experiments to identify their effects. This was a refreshing take on the traditional "correlation ≠ causation" that often leaves students confused about how to move forward. 

### What's coming

As I'm going through the course, I'll be creating a [gitbook here](https://seamus-mckinsey.github.io/data_solve_econ_social_problems/) with my notes from lectures and in exploring the data made available by the Opportunity Insights team. I was inspired by this [fantastic gitbook for ISLR](https://beaulucas.github.io/tidy_islr/) with chapter notes and solutions to exercises using the `tidyverse`.

Brief notes on some key things the course has highlighted (I'll expand on these more in the [gitbook](https://seamus-mckinsey.github.io/data_solve_econ_social_problems/) in the next few weeks):
- identification - how to tell if the quantities you're observing in the data actually relate to the phenomena of interest
- intuition for how to use methods for (I see promise for using [list-cols](https://r4ds.had.co.nz/many-models.html) and `purrr` for this )
- we need effects to hold on average (i.e., the error term not correlated), not for everyone
- how to interpret statistically insignificant results (i.e., we don't have the precision or amount of data needed to make a statement, not that there is no effect)

More broadly, I'm going to spend some time thinking about how "big data" and standard econometric techniques relate. To start, I'll be re-reading Hal Varian's article ["Big Data - New Tricks for Econometrics"](https://pubs.aeaweb.org/doi/pdfplus/10.1257/jep.28.2.3).

