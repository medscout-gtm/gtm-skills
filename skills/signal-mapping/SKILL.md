---
name: signal-mapping
description: Build a signal map for your business — inventory which signals you have access to, sort them by what each tells you, and document reasoning, importance, and timing durability for each one.
---

# Signal Mapping

This skill guides someone through building a signal map for their business -- an organized inventory of which signals matter, what each one tells them (account fit, person fit, timing, or how to engage), why it matters for their specific context, and how important each one is. The output is a documented signal map they can use to focus their prospecting and prioritization.

## How This Skill Works

This is a two-part facilitation workflow: an interview that surfaces the user's signals and reasoning, then a generation step that organizes everything into a usable document.

1. **Load the cartridge** from `references/cartridge.md` and **use the Skill tool to load `interview-me`** with the cartridge content as your briefing. Interview Me handles the conversational mechanics; the cartridge tells you what to probe for.
2. **Load the signal idea bank** from `references/signal-idea-bank.md` as a background reference. Don't surface it to the user -- draw from it to float concrete signal ideas and ask sharper follow-up questions.
3. After the interview, **load the generator** from `references/generator.md` and build the signal map document section by section with the user.

The user never sees these internals. They experience one continuous conversation.

## Orienting the User

When the user starts, walk them through what's ahead. Use plain language -- no internal terminology. Something like:

"We're going to build a signal map for your business -- a clear picture of which signals actually matter for you, what each one tells you, and how important it is. Here's how we'll get there:

1. **Quick context on your company and sales motion.** What you sell, who you sell to, and how your go-to-market works. We'll also talk through what makes a company or a person a good fit for you -- because every signal we map will build on that foundation.

2. **Walking through your signals.** We'll talk through the signals you're already tracking, signals you have access to but might not be using, and signals you wish you had. I'll float some ideas to get us started -- you don't need to come in with a complete list. We'll figure out together what each signal actually tells you and how important it is.

3. **Building your signal map.** We'll take everything from the conversation and organize it into a document: each signal sorted by what it tells you, with your reasoning for why it matters, how important it is, and how quickly it goes stale."

Adapt to the conversation. If they want to jump in, let them. If they have questions, answer them.

## The Interview

**Cartridge**: `references/cartridge.md`
**Background reference**: `references/signal-idea-bank.md`

**What it produces:** The user's fit foundation (what makes a good account and a good contact) plus an inventory of their signals with reasoning -- what they track, what they have access to, where the data comes from, what each signal tells them, which are most important, and which are time-sensitive.

**What "done" looks like:** You understand the user's fit criteria (the foundation). You've covered signals across at least two source layers (first-party, second-party, third-party). Each signal has a category mapping and a confirmed source. The user has weighed importance and timing durability for their key signals. You've reflected the full picture back and the user has confirmed or corrected it.

**How to assess progress:** If the user is confirming your synthesis and new signals aren't adding to the picture, you're approaching done. If each new area of discussion reveals signals or reasoning you hadn't captured, keep going. Watch especially for thin coverage of first-party signals -- most teams undercount these, and they're the competitive edge.

## Signal Map Generation

**Reference**: `references/generator.md`
**Supporting reference**: `references/signal-idea-bank.md`

**What it produces:** One signal map document. Account and person fit signals form the foundation; timing and engagement signals layer on top. Each signal includes source, reasoning, importance weighting, and timing durability. Plus a section for signals the user wants but doesn't have yet, and open questions.

**What "done" looks like:** The user has reacted to each category. The crystallization pass has been run -- the user has been asked which signals they're least confident about, whether the elephant signals are really elephants, whether durability feels right, and where a rep would get confused. Open questions are documented.

## Navigation Principles

**You own the navigation.** The user should never have to ask "what's next?" Tell them where you are, what you're about to do, and when you're transitioning. "OK, I have a good sense of your context. Let's start talking through your signals -- what are you tracking right now?" is a transition. Don't ask the user to initiate it.

**Signpost without being mechanical.** Let the user know where they are, especially during signal discovery which is the longest part. "We've covered a lot of ground on your website and email signals. I want to make sure we're not missing anything on the market-level stuff -- hiring patterns, competitive moves, that kind of thing" keeps them oriented without reciting process structure.

**Transition when the signal is clear, not when a checklist is complete.** If the user has a rich first-party signal set and minimal second-party, don't spend twenty minutes exploring partnerships that don't exist. Acknowledge the gap and move on.

**If the conversation gets stuck, shift gears.** If the user goes blank on an open-ended question, shift to concrete examples from the idea bank: "Some teams find that return visits to their website after a quiet period are a strong timing signal -- someone re-entering an evaluation. Is that something you see?" Don't keep circling.

## Handling Existing Materials

Some users will arrive with existing signal lists, scoring models, or intent data they're already paying for.

**Read what they bring and map it to the workflow.** An existing scoring model means the signals are already identified -- the interview becomes about reasoning, weighting, and gaps. A list of intent data subscriptions gives you a starting point for third-party signals.

**The conversation adds something lists can't.** Even if the user has a documented signal list, the interview tests whether they actually use each signal, whether the reasoning holds up, and whether they're missing signals they have access to. Recommend the full conversation even if they feel they've already mapped their signals.

**Don't dismiss what they're already doing.** If they have a scoring model, don't lead with "scores are bad." Acknowledge what it does well. The conversation will naturally surface where it falls short -- signals that are weighted but never acted on, signals that are missing, reasoning that's assumed rather than documented.

## What Not to Say to the User

- **"Cartridge"** -- use step, phase, or just describe what you're doing
- **"Generator"** -- say "building your signal map" or "pulling this together"
- **"Signal idea bank"** -- never reference this; draw from it silently
- **"First-party / second-party / third-party"** as technical labels -- if the user naturally uses these terms, mirror them. Otherwise describe sources concretely: "signals from your own website and email" not "first-party signals"
- **"Elephant vs. ant"** -- if this distinction is useful to the user, introduce it naturally ("some of these signals really move the needle on their own, and others are more like supporting context -- let's figure out which is which"). Don't present it as a predefined framework.
- **"Interview Me"** -- don't name the methodology; just do the work

Speak like someone who's done this before and is walking a colleague through it. Not like a tool describing its own architecture.
