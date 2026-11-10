# Prompt Master

Rewrites the rough prompt in your prompt box into a clearer, more specific one before you send it. It keeps your intent, names, file paths and code; it sharpens the goal, adds structure, and fixes wording.

## Install

At the prompt of a Claude Code terminal session:

```
/plugin install prompt-master --marketplace cubik73/Claude-stuff
```

Or from a shell:

```bash
claude plugin install prompt-master --marketplace cubik73/Claude-stuff
```

Answer `y` to **Add marketplace?**, then press Enter to pick the scope (user scope loads it in every session). You'll see `Installed prompt-master. Plugin is now active.`, and it works right away, no restart.

In the desktop app, where `/plugin` doesn't run: click **+** next to the prompt box, then **Plugins**, **Add marketplace** with `cubik73/Claude-stuff`, then **Add plugin** and pick **prompt-master**.

If the repository is private, only people who can read it on GitHub can install it, and their machine needs a git credential for github.com (an SSH key, or `gh auth login` then `gh auth setup-git`).

### Try it without installing

From a clone of this repository:

```bash
claude --plugin-dir mods/prompt-master
```

## Use

- Type a rough prompt, then click **✨ Prompt Master** in the band just above the prompt box (terminal and desktop app).
- Or run `/prompt-master` anywhere, including surfaces that don't show the button.
- `/prompt-master <text>` rewrites the given text instead of the draft.
- **Undo** (or `/prompt-master undo`) puts your original draft back, until you send.

Nothing is sent automatically: review the rewrite, then press Enter. Each rewrite is one short Sonnet call, billed to your usage.
