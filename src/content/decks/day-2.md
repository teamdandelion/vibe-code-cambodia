---
title: Day 2 — Build your own
subtitle: Your idea, your website, live on the internet by the end
eyebrow: Day 2
draft: true
order: 2
---

<!-- layout: title -->

# Build your own

Day 2

---

<!-- layout: statement -->

## What's your **idea?**

One sentence each: what is it, and who is it for?

<!-- notes:
Go around the room. If someone is stuck, offer one from yesterday's whiteboard list.
-->

---

## Your tools today

- **Claude app, Code tab** — the AI you talk to. It changes your files and shows you the website
- **VS Code** — look through all your files (optional)
- **GitHub + Cloudflare** — put it online

---

## Step 1 · Get your copy

1. Go to the **template repository** on GitHub
2. Click **Use this template** → **Create a new repository**
3. Give it a name, like `my-bakery-site`

Now you have your own copy. You can't break mine. 🙂

<!-- notes:
Put the template URL on the whiteboard. Use "Use this template", NOT "Fork" — a fork
sends their changes back toward your repo.
-->

---

## Step 2 · Put it on your computer

In the Claude app, **Code** tab, in your **Projects** folder, ask:

> Clone my GitHub repository my-bakery-site into this folder and install it.

Then start a **new session** and choose the **my-bakery-site** folder.

<!-- notes:
Walk the room. Most problems here are typos or being in the wrong folder.
Anyone who skipped Mac setup: send them to the Setup deck first.
The new session matters: Claude only reads the project's CLAUDE.md and /make-it-mine
when the session is opened in the project folder itself.
-->

---

<!-- layout: statement -->

## Step 3 · Make it yours

In the Code tab, type:

**/make-it-mine**

It will ask you about your idea, then rebuild the site for you.

<!-- notes:
This command deletes the lesson slides and rewrites the homepage around their idea.
Afterwards, they ask Claude to "show me the preview" and the site opens beside the chat.
-->

---

## Step 4 · Ask, look, steer

Ask Claude to **show you the preview**, then keep asking:

- "Make the headline shorter and bolder"
- "Use colors that feel like fresh bread"
- "Add a section with three prices"
- "It looks broken on my phone — fix it"

**Be specific.** "Make it better" is hard. "Make the title bigger" is easy.

---

<!-- layout: section -->

## Putting it online

---

## Step 5 · Connect Cloudflare (once)

1. Cloudflare dashboard → **Workers & Pages** → **Create**
2. **Import a repository** → connect GitHub → pick your repo
3. Click **Deploy**

A minute later you get a link: `your-site.your-name.workers.dev`

That's your website. On the internet. 🎉

<!-- notes:
Do this together, step by step. If the build fails, the usual cause is the Worker
name not matching "name" in wrangler.jsonc. Ask Claude to fix it.
Fallback if GitHub won't connect: npm run build, then drag the dist folder into a Cloudflare Pages upload.
-->

---

## Saving your work: Git in 30 seconds

| Word | Means |
| --- | --- |
| **commit** | a save point |
| **push** | send your save points to GitHub |
| **branch** | a draft copy you can try things on |
| **pull request** | "here's my draft — preview it, then accept it" |

You can just ask Claude: *"commit and push my changes."*

<!-- notes:
Only go deep here if they hit a wall. The one idea that matters: every push makes
Cloudflare rebuild the site automatically.
-->

---

<!-- layout: two-col -->

## Preview links

Change something on a **branch**, open a **pull request**, and Cloudflare gives you a private preview link.

Like it? **Merge** — and your real site updates.

::right::

> "Make a branch called new-prices, change the prices section, and open a pull request."

---

<!-- layout: statement -->

## Goal for today

**Your** website, live, at a link you can send your family.
