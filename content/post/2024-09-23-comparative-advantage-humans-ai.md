---
title: Comparative advantage of humans and AI
author: ~
date: '2024-09-23'
slug: comparative-advantage-humans-ai
categories: [AI, Economics]
tags: [AI, Economics, Comparative Advantage, Chess]
type: ''
subtitle: ''
image: ''
---

# Comparative Advantage of Humans and AI

Recently I've been working more with AI tools at work, primarly [Cursor](https://cursor.com/). It's been extremely useful in automating the lower value parts of the analytics engineering workflow: writing config for data models (dbt yml files) and writing basic documentation in markdown (drawing from comments and logic in the SQL files). It's also good enough to suggest adding basic tests, like standard `unique` and `not_null` dbt tests.

AI tools have made more productive. They've also raised a question that keeps nagging at me: if I extrapolate this out 5-10 years, what's left for humans to do? AI will move from the lower value to higher value tasks. Perhaps there's some ceiling they'll hit where humans will remain . But there's concept in economics that offers a more nuanced—and perhaps surprising—perspective: comparative advantage.

## What is Comparative Advantage?

Comparative advantage is one of those counterintuitive ideas from economics that feels wrong at first but becomes profound once it clicks. Paul Samuelson, founder of modern economics, once said "thousands of important and intelligent men have never been able to grasp the doctrine for themselves or to believe it after it was explained to them." The core insight: **two parties can benefit from specialization and trade even when one party is absolutely better at everything.**

Here's a classic example to build intuition. Imagine a lawyer who types 120 words per minute, while their paralegal types 80 words per minute. The lawyer is better at typing! Should they therefore do their own typing?

No—because of opportunity cost. While the lawyer spends an hour typing up documents, they're not spending that hour on legal work that might bill at $500/hour. The paralegal's time might be worth $50/hour. Even though the lawyer is better at both legal work *and* typing, they should specialize in legal work (where they have the greatest advantage) and let the paralegal handle the typing.

Another way to think about it: Country A can produce both cars and wine more efficiently than Country B. But Country A is 10x more efficient at making cars and only 2x more efficient at making wine. Country A should specialize in cars (where its advantage is greatest), and Country B should specialize in wine (where its disadvantage is smallest). Both countries end up better off through trade.

The key insight: **it's about relative advantage, not absolute advantage.**

## How Comparative Advantage Works with AI

Now let's apply this to AI. Suppose AI eventually becomes better than humans at most cognitive tasks—better at writing, better at data analysis, better at programming, better at research. Does this mean humans become economically obsolete?

Not necessarily, if we think through the logic of comparative advantage.

Even if AI is better than me at *everything*, there will still be tasks where the gap is smaller. If AI is 10x better than me at data cleaning but only 2x better than me at interpreting results in domain context, then it makes sense for the AI to focus on data cleaning and for me to focus on interpretation.

Why? Because the AI's time is valuable. Every hour the AI spends on interpretation (where it's only 2x better than me) is an hour it's not spending on data cleaning (where it's 10x better than me). From a productivity standpoint, we're better off if the AI focuses on tasks where its advantage is greatest.

**Important caveat**: This logic assumes AI resources are scarce—that there's a meaningful opportunity cost to how AI spends its time. If AI becomes infinitely abundant and cheap, this logic breaks down. More on this later.

## Implications and Open Questions

The optimistic interpretation of comparative advantage goes like this: there's always *something* for humans to do, even if AI is better at everything. As AI gets better at task X, humans shift to task Y. The market ensures demand for human labor because we'll always have comparative advantage somewhere.

This is genuinely true in the economic model—comparative advantage is powerful and robust.

But I have several concerns:

**Adjustment costs are real.** The theory says humans will shift to new areas of comparative advantage, but it doesn't say this will be smooth or painless. Retraining takes time. Not everyone can easily transition from data cleaning to nuanced interpretation. The chess analogy is sobering: there's a long period where humans had comparative advantage in chess teaching, commentary, and certain styles of play—but far fewer people make a living from chess than when humans were the best players.

**What if improvement is too fast?** Comparative advantage assumes we can find the new equilibrium. But if AI capabilities are improving faster than humans can retrain and adapt, we might face persistent unemployment or underemployment, even if there theoretically exists some task we have comparative advantage in.

**The abundance question.** Comparative advantage fundamentally relies on scarcity—on opportunity costs mattering. If AI becomes so cheap and abundant that there's no meaningful cost to having it do everything, why would anyone pay for the "slower, worse" human version, even in areas of human comparative advantage?

This is like asking: even though I have comparative advantage over a lawyer in painting houses, will they hire me when robot painters are $1/hour?

**Preference for human interaction.** One potential answer: maybe people will simply *prefer* human services in certain domains, even if AI is technically better. We might want human doctors, teachers, therapists, or coaches for social and emotional reasons that go beyond pure capability. This is less about comparative advantage and more about product differentiation, but it might preserve roles for humans.

## Further Reading

Some resources I've found helpful in thinking through these questions:

- **David Autor's work on automation and labor markets**: Especially [Why Are There Still So Many Jobs?](https://economics.mit.edu/sites/default/files/inline-files/Why%20Are%20there%20Still%20So%20Many%20Jobs_0.pdf) and work on task-based models of labor
- **Kasparov on advanced chess**: His writings on chess and AI collaboration. [Here's](https://news.northeastern.edu/2024/06/17/garry-kasparov-chess-humans-ai/) a recent relevant article.

This is very much a work-in-progress exploration. I'd love to hear from others thinking about these questions.
