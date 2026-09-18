# Git Basics: Commits, Branches & Merging

## Commits

A commit is a **snapshot** of your project at a specific point in time — like a save point in a video game.

- Git doesn't blindly copy your entire directory on every commit. Instead, it compresses each commit into a set of _changes_ (a "delta") from the previous version whenever possible.
- Git keeps a full **history** of commits, and most commits have a parent commit — the one that came right before it. This history is what makes collaboration possible.
- Commits are lightweight, and switching between them is fast.

> **Simple version:** Think of committing like taking a photo of your LEGO castle every time you finish a piece. Git doesn't rebuild the whole castle each time — it just jots down what changed since the last photo. All your photos are kept in an album (history) so you can see how the castle grew.

### Git Status

Before you commit (or switch branches), it's a good habit to check git status:

```
git status
```

This tells you:

- Which branch you're currently on
- Which files have been changed but not yet staged
- Which files are staged and ready to be committed
- Whether your working directory is "clean" (no changes at all)

> Simple version: git status is like asking, "Hey, what's going on with my LEGO castle right now? Did I move any pieces? Are any of them ready to be photographed (committed)?" It doesn't change anything — it just tells you what's up.

## 🌿 Branches

A branch is simply a **pointer** to a specific commit — nothing more. There's no extra storage cost to creating one:

Think of a branch as saying: _"I want to include the work of this commit, and all its parent commits."_

### Working with branches

Create a new branch:

```bash
git branch <name>
```

Switch to (check out) a branch:

```bash
git checkout <name>
```

> Since Git 2.23, there's also `git switch`, intended to eventually replace `git checkout` for this purpose. It's still considered experimental, so its syntax may change.

**Shortcut** — create a branch _and_ switch to it in one step:

```bash
git checkout -b <yourbranchname>
```

> **Simple version:** A branch is like a "pretend timeline" for your LEGO castle. Want to try adding a dragon without messing up your real castle? Make a branch! It's free to create as many as you want, so try things freely.

## Merging

Merging combines the work from two different branches. This lets you branch off, build a feature, and bring it back into the main line of work.

`git merge` creates a special commit with **two parents**. A two-parent commit means: _"Include all the work from this parent, and this other parent, and the set of all their ancestors too."_

```bash
git checkout main
git merge dragon-idea
```

> **Simple version:** Merging is like gluing your "dragon timeline" back onto your real castle — now your castle has everything from both timelines combined into one.

---

### Quick Reference

| Command                   | What it does                                     |
| ------------------------- | ------------------------------------------------ |
| `git branch <name>`       | Create a new branch                              |
| `git checkout <name>`     | Switch to an existing branch                     |
| `git checkout -b <name>`  | Create _and_ switch to a new branch              |
| `git switch <name>`       | (Experimental) Switch branches                   |
| `git merge <name>`        | Merge the named branch into your current branch  |
| `git add <name of file>`  | adds your file so you can sen it                 |
| `git add .`               | adds all your files so you can send them         |
| `git commit -m "message"` | adds a message to the commit                     |
| `git push`                | sends your files to github inside the reopsitory |

## sequence of usage to push files to github

- git add .
- git commit -m
- git push

# Git Homework: Your First Branches

Using what you learned in the `README.md` (commits, branches, and merging), complete the tasks below.

## Setup

You already have a repo — just make sure you're starting from your main branch (`main` or `master`) with no uncommitted changes:

- check on which branch you are
- switch to main

## Your Tasks

1. **Create a branch called `learning_git`** and switch to it.

2. On the `learning_git` branch, create a file named `test` with some content inside it, then commit that change with a clear commit message.

3. **Create a second branch called `submit`** — but make sure it's created starting from `main` (or `master`), _not_ from `learning_git`. This branch's only purpose is to receive the merge from `learning_git`.

4. While on the `submit` branch, merge `learning_git` into it.
   - What kind of commit did Git create?
   - How many parents does it have, and why?

## ✅ What to Turn In

Answer these three questions in a text file or comment:

1. What command did you use to create the `learning_git` branch and switch to it at the same time?
2. Before merging, did `submit` include the changes you made on `learning_git`? Why or why not?
3. After merging, what changed on `submit`?
