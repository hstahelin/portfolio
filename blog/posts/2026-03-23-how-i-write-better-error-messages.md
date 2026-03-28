---
title: "How I Write Better Error Messages as a Developer with Support Experience"
slug: "how-i-write-better-error-messages-support-to-dev"
description: "How support experience changed the way I write error messages: clearer next steps, retry guidance, and fewer unnecessary support tickets."
tags: ["ux-writing", "web-development", "support", "developer-experience", "product"]
reading_time: "5–6 min"
author: "Hugo Stahelin"
date: "2026-03-23"
keywords:
  - error message best practices
  - user-friendly error messages
  - support to developer transition
  - UX writing for developers
  - reduce support tickets
  - actionable error messages
  - validation error copy
  - permission error UX
---

# How I Write Better Error Messages as a Developer with Support Experience

If I had to pick one sentence I never want to ship again, it’s this: **“Something went wrong.”**

I’ve seen that line from both sides — as someone in support receiving frustrated tickets, and now as someone building products. The problem with vague errors isn’t just bad UX. It creates extra support load, slows down debugging, and leaves users stuck with no idea what to do next.

My support background changed how I write errors. I don’t treat error copy as a minor detail anymore. I treat it as part of the product.

## Why vague errors are expensive

In support, unclear errors created avoidable tickets all the time. People didn’t open tickets because they wanted to. They opened tickets because the product gave them no path forward.

“Something went wrong” sounds harmless, but it pushes all the work onto the user:

- They don’t know what failed
- They don’t know if they can retry
- They don’t know what to change

That confusion eventually lands in support, then in engineering, and everyone loses time.

## My default rule: every error must give next steps

A good error message should help the user recover, not just report failure. My baseline is simple: if someone sees this error, can they do something useful in the next 10 seconds?

I prefer direct and neutral tone: clear, specific, no fluff, no blame.

## Two real patterns where wording matters

### 1) Permission errors

**Before:** “Access denied.”
**After:** “You need Admin access to edit billing settings. Contact your workspace owner.”

This small rewrite changes everything. It tells users:

- what they were trying to do
- why it failed
- exactly what to do next

### 2) Validation errors

**Before:** “Invalid request.”
**After:** “Phone number must include country code (e.g., +1).”

This is the difference between guessing and fixing. The best validation errors point to the exact field and expected format.

## The 3 things every error message should include

From my support-to-dev experience, every user-facing error should include:

1. **A clear next step**
2. **Retry/contact guidance**
3. **Specific location or cause when relevant**

When you include these three, support tickets drop and trust improves.

## Clarity for users beats developer convenience

I still need technical detail for debugging — but I don’t force all users to read technical internals. My approach is:

- keep primary error copy user-friendly
- optionally expose deeper details/context for troubleshooting

That keeps the main experience clean while still helping teams diagnose issues fast.

## Quick checklist I now use before shipping

Before I merge a feature, I do a fast error-copy pass:

- Does the message explain what failed in plain language?
- Does it suggest the next action (retry, fix input, contact someone)?
- Is the guidance specific enough that support won’t need a follow-up question?

This takes a few minutes, but it saves hours later.

## If you still ship “Something went wrong…”

Try this test: imagine you are the user seeing your error with no extra context. What would you do next?

If the honest answer is “I don’t know,” the message needs rewriting.

Error messages are not edge polish. They are part of the core product experience. And in many cases, they’re the difference between a user completing a task or opening a support ticket.
