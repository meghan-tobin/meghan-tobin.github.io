---
layout: project
title: Where's the Whimsy
description: Making your life more whimsical one quest at a time....
order: 1
github_url: https://github.com/meghan-tobin/WheresTheWhimsy
demo_video: /assets/videos/whimsy-demo.mp4
mockups:
  - image: /assets/images/whimsy-open-screen2.jpeg
    caption: Opening page
  - image: /assets/images/whimsy-home-page2.jpeg
    caption: Home page
  - image: /assets/images/whimsy-quest-view2.jpeg
    caption: Quest view
  - image: /assets/images/whimsy-create-quest2.jpeg
    caption: Create a quest
  - image: /assets/images/whimsy-explore-page2.jpeg
    caption: Explore page
graphic: /assets/images/whimsey.png
docs:
    - title: README
      url: https://raw.githubusercontent.com/meghan-tobin/WheresTheWhimsy/refs/heads/main/README.md
---

## The Idea

The inspiration for this project came from living with a roommate who struggled to get outside of her comfort zone and experience new activities. I think this is something we all struggle with after college: life can become mundane, and we fall into a structured routine with little time for anything else. Maybe weekends are fun, but how often are we trying a new activity or starting a new experience?

After a few months of living with my roommate, all I could think was, **"where's the whimsy?"** She had a very structured lifestyle, so it got me thinking: is there a structured way to introduce new things? Could she enjoy life more if something helped her move past her comfort zone in a structured way?

The more I thought about it, the more I realized I'd benefit from something like that too. A way to add something new to your week.

## Thinking through the Problem

Trying something new is easier when it feels small, structured, and low-pressure. That idea became the foundation of Where's the Whimsy: a social app built around weekly **quests** — small challenges like grabbing your coffee somewhere new, cooking something you've never made, or checking out an event in your city. A quest can be anything!

I wanted to create a way for people to step outside their routines, discover new experiences, and connect with others without the pressure of putting themselves out there.

### Market Research

Before writing code, I explored existing apps to understand how they approached social discovery, group activities, and meeting new people.

- **Sidequest** was one of the closest concepts to what I had in mind, but was not widley used and was focused on an activity rating system.
- **Bumble BFF** and **222** offered ways to meet new people, but I wanted to explore a lower-pressure alternative for people who might find traditional social settings intimidating.
- **Partiful** inspired some of the app's layout and event-discovery experience, but discovering activities there often depends on your existing network or finding public events.

I saw an opportunity to bring together the discovery aspect of social apps with small, approachable challenges that people could participate in on their own terms.

### Defining the MVP

I wanted the first version to focus on three things:

1. Making quests easy to create and join
2. Helping users discover quests that interest them
3. Making participation feel low-pressure

**Anonymity was a core product decision.** Social media can make even everyday activities feel performative, and I didn't want that pressure to carry over into Where's the Whimsy. Each user gets a randomly generated username for every quest, allowing them to participate without tying their activity to a persistent public identity.

**Quests should feel like more than a checklist.** I added discussion threads, photo sharing, points for completing quests, and a community vote to crown a champion. These features introduce a sense of community and friendly competition while keeping participation flexible: users can engage as much or as little as they want.

To translate these ideas into a buildable first version, I worked through specifications for the quest lifecycle, categories, the onboarding quiz, and discussion rules, alongside UI wireframes. This helped define the core experience before implementation.

### Mock-ups

These are my original mockups when I started sketching out this idea. I had a friend from college illistrate the opening page!

## What I Built

I've built the core backend API using **Python** and **FastAPI**, with **PostgreSQL** and **PostGIS** for location-based discovery, **Redis** for caching and sessions, and **Cloudflare R2** for media uploads.

The current backend supports:

- **Quest discovery:** a feed filtered by category, location, and popularity
- **Quest creation:** titles, descriptions, categories, and whimsy point values
- **Anonymous participation:** a unique username for each user in each quest
- **Community discussion:** threaded conversations, upvotes, and moderation
- **Friendly competition:** a 30-minute champion-voting window at the end of each quest, with double points for the winner
- **Private quests:** invite links for quests shared with a specific group
- **Personalized onboarding:** a short whimsy quiz that the app uses to recommend quests

## Next Steps

The next phase is turning the backend into a complete, testable product.

1. **Build the iOS app:** develop the client in Swift and SwiftUI, with a full UI and visual design.
2. **Launch a beta:** get Where's the Whimsy into people's hands and observe how they discover, join, and participate in quests.
3. **Learn from users:** gather feedback to understand what's working, where people get stuck, and what would make them return.
4. **Iterate:** use those findings to prioritize improvements and future features.
5. **Strengthen the infrastructure:** add real-time updates, quest recommendations, push notifications, rate limiting, CI/CD, and load testing as the product develops.
