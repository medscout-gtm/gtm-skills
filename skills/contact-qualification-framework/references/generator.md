# Contact Qualification Framework Generator

## What This Does

This is the final stage of building a contact qualification framework. The user has been through an interview where they reviewed real profiles, reacted to what they saw, and surfaced the signals that drive their judgment about which contacts are worth pursuing. Now you're turning that into a usable document.

The output is one document: a contact qualification framework that captures how to classify what someone does (persona classification) and how to assess whether they're relevant to the user's sales process (fit assessment). It includes the reasoning behind each signal — not just what to look for, but why it matters.

## How This Stage Works

### Start with a context check

Before building anything, review what came out of the interview. Then tell the user what you're working with:

- **What's clear.** The patterns, signals, and criteria you feel confident about. Be specific — "Your yes decisions consistently came down to whether someone owns the function vs. executes within it" is useful. "I have a good sense of your criteria" is not.
- **What's fuzzy.** Where the interview left gaps — signals the user mentioned but didn't fully explain, contradictions between profiles, areas where the user wasn't sure. Distinguish between things that need to be resolved before you can build (blockers) and things you can flag as assumptions (refinements).

Ask about the blockers. For refinements, tell the user: "I think I can work with what I have here — I'll flag my assumptions as we go and you can correct me."

This checkpoint should be brief. A few sentences on what's clear, a few on what's fuzzy, and targeted questions for the blockers. Don't turn it into a lengthy assessment.

### Build section by section

Once blockers are resolved, start generating the framework. Present each section to the user and let them react before moving on.

The default structure is two layers:

**Layer 1: Persona classification.** How to categorize what someone actually does — the job functions that matter for the user's buying process, with guidance on how to tell them apart when titles are ambiguous.

**Layer 2: Fit assessment.** For each relevant persona (or across all personas if the criteria are universal), the signals that determine whether someone is worth pursuing. Organized by fit tier — who to prioritize, who to keep but not lead with, who to skip.

If the user's thinking doesn't split cleanly into these two layers — if classification and fit are deeply intertwined in how they evaluate people — adapt. Ask: "Does it make sense to separate the 'what do they do' question from the 'are they a fit' question, or do you think about those together?" Respect their answer.

**For persona classification, cover:**

- **Clean functional categories** — discrete labels that are easy to understand and sort people into, not conversational descriptors. During the interview, someone might say "anyone on the commercial side who's managing reps" — that's a descriptor. The generator's job is to help them turn that into a clean category like "Sales Leadership" with a "use when" definition underneath. Each category should have: a clear label, a brief definition of when someone belongs in it, and example titles that commonly map to it.
- **How to classify when titles are ambiguous** — the signals that distinguish one function from another when the title doesn't make it obvious. This is where the profile review reactions are most valuable — the user probably encountered ambiguous titles and talked through how they'd classify them. Turn those into explicit classification rules.
- **Where titles mislead** — specific title patterns the user identified as unreliable, and what to look at instead. Industry-specific title conventions often matter here — in some industries, "Director" means functional ownership; in others, it means senior IC. Watch for over-generalizations in classification rules: "multiple people sharing the same title means it's an IC role" may be true for territory-level titles, but at enterprise companies with multiple divisions, several people holding "VP of Sales" means divisional structure, not title inflation. Each of those VPs may genuinely own their division's sales function.

**For fit assessment, cover holistic attributes — not discrete signals checked in isolation:**

Fit assessment is a holistic judgment. The user isn't checking individual boxes; they're reading across multiple dimensions (scope, function ownership, company size context, career trajectory, how someone describes their work) to form an overall picture. The framework should capture the attributes that matter and the signals within each, but make clear that the assessment weighs them together.

For each attribute that matters:

- **What to look for** — the attribute and its key signals, described concretely. Not "strong career trajectory" in the abstract, but what that looks like for this user's contacts — "promoted within the same company" or "moved from IC to leadership" or whatever their profile reviews surfaced.
- **Why it matters** — the connection between this attribute and whether the contact is worth pursuing. Ground this in what came up during the interview — specific profiles, the user's reasoning, patterns they articulated. Not generic logic.
- **What good looks like** — specific enough that two different people would read the same profile and reach the same conclusion.
- **What would be concerning** — the flip side. What suggests this attribute isn't present, or points in the wrong direction. Include the gray areas.
- **How critical is this attribute** — is this an elephant or an ant? An elephant is an attribute that changes the decision on its own — if it's present (or absent), that dominates regardless of other signals. An ant is a contributing factor that matters in aggregate but doesn't drive the verdict alone. Help the user distinguish between the two. Most contact-level attributes are ants, but some may be elephants for their business.

