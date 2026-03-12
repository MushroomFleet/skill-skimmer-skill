# 🔍 Skill Skimmer

**A Claude skill that surfaces automation opportunities hidden in your existing work.**

Skill Skimmer analyses your markdown files, codebases, design documents, and project plans to identify repeatable workflows that would make strong Claude skills. Instead of starting from a blank page, you start from what you've already built — and Skill Skimmer does the reading for you.

It is the first stage of a two-stage workflow: **Skim → Build**. Once candidates are identified, any of them can be handed directly to the [skill-creator](https://github.com/MushroomFleet/) for development without additional clarification.

---

## ✨ What it does

When invoked, Skill Skimmer:

1. Reads all provided material — docs, code, plans, conversation history, GDDs
2. Identifies patterns that signal repeatable, codifiable workflows
3. Returns a **prioritised markdown report** of skill candidates, each with:
   - A short name and one-sentence description
   - An example trigger phrase a user would say to invoke it
   - What goes in, what comes out
   - Why it warrants a skill (what Claude would miss without guidance)
   - Where in your material the signal came from
   - A "Quick spec" for high-priority candidates, ready for skill-creator

No lengthy questioning before the report. It reads first, asks later if needed.

---

## 🚀 How to use it

### Installation

Download `skill-skimmer.skill` from the [Releases](https://github.com/MushroomFleet/skill-skimmer-skill/releases) page and install it into your Claude environment via the Skills panel.

### Invocation

Share your documents, codebase, or plans in a Claude conversation, then say any of the following:

```
Use the skill skimmer to identify skills for creation
```
```
Skim this for skills
```
```
What skills could I extract from this codebase?
```
```
Find skill opportunities in my work
```
```
What could be automated or systematised here?
```

### Example workflow

1. Upload a project plan, GDD, or drop in a codebase
2. Say: *"Use the skill skimmer to identify skill candidates"*
3. Receive a prioritised markdown report
4. Pick your top candidate and say: *"Use the skill creator to build [skill name]"*
5. The skill-creator picks up with a full spec — no re-explanation needed

---

## 📋 Output format

Every report follows this structure:

```
# Skill Candidates — [Source Description]

*Skimmed from: [source summary]*
*N candidates identified — X High / Y Medium / Z Low priority*

## 🔴 High Priority
### skill-name
What it does / Trigger phrase / Input / Output / Why it's a skill / Source signals
[Quick spec for high-priority candidates]

## 🟡 Medium Priority
...

## 🟢 Low Priority / Notes
...

## Next Step
Ready-to-use handoff phrases for skill-creator
```

---

## 🧠 What makes a good skill candidate

Skill Skimmer looks for workflows that are:

- **Repeatable** — triggered across multiple projects, not just once
- **Bounded** — clear start, clear end, recognisable output
- **Currently manual** — something reinvented each time rather than codified
- **Meaningfully specialised** — not something Claude handles well out of the box

Strong signals: multi-step processes in prose, recurring output formats, domain-specific judgment rules, tools composed in non-obvious ways, scripts that always get set up the same way.

---

## 🔗 Works best with

- [skill-creator](https://github.com/MushroomFleet/) — develops candidates identified by Skill Skimmer into fully tested, packaged skills

---

## 📚 Citation

### Academic Citation

If you use this codebase in your research or project, please cite:

```bibtex
@software{skill_skimmer,
  title = {Skill Skimmer: Automated Skill Candidate Identification for Claude},
  author = {Drift Johnson},
  year = {2025},
  url = {https://github.com/MushroomFleet/skill-skimmer-skill},
  version = {1.0.0}
}
```

### Donate

[![Ko-Fi](https://cdn.ko-fi.com/cdn/kofi3.png?v=3)](https://ko-fi.com/driftjohnson)
