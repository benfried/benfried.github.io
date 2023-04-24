---
title: "Bloomberg gets into the LLM game"
description: "Bloomberg's research group shows us what you can do 
  with high-quality training data"
date: "2023-04-05"
categories: ["Finance", "OpenAI competitors", "Research"]
image: image.png
comments:
 hypothesis: 
   theme: classic
---

I found [this paper](https://paperswithcode.com/paper/bloomberggpt-a-large-language-model-for)
yesterday, from the AI research group at Bloomberg.

It has substantial technical depth, but the takeaways are clear from the
abstract.

- Bloomberg trained a 50 billion parameter LLM on a combination of
  proprietary financial data (they probably have more / better financial
  data than anyone in the world) and general information. 

- It outperforms specific models at a number of finance-related tasks
  while still being useful for general tasks. 

The financial tasks are specific and rather narrow (not, say, stock
market predictions). Things like sentiment analysis of news articles for
finance-related purposes, finding known entities (people, companies,
etc) in a document, or determining whether a given topic is in an
article. Those tasks may not be as exciting as predicting the S&P would
be, but they are all important tasks people in finance use ML for today,
and these results are impressive.

Unlike anything we've heard from OpenAI recently, the Bloomberg paper
goes into great depth into the architecture of the model and how it was
trained. Of course since so much of their training data is proprietary,
it benefits them to be so comparatively open.

More importantly perhaps is that the article demonstrates some important
aspects of this new era: LLMs performance benefits from high-quality,
curated data sets; that there is extra power in training with a focus on
specific domains or tasks; and that having the resources (quality data,
lots of compute) to train these models is essential. And, finally, it
shows the impact achievable by just a few quite talented experts, if
they have the data and the compute.

### April 18 update

I spoke to Bloomberg's CTO, Shawn Edwards today; they've only gotten
started. There's a *ton* more data they want to add to the training. And
although he wouldn't say it outright, I got the distinct sense that
there was a lot of pride at Bloomberg about just how much more they were
able to publish than OpenAI has. 
