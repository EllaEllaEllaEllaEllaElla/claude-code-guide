# Terminal & Shell Study Guide

A running reference for everything covered in our sessions.

---

## The Shell

Your **shell** is a program that lets you talk to your computer by typing commands instead of clicking.

When you open Ghostty, you're looking at a shell. On your Mac, the shell is called **zsh** (Z shell). There are others (bash, fish) but zsh is the Mac default.

Think of it like this:
- **Ghostty** = the window (the terminal emulator — just displays things)
- **zsh** = the actual program listening to your commands

When you type `ls` or `cd` or any command, zsh is the thing reading it and making it happen.

---

## ~/.zshrc

A hidden file in your home folder (`~` = home) that zsh reads automatically every time you open a new terminal window.

It's a setup script — anything you put in there runs before you see the prompt. This is where you store permanent aliases, environment variables, and other config.

- `~` = shorthand for `/Users/ellajacobs`
- `.zshrc` = the file (the `.` at the start makes it hidden in Finder)
- To see it: `cat ~/.zshrc`
- To edit it: open it in any text editor, or use Claude Code

After editing `.zshrc`, run `source ~/.zshrc` to apply changes without reopening the terminal.

---

## Aliases

A shortcut for a command you'd otherwise have to type in full.

```zsh
alias dpusite='claude "/Users/ellajacobs/Desktop/projects/DPU/THEDPU.ORG WEBSITE"'
```

- `alias` = the keyword that creates a shortcut
- `dpusite` = the name you'll type
- everything after `=` = what actually runs

**Rules:**
- No spaces in the alias name
- Put the command in quotes if it contains spaces or special characters
- Defined in `.zshrc` to make them permanent

---

## Environment Variables

Variables that live in your shell session and programs can read them.

```zsh
export ANTHROPIC_API_KEY="sk-..."
```

- `export` = makes it available to any program you run from the shell
- `ANTHROPIC_API_KEY` = the variable name (all caps is convention)
- the string after `=` = the value

**Security rule:** Never put real API keys or passwords in files that could be shared or pushed to GitHub. Use `claude login` instead, which stores credentials securely.

---

## Useful Commands

| Command | What it does |
|---|---|
| `ls` | List files in current folder |
| `cd foldername` | Move into a folder |
| `cd ..` | Go up one folder |
| `cat filename` | Print a file's contents to the terminal |
| `source ~/.zshrc` | Reload your zshrc without restarting |
| `pwd` | Print your current location |

---

## Things to Learn Next
- Git & version control
- What an API is and how to call one
- How Claude Code agents work
- What a server does

*(See learning-roadmap.md for the full list)*