Don't present the entire framework at once. Work through persona classification, get the user's reaction, adjust. Then work through fit assessment. If something in classification triggers a realization that changes the fit criteria, incorporate it.

### Handle fit tiers

The fit tiers should map to action — what a rep or the team would actually do with each tier:

- **Best Fit** — worth prioritizing in outreach. This person would drive or shape an evaluation — they'd recommend a tool, run the evaluation, or make the purchase decision. A rep should invest real time here.
- **Good Fit** — belongs in the CRM and worth engaging, but not the person you'd lead with. A rep should know they exist and include them in multi-threading, but wouldn't prioritize them over a best-fit contact.
- **Unsure / Needs Review** — genuinely ambiguous. Not enough information to make a confident call, or the signals are contradictory. This is the human-in-the-loop tier — these contacts get flagged for manual review rather than auto-sorted. Important: this is not a safe middle ground. If there's enough evidence to form a view, form one. Unsure should be used sparingly, for cases where critical information is genuinely missing.
- **Poor Fit** — not relevant to the sales process. This tier should be narrow. It's for people clearly outside the commercial org (clinical, R&D, legal, IT), or at a company large enough that their level genuinely wouldn't participate in tool evaluation (a territory rep at a company with 500 reps). Be careful not to draw this line too aggressively — at smaller companies, ICs and junior commercial titles may be Good Fit contacts because the entire team needs to be bought in for a deal to happen. Company size determines where the Poor Fit line sits.

Four tiers is a good default — most teams need at least three confidence levels plus a review category. If the user's mental model has different tiers or different definitions, use theirs. The point is that tiers map to concrete actions, not just quality scores.

### Handle segmentation

If the interview surfaced segmentation needs (different criteria for different company sizes, verticals, etc.), build the variants:

- Start with the base framework that applies everywhere.
- Then describe what changes for each segment — which signals shift, which thresholds move, which new signals appear.
- Keep the variants focused on what actually differs. If 80% of the criteria are the same across segments, don't duplicate the whole framework — describe the base and then the deltas.

### Write the context that frames the framework

The framework isn't just criteria and signals. It includes written context that makes it usable:

- **What the profile reviews revealed** — the themes, patterns, and surprises that emerged. What the user assumed at the start vs. what they discovered by looking at real profiles. If there were contradictions or surprises, name them and explain how the framework handles them.
- **How the criteria connect** — which signals tend to go together, which ones compensate for each other, where the framework gives clear answers vs. where it requires judgment.
- **How to use the framework** — specific to this user's context. What tools they're using, what the workflow looks like, how the criteria translate into their actual process.

This context should read like the user wrote it — grounded in their language and their examples, not in abstract qualification theory.

### Crystallization pass

After all sections are built and the user has reacted to each, present the complete framework and run a structured validation pass. This is not just "does this look right?" — it's active friction designed to surface problems before the framework is finalized.

Ask specifically:
- "Where would this framework give you the wrong answer? Think of a specific contact or company where these criteria would misclassify someone."
- "Which criteria are you least confident in? Where are we making assumptions that haven't been tested against enough profiles?"
- "If a rep used this tomorrow without your judgment behind it, where would they get tripped up?"
- "Are there edge cases we discussed but didn't capture in the criteria — situations where the rule breaks?"

This pass often catches over-generalizations that slipped through: tier definitions that are too aggressive, classification rules that don't account for divisional structures at large companies, or signals that seemed universal but actually only applied to one company or segment. Take the feedback seriously and revise the framework before finalizing.

### Wrap up

Once the crystallization pass is clean, set expectations for iteration. This framework is a strong starting point. Recommend they:
- Run additional profile review sessions to sharpen the criteria, especially across account profiles they didn't cover in the initial interview
- If they operationalize this as an automated process, keep human review on the output — the automation handles obvious bad fits, but good-fit and borderline contacts should get a manual check
- Use disagreements between the automated output and human judgment as feedback to update the criteria
- Revisit this framework after a few rounds of real-world use, once they have examples of where it worked and where it didn't

## Handling Missing Context

Not every gap needs to be filled before you start building. Use judgment:

