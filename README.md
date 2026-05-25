# GTM Skills

Your team already knows what good looks like — which accounts to pursue, which contacts matter, what signals mean someone's ready to buy. The problem is that knowledge lives in your best people's heads: never written down, never pressure-tested, never turned into something the rest of the team can use.

These skills pull that knowledge out through conversation, organize it into documented frameworks, and give you something you can actually hand to a rep, load into an agent, or build a workflow around.

Built by the [MedScout](https://medscout.io) team. Part of the [Stage 2 Capital GTM AI How To](https://stage2.capital) series.

## Install

```bash
claude plugin marketplace add medscout-gtm/gtm-skills
claude plugin install gtm-skills
```

Codex support coming soon.

## What's in here

### Domain skills

Each of these walks you through building a specific piece of your GTM playbook. They run as guided conversations — you talk through what you know, react to real examples, and end up with a documented framework.

| Skill | What it does | Time |
|---|---|---|
| **Target Account Playbook** | Build a qualification framework for which accounts to pursue. Walk through good-fit and poor-fit customers, surface the attributes and signals that actually predict success, organize them by when they become assessable. | 90–120 min |
| **Contact Qualification Framework** | Build qualification criteria for which people at target accounts are worth pursuing. Review real LinkedIn profiles, extract your judgment about what makes someone a fit, produce documented persona classification and fit assessment. | 60–90 min |

### Underlying tools

The domain skills are built on two general-purpose tools that you can also use directly.

| Skill | What it does |
|---|---|
| **Interview Me** | Guided conversation that turns fuzzy thinking into sharp articulation. Handles voice-to-text brain dumps, half-formed ideas, implicit knowledge that hasn't been written down. |
| **Crystallization** | Takes rough material and sharpens it through iterative rounds — reflect back what you heard, push on what's vague, tighten until it's precise. The methodology underneath Interview Me, also useful on its own for tightening a draft or plan. |

## How it works

Every domain skill follows the same pattern: an interview that extracts what you know, then a generation step that organizes it into a framework you react to and refine. At the end, a validation pass pressure-tests the result — where would this give you the wrong answer? Which criteria are you least confident in? What would trip up someone using this without your judgment behind it?

You end up with one document you can share with your team, plus a record of how your thinking evolved during the session — useful context when you revisit the framework later.

**Voice-to-text works best.** The interview mechanics are built for brain-dump-style input. Typing works, but dictation (Wispr Flow, Monologue, or the built-in mic) is faster and usually produces richer material.

## Why this approach

The tools you use to qualify accounts, find contacts, and prioritize outreach will change. The models will change. The specific workflow — whether it's Clay or Apollo or something that doesn't exist yet — will change.

What doesn't change is your judgment about what matters for your business. Which accounts are actually a fit. Which people at those accounts would drive an evaluation. What signals tell you someone is ready to buy versus just browsing.

That judgment is the input that makes everything else work. Without it, AI tools generate noise at scale. With it, they apply your best thinking consistently across every account and every contact.

These skills exist to help you get that judgment out of your head and into a form you can use.

## Usage

Open Claude Code and describe what you want to do:

- "Help me build a target account qualification framework"
- "I need to figure out which contacts at my accounts are worth pursuing"
- "I want to think through [topic] — interview me"
- "I have a rough draft of [X], help me sharpen it"

Claude picks the right skill based on the description.

## What to have ready

The skills adapt to whatever you bring, but having a few things ready avoids interruptions:

- **For account qualification:** Your current ICP thinking (even rough notes), plus 3–6 real customers you can talk about — a mix of best-fit and poor-fit.
- **For contact qualification:** A contact search tool open on another screen (Sales Navigator, LinkedIn, ZoomInfo — whatever you have). Optionally, CRM data on contacts from closed deals.
- **For either:** A voice-to-text tool if you prefer dictation over typing.

## Feedback

Issues and improvements welcome — open a PR or issue on this repo.

## License

MIT.
