---
layout: project
title: Wikipedia Automator
description: "Finds the shortest hyperlink path between any two Wikipedia articles: the Wikipedia Game, automated."
order: 4
github_url: https://github.com/meghan-tobin/Wikipedia-Automater
website_url: https://wikiautomator.dev/
demo_url:
graphic: /assets/images/wiki.png
graphic_dark: /assets/images/new-wiki.png
demo_video: /assets/videos/wikidemo.mp4
docs:
    - title: README
      url: https://raw.githubusercontent.com/meghan-tobin/Wikipedia-Automater/refs/heads/main/README.md
---

## The Idea

This is a revamped project from my Data Structures course in college. Around that time I'd been watching people play the Wikipedia Game — the challenge of navigating from one Wikipedia article to another in as few hyperlink clicks as possible. Could I automate it?

## Thinking through the Problem

The assignment was to work with a directed graph dataset of our choosing and implement graph traversal algorithms to explore it. Wikipedia's hyperlinks are a natural fit: every article is a node and every link is a one-way edge.

I used the Stanford SNAP wiki-topcats dataset — 1.79 million articles and 25.4 million links. Breadth-First Search was the right tool for shortest paths, since it explores by hop count, so the first time it reaches the destination is guaranteed to be the shortest route. PageRank added a second angle: ranking articles by connectivity to see which ones act as "hubs." The dataset came with real constraints too — links only go one way, it's a snapshot from around 2011, and it only includes articles with 100+ inbound links.

## What I Built

I implemented BFS, DFS, and PageRank in C++. The program loads the whole graph into memory once (about 45 seconds), after which BFS finds a path in milliseconds. The original submission was command-line only, so I recently built a frontend to better showcase it: a FastAPI server keeps the C++ graph loaded, and the site animates the path between articles as it's discovered and lets you compare how each algorithm explores the graph differently.

## Next Steps

_Add what you'd like to build next._
