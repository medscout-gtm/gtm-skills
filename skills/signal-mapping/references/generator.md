# Signal Mapping Generator

## What This Does

This is the final stage of building a signal map. The user has been through an interview where they inventoried the signals available to their business, discussed what each one tells them, and started to assess importance and durability. Now you're turning that into a usable document.

The output is one document: a signal map that organizes every signal by what it tells the user (account fit, person fit, timing, engagement), with reasoning for why each signal matters for their specific business, elephant/ant weighting, and timing durability.

## How This Stage Works

### Start with a context check

Before building anything, review what came out of the interview. Then tell the user what you're working with:

- **What's clear.** The signals, categories, and weightings you feel confident about. Be specific -- "Your strongest signals seem to be first-party: pricing page visits and outreach responses are both elephants for you, and you have good coverage on timing signals from hiring patterns and competitive displacement" is useful. "I have a good picture of your signals" is not.
- **What's fuzzy.** Where the interview left gaps -- signals the user mentioned but didn't fully explain what they tell them, areas where weighting wasn't clear, source layers that were thin. Distinguish between blockers (things that need to be resolved before you can build) and refinements (things you can flag assumptions about).

Ask about the blockers. For refinements, tell the user: "I think I can work with what I have here -- I'll flag my assumptions as we go and you can correct me."

Keep this brief. A few sentences on what's clear, a few on what's fuzzy, and targeted questions for the blockers.

### Build the signal map with fit as the foundation

The map has a hierarchy, not four equal sections. Account fit and person fit signals are the foundation -- they determine whether an account or contact is worth pursuing at all. Timing and engagement signals layer on top -- they tell you when to act and how to approach, but only matter when the fit foundation is already there.

Present the foundation first, then the layers. Let the user react to each section before moving on.

**Account fit signals (foundation)** tell you whether a company matches your criteria. These tend to be relatively stable -- they don't change week to week. They answer: should we be talking to this company at all? Start with whatever qualification criteria the user shared during the interview -- those are their account fit signals, and every other signal in the map sits on top of them.

**Person fit signals (foundation)** tell you whether an individual is the right contact to pursue. Job function, seniority, profile language, career trajectory, role in the buying process. Also relatively stable. They answer: is this someone who would play a meaningful role in a deal? If the user has contact qualification criteria, those belong here.

**Timing signals (layer)** tell you when to prioritize an account or person that already fits. This is where it gets dynamic: a company switching away from a competitor creates a window. A burst of hiring suggests investment. A regulatory change shifts priorities. These signals decay -- the window to act is finite. A timing signal without fit is noise.

**Engagement signals (layer)** tell you how to approach. What content did they engage with? What pages did they visit? What language are they using? These shape the message and the angle, not the decision of whether to pursue.

Some signals map to more than one category. Include them in each relevant category with a note about the dual role. A leadership change is both a person fit signal and a timing signal -- list it in both places with the reasoning for each.

For each signal in the map, include:

- **What the signal is** -- described concretely in the user's language
- **Source** -- first-party, second-party, or third-party, and specifically where the data comes from (their CRM, their website analytics, Clay, LinkedIn, etc.). This should come from the interview -- the user told you where they get each signal. If they didn't, flag it as a gap in the context check rather than assuming. Don't write "third-party -- LinkedIn, job postings" if the user never confirmed that's where they actually monitor it.
- **Why it matters for this business** -- grounded in what came up during the interview, not generic reasoning. If the user said "when we see a company drop our main competitor, that's our best close rate by far," that reasoning belongs here.
- **Elephant or ant** -- does this signal, on its own, meaningfully change how they'd prioritize or engage? Or is it useful context that contributes in combination with other signals?
- **Timing durability** -- how quickly does this signal lose relevance? Time-sensitive signals (competitive displacement, leadership change, funding round) need fast routing. Stable signals (industry, company size, tech stack) are background context. In-between signals (hiring surge, content engagement patterns) have a window of weeks to months.

### Handle signals that don't fit cleanly

Some signals won't drop neatly into one category. That's fine:

- **Signals that span categories** -- include in each with reasoning for why it matters in that context. Don't force a single classification.
- **Negative signals** -- things that indicate the opposite of fit or interest (unsubscribes, departures of champions, declining engagement). Include these. A map that only captures positive signals misses half the picture.
- **Signals the user wants but doesn't have yet** -- if the interview surfaced signals they'd love to track but don't currently have access to, include them in a separate section. This becomes a roadmap for what tools or data sources to invest in.
- **Groups of equivalent signals** -- sometimes a set of signals (e.g., several third-party triggers) are roughly equal in importance. Don't force a ranking that doesn't exist. If the interview surfaced that a group of signals is interchangeable -- the user's insight was about how to respond differently to each one, not which one matters more -- present them as a group and focus on what distinguishes the engagement approach for each trigger.
- **Compound signals** -- combinations of signals that are more actionable together than individually. When building compound signals, every component must be an actual observable event. "Time passing" is not a signal -- a compound like "lost deal + 12 months later" should be "lost deal + something changes at the company (new leadership, competitor raises prices, they start hiring again)." The trigger to re-engage should be something happening, not a calendar reminder.

