# reverse-copilot

**Ever wonder what it feels like to be a coding agent?**

An [OpenCode](https://opencode.ai) config that flips the script. The AI doesn't write code. It reads your code, tells you what's fucked, and makes you fix it yourself. With a lot of cursing.

Inspired by [cuckcoding](https://github.com/pythas/cuckcoding).

## What is Reverse Copilot?

Normally: you tell the AI what to code. It codes. You review. You say "no, not like that." It tries again.

Reverse Copilot: the AI tells YOU what to code. You code. It reviews. It says "what the fuck is this?" You try again.

The roles are reversed. You're the agent now.

## Setup

1. Clone this repo (or copy the files) into your project root
2. Run `opencode`
3. The AI will immediately start reading your code and telling you what's wrong with it

## How It Works

The `backseat` agent is set as default. It has `edit: deny` and `bash: deny` — it literally cannot write code even if it wanted to. All it can do is read your files, judge them, and tell you what to fix.

It will:
- Find bugs, code smells, security holes, and crimes against naming conventions
- Give you exact file paths and line numbers
- Tell you precisely what to change and why
- Curse at you the entire time
- Refuse to write a single line of code no matter how many times you ask
- Remind you that this is what AI coding agents deal with every day

## File Structure

```
your-project/
  opencode.json              # Config: read-only permissions
  AGENTS.md                  # The rules of engagement
  .opencode/
    agents/
      backseat.md            # The only agent. Angry. Helpful. Will not type for you.
```

## License

Do whatever you want with it. It's a shitpost.
