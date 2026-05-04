---
title: "Building my Personal LLM Wiki (Part 1): The Motivation"
source: "https://www.rangaprabhu.com/blog/building-my-llm-wiki"
author:
  - "[[Written By Rangaprabhu Parthasarathy]]"
published: 2026-04-08
created: 2026-05-04
description: "Inspired by Karpathy’s post, my ongoing journey in building my own llm wiki."
tags:
  - "clippings"
---
Inspired by Andrej Karpathy’s [post](https://x.com/karpathy/status/2039805659525644595?s=20) and subsequent [LLM Wiki note](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f#llm-wiki), I have built a simple personal LLM Wiki. After building a [sophisticated second brain system at work](https://www.rangaprabhu.com/blog/leveraging-my-second-brain-to-build-a-chief-of-staff-and-secretary), I was looking for a simpler, lightweight solution for my personal stuff. Karpathy’s post was a great starting point: instead of investing in a large repository, start with something small, have the model incrementally build and maintain a persistent wiki that compounds as new sources arrive. In the first of two posts, I will share how I got started and how I approached the exercise. In my second post, I will share the technical underpinnings so you too can build your personal wiki.

![](https://images.squarespace-cdn.com/content/v1/654ef4e2544df93addd091c2/a680ded9-32d3-4a5b-9a93-0031a39da9e9/llmwiki.png?format=2500w)

#### The Motivation

When I read Karpathy’s post, what stuck was that it complements my earlier “ [second brain](https://www.rangaprabhu.com/blog/leveraging-my-second-brain-to-build-a-chief-of-staff-and-secretary) ” thinking rather than replacing it. A second brain works really well as a broad sink. It can pull from email, chat, workplace tools, docs, notes, meetings, and all the messy streams where modern work actually happens. That matters because context is often trapped in those systems. For my personal use, I am less interested in building an all-knowing context machine than in building a personal library that makes connections.

That distinction matters especially given the token costs to build and maintain a high functioning second brain system. My second brain at work is about capture and building context across sophisticated enterprise tools and systems. It helps me save things, synthesize them and leverage it for business outcomes. The personal library helps me develop taste, patterns, and points of view. To help my ideas start talking to each other.

That is what made the LLM Wiki pattern interesting to me. The missing piece in most personal knowledge systems was never storage. It was maintenance. Humans are bad at the quiet work that makes a knowledge base valuable over time: updating pages, adding links, folding new material into old understanding, noticing contradictions, keeping structure intact. Karpathy’s note gets right to that. The wiki becomes the persistent, compounding artifact, and the model does the bookkeeping.

#### The System

So my experiment is pretty simple. I clip things I care about using [Obsidian Web Clipper](https://obsidian.md/help/web-clipper), bring them into Obsidian, and have Claude ingest them into a small personal wiki. Not just archive them. Read them, extract what matters, connect them to existing pages, and slowly build a body of synthesized knowledge. The point is not to create a prettier notes folder. The point is to create a layer between me and the raw material, one that gets more useful as the connections deepen.

That also feels like the natural evolution of my writing workflow starting to help me think. A page is no longer just a note. It can become an outline, an argument, a blog post draft, or a sharper way to answer a question I have been thinking about for months. The system helps me see relationships I would not have maintained by hand. For example, the outline for this particular post was driven out from my personal wiki. I just had to ask.

It is still early. This is a one-day experiment, not a mature system. But the direction feels right. A small, living system that helps ideas compound.

In [the next post](https://www.rangaprabhu.com/blog/building-my-personal-llm-wiki-part-2-the-implementation), I share my technical implementation if you are interested in building your own LLM Wiki.