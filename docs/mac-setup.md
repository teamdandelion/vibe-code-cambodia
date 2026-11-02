# Set up your Mac for building websites

You're going to set up your Mac the way professional developers do — but you're not going to do it by hand. You'll install **one** app yourself (Claude), and then ask the AI to set up everything else, step by step, explaining as it goes.

This is the most important skill in this workshop: **when you don't know how to do something, ask the AI to do it with you.**

## What gets installed, and why

| Tool | What it is | Why you need it |
| --- | --- | --- |
| **Claude app** | The AI app. Its **Code** tab writes code and runs commands for you | It does the rest of this setup with you |
| **Terminal** | A window where you type commands to your Mac | Already on every Mac. You'll use it for the steps that need your password |
| **Xcode Command Line Tools** | Apple's basic tools for developers | Many other tools need them. Includes **git** |
| **Homebrew** | An "app store" for developer tools, used from Terminal | Makes installing everything else one command |
| **git** | Keeps every version of your files, like save points in a game | So you can always go back, and send your work to GitHub |
| **GitHub CLI** (`gh`) | Connects your Mac to your GitHub account | Lets you push your website to GitHub without passwords |
| **nvm + Node.js** | Node runs JavaScript tools on your computer; nvm installs and switches Node versions | Astro (what builds your website) runs on Node |
| **VS Code** | A text editor for code | Handy for looking through all your files (optional, the Claude app shows changes too) |

## Step 1 · Install the Claude app

1. Go to **[claude.ai/download](https://claude.ai/download)** and download the Mac app.
2. Open the download and drag **Claude** into **Applications**.
3. Open Claude and log in with your Claude account.

## Step 2 · Make a Projects folder

In **Finder**, go to your home folder (**⌘ Shift H**) and make a new folder called **Projects**. Your websites will live here.

## Step 3 · Ask Claude to set up the rest

In the Claude app, open the **Code** tab, choose your **Projects** folder, and paste this message:

> Help me set up this Mac for web development. I'm a beginner. Please check what's already installed, then install whatever is missing from this list, one at a time: Xcode Command Line Tools, Homebrew, git, the GitHub CLI, nvm with the latest LTS version of Node.js, and VS Code (with the `code` command in the Terminal).
>
> Before each step, tell me in one sentence what it is and why I need it. If a step needs my Mac password or a popup window, give me the exact command to paste into Terminal myself (and remind me how to open Terminal), and wait for me to say "done". After each step, check that it worked.
>
> At the end, help me log in to GitHub with `gh auth login`, set my git name and email, and show me a short summary of everything that's installed.

Then follow along. Read what the AI says before you approve each command — that's how you learn what's happening.

### Things that will happen

- **A popup about "command line developer tools."** Click **Install** and wait. This can take 10–20 minutes on slow internet.
- **Your Mac password.** When you type it in Terminal, **nothing appears on screen** — no dots, no stars. That's normal. Type it and press Return.
- **Claude asks permission** before running commands. Read what it wants to run, then approve it.
- **Something fails.** That's normal too. Copy the error, paste it to Claude, and say "this happened". This is the real skill.

## Step 4 · Check it worked

Ask Claude: *"Check that git, node, npm, gh, and code all work, and that I'm logged in to GitHub."*

Or run it yourself:

```bash
git --version && node --version && npm --version && gh auth status && code --version
```

Every line should print a version number or "Logged in". You're ready.

To open Terminal: press **⌘ Space**, type **Terminal**, press **Return**.

## If the Claude app won't install or log in

Use [claude.ai](https://claude.ai) in your web browser instead. Paste the same Step 3 message, and add: *"Give me each command to paste into Terminal myself."* It's slower, because you copy and paste every command, but it works the same way. Then try the app again.