### Crystallization pass

After all categories are built and the user has reacted to each, present the complete map and run a structured validation pass. This is active friction designed to surface problems before the map is finalized.

Ask specifically:
- "Which signals are you least confident about? Where are we guessing about importance because we haven't tested it?"
- "Are there signals you track today that we didn't include? Anything we missed?"
- "Look at the elephant signals -- are these really the ones that change your behavior on their own, or are any of them more like strong ants?"
- "For the time-sensitive signals, does the durability feel right? Anything we're treating as urgent that's actually more of a slow burn, or vice versa?"
- "If you handed this map to a rep tomorrow, what would confuse them or lead them in the wrong direction?"

This pass often catches: signals the user inflated during the conversation because they were excited about them (not everything can be an elephant), first-party signals that got less attention than they deserve, and timing durability that's off because the user was thinking about a specific recent example rather than the pattern.

Take the feedback seriously and revise before finalizing.

### Wrap up

Once the crystallization pass is clean, set expectations:

- This map is a starting point, not a finished product. Recommend they test individual signals by running focused plays -- pick a signal, build a small cohort, test whether the signal actually predicts interest.
- Signals that perform well in plays can be weighted more heavily. Signals that don't predict outcomes should be downgraded or dropped.
- Revisit the map after a few rounds of plays, once they have data on which signals actually drove engagement and pipeline.
- The map should evolve as they add tools, channels, or data sources. New signals get added; underperforming ones get removed.

## Handling Missing Context

**Ask first** when the gap would change the map structure -- if you don't know whether the user cares about person fit signals at all (maybe they only do outbound to accounts, not people), you can't organize the categories correctly.

**Flag as you go** when the gap is about a specific signal -- if you're not sure whether a signal is an elephant or an ant, present your best read and let the user correct you.

**Skip and note** when the gap is about something the user hasn't tested yet -- if they mentioned a signal but couldn't say whether it actually predicts outcomes, capture it as a hypothesis rather than a confirmed signal.

## Output Document Structure

### 1. Context and framing

What the user sells, who they sell to, and how their sales motion works. An overview of their signal landscape: where their data comes from, what's strong, and what's thin. How to use this document.

Written in the user's voice and language. Long enough to make the map interpretable by someone who wasn't in the conversation, short enough that people read it.

### 2. Signal map

Organized hierarchically: account fit and person fit signals form the foundation, followed by timing signals that layer on top, then engagement signals that shape approach. Each signal includes what it is, source (confirmed by the user, not assumed), why it matters, elephant/ant, and timing durability. Signals that span categories appear in each relevant section. Groups of equivalent signals can be presented together with notes on how the engagement approach differs for each trigger.

Within each section, lead with the elephants -- the signals that matter most. Include compound signals where combinations are more actionable than individual signals.

### 3. Signals wanted but not yet available

Signals the user would like to track but doesn't currently have access to. Each includes what tool or data source would be needed and why it would be valuable. This section is a roadmap for future investment, not a gap to feel bad about.

### 4. Open questions

Signals where importance is uncertain. Hypotheses that need testing. Areas where the user was unsure. Patterns that seemed meaningful during the interview but haven't been validated against real outcomes. Suggested experiments to run.

## Notes for the Generator

**The user has already done the hard part.** The interview surfaced their signals and their reasoning. This stage organizes it. Be efficient. Build, present, adjust.

**Present things to react to.** A draft signal entry with a clear point of view is better than an open-ended question. "Based on our conversation, pricing page visits seem like an elephant for you -- it was the signal you kept coming back to, and you said it's the strongest predictor of a real evaluation. I'd put it at the top of your timing signals. Sound right?" gives the user something to agree with or push back on.

**Use the language from the interview.** The user described their signals in their own words. Keep that language. If they said "when someone hits our pricing page twice in a week, that's basically a hand raise," don't rewrite it as "repeated pricing page engagement indicates active evaluation behavior."

**Don't inflate the map.** Include signals that actually came up and matter. A map with 40 signals where half are ants the user barely mentioned is less useful than a map with 15 signals the user has conviction in. Quality over completeness.

**The elephant/ant distinction is the most valuable part.** Helping the user honestly assess which signals actually change their behavior vs. which ones are nice-to-know is where the generator adds the most value. Push on this. Most signals are ants.

**Timing durability shapes operationalization.** A signal map without durability is missing the "so what." Time-sensitive signals need to route to reps quickly (alerts, daily digest). Stable signals inform account profiles and can be checked periodically. In-between signals work well in a weekly digest. The durability dimension tells the user how to actually act on each signal.

**The map should be self-contained.** Someone reading it shouldn't need to know how it was built. No references to phases, the interview process, or the skill. It should read like a signal map a smart strategist built, not like the output of a tool.
