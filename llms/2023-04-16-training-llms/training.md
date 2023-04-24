---
title: "Nuggets from Weights & Biases' white paper on training LLMs"
description: "Gems for the general audience in this otherwise rather
technical paper"
date: "2023-04-16"
categories: ["OpenAI competitors", "Research"]
image: image.png
comments:
 hypothesis: 
   theme: classic
---

Weights & Biases, an ML tools company, just issued [this report](https://drive.google.com/file/d/1MXWIsjCogjDVORge5eYGKXUyOy5J2EnP/view?usp=share_link). 

You might think, given the title and author, this is a dry and
jargon-filled report relevant to practitioners and other experts. And
you would be right.

But there is also some very good, and more generally useful content that
makes it worth a skim, or at least reading the notes I've cribbed from
it, below:

- There's a good section laying out principles for when it makes sense
  to buy a pre-trained LLM (like ChatGPT-4), or use an open source one,
  or build your own. Well written for a general audience and useful for
  any founder or decision-maker trying to figure this out. 

- The section on hardware has a lot more detail than most people need,
  but there are some useful data points in there about just how
  computationally intensive and expensive it is to train these large
  language models. Google's PaLM model, which is very large, is
  estimated to have cost $23 million and taken 64 days to train. 
  
  But I'd call that a very flawed estimate. It is based on the list
  price of using Google Cloud Platform to do the training; no enterprise
  spending real sums actually pays list price (I have no special
  knowledge, but the benchmark for enterprise discounts used to be about
  30%), and Google certainly didn't pay *itself* list price to train
  PaLM; the insider prices are far, far below what they charge
  customers. On top of that, we should ask what the very
  latest-generation GPUs and TPUs would cost to do this work.

- The page and a half on dataset collection and dataset pre-processing
  are also worth a read, because they give people not in the field a
  sense of the high-effort grunt work that goes into training. To train
  models well, you need to not just have a lot of data, but have a lot
  of the *right* data, and that can be hard to collect and then
  laborious to clean and format. 

- The section on reinforcement learning through human feedback is a bit
  drier than the above, but will give you a good idea of how OpenAI is
  using people (controversially, in call centers in Ethiopia I believe)
  to improve ChatGPT.

