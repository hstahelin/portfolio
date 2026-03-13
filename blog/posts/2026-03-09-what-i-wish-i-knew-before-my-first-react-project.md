---
title: "What I Wish I Knew Before My First React Project"
slug: "what-i-wish-i-knew-before-my-first-react-project"
description: "A candid look at my first React project—misconceptions, time sinks, and the practical lessons I wish I knew before I started."
tags: ["react", "web-development", "bootcamp", "frontend", "javascript"]
reading_time: "5-6 min"
author: "Hugo Stahelin"
date: "2026-03-09"
keywords:
  - react beginner mistakes
  - first react project
  - react lessons learned
  - react state management
  - react components
  - jsx basics
  - react devtools
  - web development bootcamp
  - react tips
  - frontend development
image_references:
  hero: "desk setup with code editor open on React component architecture"
  in_article:
    - "whiteboard sketch of component tree and props flow"
    - "debugging session screenshot style illustration with React DevTools"
    - "before/after UI mock showing ugly-first then polished interface"
---

My first React project was my bootcamp capstone: a support desk app with ticket creation and editing, a knowledge base, user management, and notifications. It sounded like “build a website.” It felt like building a living system. I didn’t realize then that React wasn’t the whole app — it was only the view. The rest of the stack mattered just as much.

The first thing that surprised me was JSX. I expected HTML with a bit of JavaScript sprinkled in. What I got instead was JavaScript that happened to look like HTML. Once that clicked, my mental model changed. JSX wasn’t a markup language — it was a language for composing logic and UI at the same time. That shift took longer than I expected.

The second misconception was bigger: I thought React *was* the app. In reality, React was just the front door. The real complexity lived in the data flow. I was stitching together Express sessions, Passport auth, MySQL persistence, sessionStorage for login state, and then a React UI on top. The UI felt easy compared to making everything work together.

The biggest mistake I made had nothing to do with data or architecture — it was CSS. I spent way too much time polishing the UI before the underlying logic was stable. It looked nice, but it slowed everything down. If I could go back, I’d ship ugly, make it work, then make it pretty.

Where things finally clicked was when I leaned into reusable components. Once I started thinking “components are just functions, props are inputs,” the project got easier to reason about. That was my real “aha” moment — not a fancy pattern, just a clearer mental model.

State management was another lesson. At the time, I kept it lightweight: local state, a small context, sessionStorage for login state, and Express sessions persisted in MySQL. It worked. If I rebuilt the same project now, I’d still keep it simple, but I’d reach for TanStack Query for server state and Zustand for small UI state. It’s not about chasing shiny tools — it’s about matching the tool to the type of state you’re managing.

The debugging habit that saved me was React DevTools in Chrome. Being able to inspect props and state in real time made bugs visible instead of mysterious.

If I could talk to my past self before starting, I’d say three things: ship ugly, build small components early, and don’t be afraid to break big ideas into tiny pieces. React rewards that mindset.

## References

- React documentation: https://react.dev
- TanStack Query documentation: https://tanstack.com/query/latest
- Zustand documentation: https://zustand.docs.pmnd.rs
- React DevTools overview: https://react.dev/learn/react-developer-tools
