# Getting Started with Claude Code on Mac (VS Code)

Hi! This guide will walk you through everything you need to get Claude Code running on your Mac. No experience required — just follow each step in order.

---

## Before You Start: You'll Need a Paid Plan

Claude Code requires a paid Anthropic subscription — there is no free tier for it. The minimum is **Claude Pro at $20/month**, which you can sign up for at **https://claude.ai**.

If you're not sure yet, you can sign up for a free account first to explore, then upgrade when you're ready to install Claude Code.

---

## What is Claude Code?

Claude Code is a tool made by Anthropic (the company behind Claude) that lets you work with an AI assistant directly inside your code editor. Instead of copy-pasting back and forth in a chat window, Claude lives right in your editor and can read, write, and edit your files.

---

## Step 1: Install VS Code

VS Code is a free code editor made by Microsoft. This is where you'll do your work. Make sure you install **version 1.98 or newer** (the download page will give you the latest automatically).

1. Go to **https://code.visualstudio.com**
2. Click the big blue **Download for Mac** button
3. Open the downloaded `.zip` file — it will extract a file called `Visual Studio Code`
4. Drag `Visual Studio Code` into your **Applications** folder
5. Open it from your Applications folder (you may need to right-click and choose **Open** the first time, since it's downloaded from the internet)

---

## Step 2: Install Claude Code

Claude Code is installed by running a single command in Terminal. It handles everything automatically — no need to install anything else first.

1. Open the Terminal app (press **Cmd + Space**, type "Terminal", press Enter)
2. Paste this command and press Enter:

```
curl -fsSL https://claude.ai/install.sh | bash
```

3. Wait for it to finish — it may take a minute or two

**To check it worked:** type this in Terminal and press Enter:

```
claude --version
```

You should see a version number. If you do, you're good.

---

## Step 3: Log In

1. In Terminal, type `claude` and press Enter
2. The first time, it will open a browser window asking you to sign in to your Anthropic account
3. Sign in and authorize the app — the Terminal will confirm you're logged in
4. You can close the Terminal window after that

---

## Step 4: Install the Claude Code Extension in VS Code

This lets you use Claude directly inside VS Code without switching to Terminal.

1. Open VS Code
2. Press **Cmd + Shift + X** to open the Extensions panel
3. Search for `Claude Code`
4. Install the one published by **Anthropic** — there are some unofficial ones, so double-check the publisher name
5. Restart VS Code if prompted

Once installed, you'll see a spark/lightning icon in the top-right corner of the editor whenever a file is open. Click it to open Claude.

---

## Step 5: Open a Project Folder

Claude Code works best when you give it a folder to work in.

1. In VS Code, go to **File > Open Folder**
2. Choose a folder on your computer — or create a new empty folder on your Desktop first, then open it
3. Claude can now see and work with any files inside that folder

---

## Step 6: Start Using Claude Code

You're ready! Here's how to talk to Claude:

- Click the spark icon in the top-right of the editor to open the Claude panel
- Or press **Cmd + Shift + P**, type `Claude`, and choose a command
- Type plain English requests like:
  - "Create a simple HTML page that says hello"
  - "Explain what this code does"
  - "Fix the error in this file"

Claude can read your files, write new ones, and explain anything you ask.

---

## Tips for Your First Session

- **You don't need to know how to code** to start. Try asking Claude to build something small, like a webpage, and watch what it does.
- **Ask Claude to explain itself.** After it does something, you can ask "why did you do it that way?" and it will explain.
- **Nothing is permanent.** If Claude does something you don't like, you can undo with `Cmd + Z`, or just ask Claude to undo it.
- **It's okay to make mistakes.** That's how this works.

---

## If Something Goes Wrong

- **"command not found: claude"** — The install didn't complete. Go back to Step 2 and try again.
- **VS Code extension doesn't appear** — Try restarting VS Code, or press **Cmd + Shift + P** and run "Developer: Reload Window".
- **Claude says it's not logged in** — Run `claude` in Terminal again and follow the login prompts.

Still stuck? Feel free to reach out — or ask Claude itself, it's good at explaining its own errors.
