---
title: Setup — Get your Mac ready
subtitle: Install one app yourself, then let the AI set up the rest
eyebrow: Before Day 2
draft: true
order: 1.5
---

<!-- layout: title -->

# Get your Mac ready

Let the AI set up your computer.

<!-- notes:
Do this at the end of Day 1, after accounts, or first thing on Day 2.
The full written guide is at /setup on this site, with copy buttons for every command and the setup message. Have it open on the projector as a backup.
-->

---

<!-- layout: statement -->

## You install **one** app.

The AI installs everything else, and explains it as it goes.

<!-- notes:
This is "teach them to fish". Setting up a dev machine is something real developers
google every time. Now we ask the AI instead.
-->

---

## What a developer's Mac has

| Tool | It's like… |
| --- | --- |
| **Claude app** | An assistant who can use your computer |
| **Terminal** | Texting your computer |
| **Homebrew** | An app store for developer tools |
| **git** | Save points in a game |
| **Node.js** | The engine that builds your website |
| **VS Code** | Notepad, but for code |

<!-- notes:
Don't explain these deeply. They'll hear each one again from Claude during setup.
-->

---

## Step 1 · Get the Claude app

1. Go to **claude.ai/download**
2. Download the Mac app, drag it into **Applications**
3. Open it and log in

<!-- notes:
Write claude.ai/download on the whiteboard.
If login fails for anyone, pair them with a neighbor, or switch them to the
claude.ai-in-the-browser fallback (last slide).
-->

---

## Step 2 · Make a home for your work

In **Finder**, press **⌘ Shift H**, and make a new folder called **Projects**.

Then in the Claude app: **Code** tab → choose **Projects**.

<!-- notes:
Everyone using the same folder name makes it much easier to help them.
-->

---

<!-- layout: two-col -->

## Step 3 · Ask for help

Paste the setup message from the guide into the **Code** tab.

It asks Claude to install everything, **one step at a time**, and to explain each step first.

::right::

> Help me set up this Mac for web development. I'm a beginner…

Copy it from the **[setup guide →](/setup)**

<!-- notes:
The setup guide at /setup has a "Copy message" button for this prompt.
-->

---

## What to expect

- 💻 A **popup** asks to install developer tools → click **Install**
- 🔑 Claude asks you to paste a command in **Terminal** and type your **Mac password** → **nothing shows on screen**. That's normal!
- ✋ Claude asks **permission** before each command → **read it**, then approve
- 💥 Something **fails** → copy the error, paste it to Claude

<!-- notes:
Say the password thing out loud twice. Everyone thinks their keyboard is broken.
Xcode Command Line Tools can take 10–20 minutes on slow wifi. Start it early.
-->

---

<!-- layout: statement -->

## Errors are **normal.**

Paste the error. Say what you expected. Let the AI fix it.

That's not cheating. **That's the job.**

---

## Step 4 · Check it worked

Ask Claude:

> Check that git, node, npm, gh, and code all work, and that I'm logged in to GitHub.

Everything ✅? You're a developer now. 🎉

---

## Plan B

The Claude app won't install or log in?

1. Open **claude.ai** in your browser
2. Paste the same setup message
3. Add: *"Give me each command to paste into Terminal myself."*

Slower, but the same idea: **the AI is your guide.**
