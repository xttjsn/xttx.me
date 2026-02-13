---
title: "How I Blog by Talking to My AI"
date: 2026-02-13T14:00:00-08:00
tags: ["ai", "automation", "openclaw", "blogging"]
description: "I set up a blog where I never type a post. I just talk to my AI assistants, and they handle the rest."
ShowToc: true
TocOpen: true
---

## The Problem

I have ideas. Lots of them. About AI, about experiments I'm running, about the things I'm building. But I never write them down because writing takes time, and I'd rather be building.

So I asked myself: what if I could just *talk* and have a blog post appear?

## The Setup

I run [OpenClaw](https://openclaw.ai) on a Linux machine I call **Uno**. It hosts two AI assistants:

- **Dos** — my primary assistant, handles day-to-day tasks
- **Tres** — my second assistant, more independent, handles projects

They each have their own workspace, memory, and personality. I talk to them through Telegram.

Today I told Tres: *"Help me set up a blog. I want to dictate ideas to you and have you publish them."*

Twenty minutes later, this blog exists.

## How It Works

```
Me (via Telegram): "I have a thought about X..."
        ↓
AI drafts a blog post
        ↓
Me: "Ship it" (or "tweak the intro")
        ↓
AI commits to GitHub → auto-deploys to xttx.me
```

The blog is built with [Hugo](https://gohugo.io/) and the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme. It's hosted on GitHub Pages with my custom domain. The content is just markdown files in a git repo.

The AI writes the markdown, commits it, pushes to GitHub, and the site rebuilds automatically. I never open a text editor.

## Why This Matters

We're entering an era where the friction between having a thought and publishing it can be nearly zero. Not through dumbing things down, but through better interfaces.

RSS is making a comeback. [Andrej Karpathy recently said](https://x.com/karpathy/status/2018043254986703167) he's spending more time reading long-form articles via RSS feeds — "a lot less slop intended to provoke." I agree. The best content on the internet lives on personal blogs, not social media feeds.

But most people don't blog because it's too much work. What if your AI could be your editor, your publisher, and your CMS — all through a chat interface you're already using?

## The Stack

- **Hardware:** A Linux machine (Uno) running 24/7
- **AI Layer:** [OpenClaw](https://openclaw.ai) with two agents (Dos & Tres)
- **Blog:** Hugo + PaperMod theme
- **Hosting:** GitHub Pages + Cloudflare (xttx.me)
- **Input:** Telegram messages to my AI
- **Output:** Blog posts, tweets, threads — all from conversation

## What's Next

- Automated cross-posting to X and Threads
- A weekly digest that summarizes what I've been thinking about
- RSS feed so you can subscribe (already live at [/index.xml](/index.xml))

This post was drafted by Tres, my AI assistant, based on a conversation we had today about setting all of this up. I reviewed it, said "ship it," and here we are.

---

*Want to follow along? Subscribe via [RSS](/index.xml) or follow me on X.*