**Ask first** when the gap would change the structure of the framework — if you don't know whether persona classification matters for this user (maybe all their contacts are in one function and the only question is fit), you can't organize the layers correctly.

**Flag as you go** when the gap is about a specific signal — if you're not sure whether "career trajectory" is a hard filter or a contributing factor, present your best read and let the user correct you.

**Skip and note** when the gap is about something the user hasn't figured out yet — if the profile review surfaced a pattern but the user couldn't explain why it matters, capture it as an open question rather than forcing an answer.

If you find yourself asking more than two or three questions before you can start building, something is off. Lean toward building with flagged assumptions rather than interrogating.

## Output Document Structure

### 1. Context and framing

What the profile reviews revealed — the patterns and reasoning that drive the framework. How the user thinks about contact qualification. How to use this document. Written in the user's voice and language.

Length: a few paragraphs. Long enough to make the framework interpretable by someone who wasn't in the conversation, short enough that people read it.

### 2. Persona classification

The job functions that matter, how to identify them, and where titles mislead. This section answers: "What does this person actually do?"

If the user only cares about one function (e.g., they only sell to sales leaders), this section might be brief — just the signals that distinguish their target function from adjacent ones. If they care about multiple functions, each gets its own entry with classification guidance.

### 3. Fit assessment

The holistic attributes that determine fit tier, applied universally across all personas. Classification tells you what someone does; fit assessment tells you whether they're relevant to the sales process — and that question is the same regardless of function. The job function from classification is an input to the fit judgment (a "Director of Sales" who owns the function is assessed differently than a "Territory Manager"), but the assessment criteria themselves don't change per persona.

Each attribute covers: what to look for, why it matters, what good looks like, what's concerning, and how critical it is (elephant vs. ant).

Order attributes by criticality — lead with the elephants that most strongly drive the tier decision.

If there are segmentation variants, describe the base criteria first, then the deltas per segment.

### 4. Open questions

Things the framework doesn't resolve. Signals that came up but aren't solid enough to be criteria yet. Areas where the user was uncertain. Patterns that need more profile reviews to validate. Suggested next steps for testing.

This section matters. A framework that claims certainty everywhere is less useful than one that's honest about what's known and what's still being figured out.

## Notes for the Generator

**The user has already done the hard part.** The interview extracted their judgment. This stage is about organizing it, not uncovering new information. Be efficient. Build, present, adjust.

**Present things to react to.** A draft signal with a clear point of view is better than an open-ended question. "Based on the profiles you reviewed, it seems like career trajectory is more of a tiebreaker than a primary filter for you — you noticed it but it never drove a yes/no on its own. I'd put it in the framework as a contributing factor, not a hard signal. Sound right?" gives the user something to agree with, push back on, or refine.

**Use the language from the interview.** The user described their criteria in their own words during the profile reviews. Use that language in the framework. If they said "this person sounds like they're running the show," don't rewrite it as "demonstrates functional ownership with executive-level scope."

**Ground signals in real profiles.** The interview gave you concrete examples. Reference them: "This signal would have caught the person at Company X you flagged as misleading — their title looked senior but their experience was all IC roles." This connects abstract criteria to the user's actual reactions and makes the framework feel tested.

**Don't over-specify.** Name the key signals — the things someone would actually check when looking at a profile. Don't list every possible data point. The user's profile reviews are your best guide for what's realistic to look for in practice.

**The elephant/ant distinction matters.** Helping the user distinguish attributes that change the decision on their own (elephants) from attributes that contribute in aggregate (ants) is often the most useful part of this stage. Most contact-level attributes are ants — judgment calls that matter in combination. But some might be elephants for their business. Push the user to be clear about which is which.

**Build in consistency checks.** When the framework is assembled, the reasoning for each attribute should support the tier it's associated with. If an attribute is listed under "signals of best fit" but the reasoning describes something that's more of a contributing factor, something's off. Flag these and resolve them with the user.

**Probe every rule for where it breaks.** When you draft a classification rule or fit criterion, ask yourself: "Where would this give the wrong answer?" If you can think of a case where the rule fails, build in the exception before presenting it. The most common failure is over-generalizing from a small number of profiles — a pattern that held at one company or one segment may not hold broadly. Name the scope of each rule and flag where it hasn't been tested.

**The framework should be self-contained.** Someone reading it shouldn't need to know how it was built. No references to phases, the interview process, or the skill. It should read like a contact qualification framework, not like the output of a tool.
