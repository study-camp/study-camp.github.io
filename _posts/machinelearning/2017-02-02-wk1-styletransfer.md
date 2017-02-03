---
layout: post
title: "DLNDF: Applying Deep Learning "
author: nitya_n
modified:
categories: machinelearning
excerpt:
tags: [deep-learning, nanodegree, dlndf]
image:
  feature: color-flame.png
comments: true
share: true
---

# Accountability: Progress Report (Wed, Feb 1)

> **TL;DR**
> 
> I am a lifelong learner and autodidact currently invested in growing my understanding of machine learning and deep learning. So I enrolled in the Udacity Deep Learning Nanodegree Foundations, a 17-week curriculum that covers key topics and concepts. I'm using these posts to keep myself accountable by sharing my progress and goals for each week.
> 
> [_You can read the longer version here_](http://study.camp/machinelearning/deep-learning-nd/)



### Goals

My goals were simple
 
  * Setup the software and environment required
  * Finish watching at least 1 of the 9 lessons 
  * Complete any related tasks identified in the lesson

### Progress

  * Completed 2 lessons (_Welcome_ and _Applying Deep Learning_)
  * Started reviewing 2 more (_Anaconda_ and _Jupyter_). I have used these tools before before so installation/setup time was saved. However, I plan to watch these today. I tend to learn things through usage (and not by reading manuals) - so these kind of refreshers are really useful in filling in the gaps in my knowledge or understanding. 
  * I also find it super useful to take Markdown notes on resources and concepts shared in the lessons. I may never actually go back and read those notes -- but the act of writing them down helps me crystallize and consume ideas better. It also seems to help my recall of those ideas.

### Applying Deep Learning

A perfect start to the program, introducing three projects that illustrate the use of deep learning in different domains (art, autonomous vehicles, gaming). 

Because all three projects have open source resources, you have the opportunity to get an applied understanding of concepts by playing with the code and parameters.

<a href="https://github.com/lengstrom/fast-style-transfer" class="btn">Project 1: Style Transfer</a>

This highlights the ability to use neural networks to _learn_ the signature painting or drawing style of an artist, and them _apply_ it to an image, effectively _transferring the style_ of the artist to the new medium.

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Perfect timing too. Exploring Deep Learning foundations <a href="https://twitter.com/udacity">@udacity</a>. Played with style transfer (with curious 8yo here)<br><br>I did one. He did one. <a href="https://t.co/XeV4kuKTXi">pic.twitter.com/XeV4kuKTXi</a></p>&mdash; Nitya Narasimhan (@nitya) <a href="https://twitter.com/nitya/status/826986532946980869">February 2, 2017</a></blockquote>

In this section we simply used pre-trained models (checkpoint files for six popular artworks) with our own images, thereby validating that our setup works. I am looking forward to revisiting this later (once I understand the inner workings) to create my own training models using artwork from India.


<a href="http://selfdrivingcars.mit.edu/deeptrafficjs/" class="btn">Project 2: Deep Traffic</a>

<figure>
    <a href="http://selfdrivingcars.mit.edu/deeptrafficjs/" class="image-popup"><img src="/images/dlndf/deeptraffic.png" alt="image"></a>
    <figcaption>
        <a href="http://selfdrivingcars.mit.edu/deeptraffic/" title="Deep Traffic: A gamified simulation of typical highway traffic">Deep Traffic: A gamified simulation of typical highway traffic
        </a>
    </figcaption>
</figure>

The focus here is on understanding how neural networks can assist in domains like autonomous driving by _learning to navigate in high-traffic roads_. And it serves as a nice sandbox to illustrate [_reinforcement learning_](https://en.wikipedia.org/wiki/Reinforcement_learning), where the network tries to take decisions that maximize a desired reward or outcome.

The simulator allows you to take control of one of the cars and build a neural agent that makes a single decision: "should the car accelerate, slow down or change lanes". 

It has a built-in safety system that takes care of driving and prevents crashes; in other words, it will follow the decisions of your neural network _if_ it can do so without crashing into another car.

The efficiency of your algorithm or training is thus based on how _fast_ you can get your car to move in that traffic.


<a href="https://github.com/yenchenlin/DeepLearningFlappyBird" class="btn">Project 3: Flappy Bird</a>

A perfect illustration of a deep learning agent that automatically _discovers_ the rules of the game by playing the game multiple times, finding out how it scored on each try, then using _reinforcement learning_ to prioritize moves that provided the best rewards. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/THhUXIhjkCM" frameborder="0" allowfullscreen></iframe>

I am not yet at the level where I can appreciate the details, but I hope to revisit the [report](http://cs229.stanford.edu/proj2015/362_report.pdf) later to get a better understanding of how decisions were made. 

### Takeway

My key takeaway is to think consciously about how deep learning could be applied to various applications or activities that I encounter or engage in on a regular basis. 

In particular, for each of these, I hope to identify:
 * What are the inputs (sensors/data) available to the neural network
 * What are desirable outcomes (quantifiable parameters) to use as rewards
 * What are the tradeoffs (resources vs. accuracy?) we need to study



### Next Goals:

_Finish reviewing Anaconda and Jupyter lessons. Start watching the lessons on Regression_
