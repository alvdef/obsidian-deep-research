# Vault Researcher

An [Agent Skill](https://agentskills.io/specification) that turns Claude into a research partner for your Obsidian vault. Give it a topic and it searches the web, synthesizes findings into structured notes, links everything together, and asks what to dig into next.

Inspired by [Obsidian: The King of Learning Tools](https://youtu.be/hSTy_BInQs8?si=Ai9_s4XWiYTMyQJJ) by Odysseas.

## What it does

You give it a topic, a question, or a document. It uses Claude's web search to research the subject, creates notes from what it finds, connects them to your existing knowledge, and surfaces new questions. You decide whether to go deeper, pivot, or stop — it never continues without asking.

- **Research** — searches the web, creates notes from findings, links them into your vault, surfaces new questions and contradictions, repeats with your approval
- **Decomposition** — takes a document (PDF, AI report, pasted text) and breaks it into individual notes, each rewritten and linked
- **Verification** — finds uncertain notes and searches for corroborating or contradicting evidence to update their confidence level

Every session ends with a closing checklist: update index pages, refresh the research backlog, write a timestamped log entry, and clean up project context.

## How opinionated it is

Very. The skill follows a [Zettelkasten](https://en.wikipedia.org/wiki/Zettelkasten)-inspired methodology and enforces a specific structure for folder layout, file naming, frontmatter schemas, tagging, and linking. Every note must connect to an index page and at least one related note. Note titles state a claim, not a topic. AI-generated notes are tagged as uncertain until verified.

If you want a lighter system, this isn't the skill for you. If you want a vault that stays searchable and connected over months of research, it will do the work to keep it that way.

## Requirements

- [`obsidian` CLI](https://help.obsidian.md/cli) (from [kepano/obsidian-skills](https://github.com/kepano/obsidian-skills))
- [`defuddle-cli`](https://github.com/kepano/defuddle-cli) (`npm install -g defuddle-cli`)



## License

MIT
