---
layout: project
title: Bijoux Breakdown
description: "A sketchbook-style board for pricing handmade jewelry, without touching a formula."
order: 3
github_url: https://github.com/meghan-tobin/BijouxBreakdown
website_url: https://bijouxbreakdown.com/
demo_url:
graphic: /assets/images/earrings2.png
demo_video: /assets/videos/bijoux.mp4
docs:
    - title: README
      url: https://raw.githubusercontent.com/meghan-tobin/BijouxBreakdown/refs/heads/main/README.md
---

## The Idea

Designing a jewelry collection means constantly juggling material costs, time, and pricing — and for me, that meant a lot of notebook sketches that got erased the moment plans changed. Spreadsheets were too rigid and too much work to set up, and I kept wishing for something in between: visual like a sketchbook, but smart enough to handle the math automatically.

## Thinking through the Problem

I started by sketching how the tool should feel. The sketchbook aesthetic is intentional; it's meant to feel like the notebook it replaces, with a page that grows longer as you use it.

The key insight was separating **supplies** from **items**. You define your materials once — name, cost, quantity, and unit — in a supply configuration, and every item you price pulls from it automatically. Different pieces have different needs, so you can keep several configurations, like one for earrings and another for necklaces. Logging in is only needed to save your work, so anyone can start sketching right away.

## What I Built

BijouxBreakdown is a drag-and-drop board where you define material configurations, log time costs, and track selling prices — without touching a formula. Each item you create lands on your board showing its total production cost; you can open it for details, resize it, drag it around, and group related pieces together. The backend is written in Rust with Axum, with an HTML, CSS, and JavaScript frontend.

## Next Steps

_Add what you'd like to build next._
