---
layout: post
title: creating my first full-stack web application
date: 2023-04-27 16:40:16
description: building a web-app to rank colleges
tags: projects
categories: projects
---

I've always been passionate about technology and education. I recently decided to channel this passion into creating a web application called [collegeshunt.com](https://collegeshunt.com), which aims to help folks find the most prestigious colleges based on their preferences.

## My thoughts on prestige

In my perspective, the concept of prestige in higher education should be approached with a balanced mindset that acknowledges its importance while remaining grounded in reality. Prestige is undeniably intertwined with academic reputation, alumni networks, and the overall educational experience, yet it remains a multifaceted and often subjective notion. As an advocate for well-rounded decision-making, I believe prestige can provide valuable insights but should not overshadow other crucial factors such as personal values, academic interests, and individual aspirations.

## The Idea

The idea was born from [prestigehunt.com](https://prestigehunt.com), a website that ranks companies by prestige. In fact, I ripped off most of their front-end.

This could also be applied to institutions of higher education, as traditional rankings often don't provide the complete picture, and there's a need for a more dynamic and community-driven platform. With this website, users can contribute to the rankings by participating in head-to-head (H2H) prestige matches, creating a more accurate and constantly evolving list of top colleges. Plus, I think it would be funny to see the results.

## The Tech Stack

I built a single-page application using React for the front-end and Firebase for the back-end. React's component-based architecture and Firebase's real-time database capabilities made it an excellent choice for creating a responsive and interactive user experience.

## Challenges and Solutions

One of the main challenges I encountered during development was that I did not know much about web development. I knew almost nothing about React, Node.js, and databases. I had to figure out how to build this damn thing in the shortest time possible. Conveniently, I generally knew from the front-end what was required of the back-end. The challenge was to figure out how to properly structure the back-end code to fulfill the requests of the front-end client.

To overcome these challenges, I used [ChatGPT](https://chat.openai.com/) and [Github Copilot](https://github.com/features/copilot). It saved me a TON of time. Since I knew how the backend should generally behave (and it wasn't super complicated), they got about 90 percent of the code correct. Being a complete noob, I also wasn't aware that Firestore had a limit of 500 actions (read, write, or delete operations) per transaction. This limitation posed a challenge when scaling my application to handle hundreds of head-to-head matches. It required me to use batched writes instead.

## Final Thoughts

Building this website has been an incredibly rewarding experience, as I've learned a lot about React, Firebase, and ChatGPT prompting. Finally, don't take the rankings too seriously.
