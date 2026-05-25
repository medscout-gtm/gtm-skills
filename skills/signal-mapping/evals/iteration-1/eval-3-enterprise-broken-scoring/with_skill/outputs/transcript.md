# Eval 3 Transcript: Enterprise with Broken Scoring Model

**Simulated user:** Director of Revenue Operations at a cybersecurity company selling to Fortune 500. Full tech stack (Salesforce, 6sense, ZoomInfo, Outreach, LinkedIn Sales Nav). Built a scoring model a year ago that reps ignore. Knows which signals reps actually act on vs. what the model says.

---

**User:** We need to rethink our signal strategy. We sell cybersecurity software to enterprise companies -- Fortune 500 mostly. We've got a full tech stack: Salesforce, 6sense, ZoomInfo, Outreach, LinkedIn Sales Nav. We built a lead scoring model about a year ago but nobody trusts the scores. Reps ignore them. We've got tons of data but I don't think we're using it well. I think we need to go back to basics and figure out which signals actually matter before we try to score anything.

**Interviewer:** That makes sense -- stepping back to figure out which signals actually matter before putting numbers on them. That's exactly what we're going to do here.

We're going to build a signal map for your business. Not a scoring model -- a clear picture of which signals matter for you, what each one tells you, and how important it is. Here's how we'll work through it:

First, I'll get some quick context on your company and sales motion -- what you sell, who you sell to, and what makes a company or a person worth pursuing. That's the foundation, because every signal we map builds on top of it.

Then we'll walk through your signals -- what you're tracking now, what you have access to but might not be using well, and what you wish you had. I'll float some ideas along the way. We'll figure out what each signal actually tells you and how important it is.

Finally, we'll take everything and organize it into a document you can actually use -- each signal sorted by what it tells you, with your reasoning for why it matters, how important it is, and how quickly it goes stale.

The scoring model you built is useful input here. It tells us which signals your team has already identified and put weight behind -- we'll use that as a starting point rather than ignoring it. The conversation will naturally surface where the model lines up with reality and where it doesn't.

So let's start with the basics. Tell me about what you sell and who you're selling to. You said Fortune 500 -- what does your cybersecurity product do, and what's the typical buyer look like?

**User:** We sell an endpoint detection and response platform -- EDR. Think CrowdStrike, SentinelOne, that tier. Our sweet spot is large enterprises with complex environments -- lots of endpoints, distributed workforce, heavy compliance requirements. Fortune 500 is the core, but we also work with large government agencies and some of the bigger healthcare systems.

The typical deal involves the CISO's office, but the technical evaluation runs through the security operations team -- the SOC analysts, the threat hunters. Deals are usually $500K to $2M ARR, 6-9 month sales cycles. We're displacing incumbents in most cases, not selling into greenfield.

**Interviewer:** That's helpful context. Displacement selling into complex enterprises with long cycles -- that shapes a lot of what matters signal-wise.

Before we get into the signals themselves, I want to understand what makes a company a good fit for you. You mentioned Fortune 500, complex environments, heavy compliance. What are the actual criteria your team uses to say "this is our kind of account"? Is that formalized somewhere, or more intuitive?

**User:** It's semi-formalized. We have a target account list in Salesforce -- about 800 accounts. The criteria we used to build it were: Fortune 1000 by revenue, minimum 10,000 employees, in verticals where compliance pressure is high -- financial services, healthcare, critical infrastructure, government. We also filtered for companies we know are running legacy EDR -- older versions of McAfee, Symantec, Trend Micro -- because that's our displacement play.

But honestly, the TAL has gotten stale. We built it 18 months ago and haven't refreshed it. Some of those companies have already switched to CrowdStrike or are mid-contract with someone else. The reps who do well tend to have their own mental filters on top of the official list.

**Interviewer:** Got it. So the formal criteria are size, industry vertical, and legacy EDR stack -- but the reps who perform well are layering their own judgment on top. We'll come back to what those informal filters look like.

What about on the person side -- what makes someone the right contact to pursue at one of these accounts? Is it always the CISO, or is it more nuanced than that?

**User:** More nuanced. The CISO is the economic buyer, but they rarely take a cold meeting. The people who actually drive evaluations are usually one level down -- VP of Security Operations, Director of Threat Intelligence, Head of SOC. Sometimes it's a senior security architect who gets tasked with running a competitive bake-off.

The real signal on person fit is whether they have budget authority or evaluation authority. A SOC analyst can champion us internally, but if they can't get the eval approved, it stalls. We've learned the hard way that the title matters less than where they sit in the decision chain.

The other thing -- and this is something the scoring model completely misses -- is community presence. The CISO community is tight. If someone is active in ISSA, ISACA, or one of the regional CISO roundtables, that tells us two things: they're influential in their peer group, and we can potentially reach them through community channels rather than cold outreach.

**Interviewer:** That's a good distinction -- evaluation authority vs. budget authority, and community presence as a separate dimension. The model probably can't see community involvement at all, which might be part of why it feels disconnected from what reps experience.

OK, so we have the fit foundation: on the account side, it's large enterprises in compliance-heavy verticals running legacy EDR. On the person side, it's people with evaluation or budget authority in the security org, with community presence as a bonus indicator.

Let's talk about the scoring model you built. Walk me through what's in it -- which signals did you include, and how did you weight them?

**User:** Sure. The model runs in Salesforce with data flowing in from 6sense and ZoomInfo. Here's roughly what it scores on:

Account-level: company size by employee count (20 points max), industry match to our target verticals (15 points), 6sense intent topics -- we're tracking about 30 topics related to EDR, endpoint security, SIEM, threat detection (25 points max based on topic volume and surge), and 6sense buying stage (10 points for "decision" or "purchase" stage).

Contact-level: title match to our persona list (15 points), email engagement with our marketing campaigns (10 points), and website visits to specific pages (5 points).

Total possible is 100. We set "MQL" at 60 points and "SQL" at 80.

**Interviewer:** Thanks -- that's detailed. So the model is heavily weighted toward intent data from 6sense (35 points between topics and buying stage) and firmographic fit (35 points for size and industry). Contact-level signals are 30 points total, mostly title match and email engagement.

When you say reps don't trust the scores -- can you be more specific about what they're seeing? Is it that high-scoring accounts go nowhere, or that deals close from low-scoring accounts, or both?

**User:** Both, but the false positives are the bigger problem. We'll have an account light up at 85 points -- it's the right size, right industry, 6sense shows intent surge across multiple topics -- and the rep reaches out and gets nothing. Crickets. Happens over and over.

Meanwhile, a rep closes a $1.2M deal with a company that scored 45 because the company wasn't in our target verticals (it was a logistics company, which isn't on our list) and 6sense never showed meaningful intent. What actually happened was the rep got a warm intro from a CISO at a different company who said "hey, my friend just took the CISO job at this logistics firm and they're ripping out Symantec." That deal closed in 4 months.

The reps see enough of those stories that they just stopped looking at the scores. And honestly, I don't blame them. The model is measuring availability of data, not actual buying intent.

**Interviewer:** "Measuring availability of data, not actual buying intent" -- that's a sharp diagnosis. And the logistics deal is a perfect example of why: the signals that actually predicted that deal -- warm intro from a peer, new CISO, competitive displacement of a legacy vendor -- are things the scoring model can't see.

I want to dig into that gap. You've got a model that says "this is what matters" and you've got reps who act on something different. Let's talk about what reps actually act on. When your top performers decide to prioritize an account or a contact, what's driving that decision? Not what the score says -- what actually makes them pick up the phone?

**User:** I've watched this closely because it's been driving me crazy. The top reps act on four things consistently:

One -- warm intros from the CISO community. If someone in their network says "talk to this person," they drop everything. Those deals have our highest win rate by far. It's not even close.

Two -- breach announcements. When a target company has a public breach or a significant security incident, that creates a window. Not because we're ambulance chasing -- because the aftermath of a breach almost always triggers a full vendor review. The CISO is under pressure, the board is asking questions, and suddenly there's budget that didn't exist before.

Three -- compliance deadline pressure. SOX audits, GDPR reviews, CMMC deadlines for defense contractors, HIPAA audits for healthcare. When a company is coming up on a compliance deadline and their current tooling has gaps, they move fast.

Four -- security leadership hiring. When a company posts for a new CISO or Head of Security, it usually means the current approach isn't working. And the new person coming in wants to make their mark -- they're evaluating everything fresh in the first 90 days.

**Interviewer:** Those are four very different kinds of signals, and none of them are well-represented in the current model. Let me make sure I understand what each one is actually telling you.

The warm intros -- where does that intelligence come from? Is that purely rep relationships, or do you have any systematic way to track community connections?

**User:** It's almost entirely ad hoc. Some reps are better networked in the CISO community than others. We don't have a system for it. I've thought about trying to map our CISOs' networks in LinkedIn Sales Nav, but the CISO community operates a lot through private channels -- Signal groups, invite-only dinners, closed Slack communities. You can't really scrape it.

The closest thing we have to a system is that our CEO and our field CTO both speak at CISO roundtables, and they'll sometimes come back with "I just talked to the CISO at [company] and they're looking." But that's maybe 2-3 leads a quarter. The reps who generate warm intros do it through their own relationships.

**Interviewer:** So the data source for warm intros is essentially human intelligence -- rep networks, executive relationships, event conversations. It's your strongest signal but also your least scalable and least systematizable one.

What about the breach announcements? Where do reps pick those up?

**User:** A mix. Some reps have Google Alerts set up. A few follow security news feeds -- Krebs on Security, The Record, BleepingComputer. We also get some of it from 6sense -- when a company has a breach, their intent data sometimes spikes because they're suddenly researching everything. But the 6sense spike is too slow. By the time it shows up as an intent surge, the news has been out for a week and every cybersecurity vendor has already called.

The reps who move fastest on breaches are the ones who see the news first and reach out within 24-48 hours. Not with a pitch -- with a "we've been in situations like this, happy to share what we've seen work" angle.

**Interviewer:** Speed matters a lot on that one. So the signal itself -- breach announcement -- is public information, but the competitive advantage is in response time and approach. The 6sense intent spike is a lagging indicator of the same event.

For compliance deadlines -- where does that information come from? Are reps tracking audit cycles, or is it more about knowing the regulatory calendar?

**User:** It's a combination. Some of it is the regulatory calendar -- SOX deadlines are predictable, CMMC has published milestones, HIPAA audits follow known cycles. That part is knowable. The harder part is knowing which companies are actually under pressure. A SOX audit date doesn't tell you whether the company's current EDR is compliant or not.

What we've found is that the reps who do this well combine the regulatory calendar with conversations. They'll reach out to contacts at a company 3-4 months before a known compliance deadline and ask about their readiness. That's where they learn whether there's actual pain. So the compliance calendar is really a timing signal that tells reps when to start the conversation, and then the conversation itself is the qualifying event.

Right now that knowledge lives in individual reps' heads. There's no system tracking compliance deadlines against target accounts.

**Interviewer:** That's interesting because the compliance calendar is actually systematizable -- the dates are knowable -- but the qualifying layer on top of it requires human judgment. Those are two different pieces you could operationalize differently.

And the security leadership hiring -- where are reps seeing those job postings?

**User:** LinkedIn mostly. A few use ZoomInfo alerts for leadership changes. The ZoomInfo data is hit or miss -- sometimes we find out about a new CISO months after they started, which is too late. The reps who are effective with this signal check LinkedIn manually for their target accounts, which obviously doesn't scale.

**Interviewer:** OK. Let me step back and lay out what I'm seeing so far, because I think the gap between the model and reality is becoming clear.

Your scoring model is built primarily on firmographic fit and 6sense intent data. Those are real signals, but they're table stakes -- every competitor in your space has the same 6sense data and the same firmographic filters. The model can't see the signals your best reps actually act on: community relationships, breach events with fast response, compliance timing, and leadership transitions.

And critically -- the four signals reps trust all share a pattern. They're not about whether a company looks like it might buy someday. They're about whether something specific has changed that creates an opening right now. They're timing and engagement signals that layer on top of fit.

Does that match how you see it?

**User:** Yeah, that's exactly right. The model tells us who could buy. The reps are looking for who's ready to buy right now and why. The model is all fit with some vague intent sprinkled on top. The reps are working on timing and approach.

I'd push back on one thing though -- I don't think 6sense intent is completely useless. I think the problem is how we're using it. When I look at our closed-won deals, intent data does show up -- but it shows up as a confirming signal, not a leading one. If we already know a company is in play for other reasons and then we see intent activity, that's validating. But using intent as the primary trigger generates too much noise.

**Interviewer:** That's a really useful distinction. Intent as confirmation vs. intent as trigger -- those are two completely different roles for the same data. And the scoring model treats it as a trigger (25 points just for having intent activity), when its actual value might be as a supporting signal that validates what you're already seeing from other sources.

Let me ask about that -- when intent data does confirm something, what does that look like concretely? Is it the topic match, the surge, the buying stage indicator, or something else?

**User:** It's the surge relative to baseline, combined with topic specificity. If a company is surging on "endpoint detection and response" and "EDR migration," that's meaningful. If they're surging on generic "cybersecurity" topics, that could mean anything -- they might be hiring, they might be dealing with an incident, they might be doing annual training. The model doesn't distinguish between those.

Also, the buying stage indicator from 6sense has been unreliable for us. It says "decision stage" and the company has never heard of us. I think it's calibrated for a different sales motion -- maybe mid-market SaaS where the buying stage maps to website activity. For enterprise cybersecurity with 6-9 month cycles, the stages don't line up.

**Interviewer:** Good -- so the intent data has a useful version (specific topic surge as confirmation) and a less useful version (generic topics or buying stage as a trigger). That's worth capturing in the map because it changes how you'd operationalize it.

I want to make sure we're not missing other signals you have access to. You mentioned Outreach -- are you getting any signal from outreach engagement? Reply rates, bounce patterns, anything like that?

**User:** Yeah, actually. We see some useful stuff in Outreach. Reply sentiment is interesting -- we started tagging replies as positive, negative, or neutral, and the accounts where we get positive or even "not now but check back" replies convert at a much higher rate than accounts where we just get silence or hard nos.

The other one from Outreach is multi-threading signal. When more than one person at an account is responding to sequences, that tells us there's organizational awareness. Even if the responses are just "pass me to the right person," the fact that multiple people are engaging means our name is circulating internally.

**Interviewer:** Both of those are strong first-party signals, and they're hard for competitors to see. Reply sentiment as a timing signal -- someone who says "not now" is telling you they're aware of you and have some interest but the timing isn't right. That's a signal to come back, not to give up. And multi-threading as an engagement signal -- organizational awareness is a real indicator that something is happening internally.

Are you doing anything with your website beyond the 5 points in the scoring model?

**User:** Honestly, not much. We track visits in HubSpot (we use it for marketing alongside Salesforce for sales) but the website traffic from Fortune 500 companies is mostly anonymous. We can't tie it to specific people very often. We see the account-level visits through 6sense reverse IP, but it's noisy. A lot of our target accounts have tens of thousands of employees -- a website visit from Citigroup doesn't tell you much.

The one exception is our competitive comparison pages. We have pages like "Us vs. CrowdStrike" and "Us vs. SentinelOne." When a known account hits one of those pages, that's actually a strong signal because it means someone is actively comparing. But it happens rarely enough that we've never operationalized it.

**Interviewer:** Competitive comparison page visits from a known account -- that could be a meaningful signal precisely because it's rare. When it does happen, it's telling you someone is in active evaluation. Combined with other signals -- like if you know there's a new CISO and then see a comparison page visit -- that becomes very high conviction.

Let me ask about something we haven't touched on. You mentioned you're mostly doing displacement selling. Do you have any visibility into when competitor contracts are up for renewal? Or when companies are running RFPs in your space?

**User:** We don't have systematic visibility into contract renewal timing. Sometimes reps pick it up in conversations -- a contact will mention "we're locked in with CrowdStrike for another 18 months" -- and ideally that goes into Salesforce, but the data quality is spotty.

RFPs we occasionally see through government procurement channels -- those are public for federal and state agencies. We have someone who monitors SAM.gov and a couple of state procurement portals for cybersecurity-related RFPs. That's actually a decent signal for the government vertical specifically, but it doesn't help with commercial enterprises.

**Interviewer:** So government RFP monitoring is a signal you have for one segment, and competitor contract intel exists but lives in rep notes inconsistently. Both worth capturing.

Let me make sure we're not leaving anything on the table. Are there signals you wish you had but don't? Things you'd track if you could?

**User:** Two big ones. First, I wish we had better visibility into when companies are actually running security tool evaluations. Not the vague "intent surge" from 6sense -- I mean actually knowing "Company X just kicked off an EDR evaluation." Sometimes we find out after the fact that we weren't even invited to an RFP because we didn't know it was happening. G2 and Gartner Peer Insights sometimes show review activity that could indicate evaluation, but we don't pay for those data feeds.

Second, I wish we could track CISO network connections at scale. Our best signal is warm intros, but we can't systematically map who knows who in the CISO community. If we could see that our field CTO spoke on a panel with the CISO at a target account, or that one of our customer CISOs is in the same ISSA chapter as a prospect CISO, we could manufacture more of those warm intro opportunities. Right now it's serendipity.

**Interviewer:** Both of those are real gaps. The evaluation visibility one is interesting because it sits between what 6sense promises and what you actually need -- you want a specific, confirmed evaluation event, not a probabilistic "buying stage."

OK, I want to start pulling this together. We've covered a lot of ground. Let me check whether we're missing any major areas before we move to weighting.

You've got strong first-party signals from Outreach (reply sentiment, multi-threading) and a potentially useful but underutilized website signal (competitive comparison page visits). Your third-party signals are the ones reps actually trust: breach announcements, compliance calendar, security leadership changes. Your highest-conviction signal is warm intros from community relationships, which is human intelligence rather than tool-generated data. And you have 6sense intent data that has a role as a confirming signal but not as a primary trigger.

On the second-party side -- do you have any partner relationships, channel partners, MSSPs, or integration partners who generate leads or share intelligence?

**User:** We have a few MSSP partnerships, but they're mostly for delivery, not lead gen. We do get occasional referrals from our technology partners -- we integrate with Splunk, Palo Alto, and a few SIEM vendors -- and sometimes their field teams will flag opportunities. But it's sporadic and there's no formal data sharing.

Actually, the one second-party source I should mention is our customer advisory board. We have a CAB with about 20 CISOs from our customer base. They sometimes refer us into their networks -- that's actually a subset of the "warm intro" signal we talked about. It's not a data feed, but it's a repeatable motion when we activate it.

**Interviewer:** Got it. The CAB referrals are essentially a more structured version of the warm intro signal, with the advantage that you can proactively activate them rather than waiting for them to happen organically.

Let's move into weighting. I want to help you separate the signals that genuinely move the needle from the ones that add useful context but wouldn't change what you do on their own. The way to think about it: if a signal were the only thing you knew about an account, would it change what you do?

Let me start with the obvious one. Warm intros from the CISO community -- if you get a warm intro to a company you've never heard of, do you act on it regardless of anything else?

**User:** Absolutely. Doesn't matter if they're on the TAL, doesn't matter what 6sense says, doesn't matter what vertical. If a trusted CISO says "talk to this person," we're calling. It's our highest win rate signal by a factor of 3x.

**Interviewer:** So warm intros are clearly in the "changes your behavior on their own" category. What about breach announcements? If you see a public breach at a company that's on your TAL, does that alone trigger action?

**User:** Yes, with a caveat. We act on it, but the approach is different. We're not cold-calling to pitch. We're reaching out with a value-add angle. And not every breach means they need a new EDR -- sometimes the breach happened despite good tooling, and they're not switching. But the breach creates the opening, and we reach out fast. So yes, it changes our behavior on its own.

**Interviewer:** And compliance deadline pressure -- same question. If you know a target account has a SOX audit in 3 months, does that alone trigger outreach?

**User:** It triggers a specific kind of outreach -- a compliance-angle conversation to assess readiness. It doesn't trigger a product pitch. So it changes what we do, but more in terms of timing and approach than "drop everything." I'd say it's a strong signal but not quite at the level of a warm intro or a breach. It's more of a "this is the right window to have a specific conversation."

**Interviewer:** That's a useful distinction. It's strong enough to drive action, but the action is a qualifying conversation rather than full pursuit. What about security leadership hiring?

**User:** Similar to compliance deadlines. New CISO posting triggers outreach, but it's a longer play. You're not reaching the new person for months -- you're watching for when they start, then reaching out in their first 90 days. So it changes our behavior, but on a longer timeline.

I'd put warm intros and breach announcements in the top tier -- those change what we do immediately. Compliance deadlines and leadership changes are the second tier -- they change what we do, but on a longer timeline and with a different approach.

**Interviewer:** I actually want to resist forcing those into a strict hierarchy. It sounds like warm intros and breaches are immediate action triggers, and compliance deadlines and leadership changes are windows that shape timing. They're doing different jobs rather than being better or worse versions of the same thing. The right question might be less "which is more important" and more "how does the engagement approach differ for each one."

Does that match how you think about it?

**User:** Yeah, that's actually more accurate. They're not competing with each other. A warm intro means "call today." A breach means "reach out this week with a specific angle." A compliance deadline means "start a conversation 3-4 months out." A leadership change means "watch and engage when they're settled in." Different signals, different playbooks, different timelines. Ranking them against each other doesn't really help -- we need all four.

**Interviewer:** Good. Now let's talk about the supporting signals -- the ones that add context but wouldn't drive action on their own. Where does 6sense intent data fall when you think about it honestly?

**User:** It's context. It's the thing that makes me feel better about a decision I've already made for other reasons. If we know a company just had a breach and 6sense shows intent activity in EDR topics, that's validating. But if 6sense shows intent activity and I have no other signal? I've learned not to act on that alone. So it's supporting context, not an action trigger.

**Interviewer:** And the firmographic signals in your model -- company size, industry match?

**User:** Those are foundational. They determine whether a company is in our addressable market at all. They're not timing signals -- they don't tell us when to act. They're the baseline filter. Every other signal we've talked about only matters if the company meets those criteria first. Well, except for warm intros -- we'd pursue a warm intro even outside our standard ICP, as we saw with the logistics deal.

**Interviewer:** Right. So firmographic fit is the foundation the other signals sit on top of, but your single strongest signal -- warm intros -- can override it. That's worth documenting because it means the foundation has an exception clause.

Let me bring in the compound signal idea. You mentioned that intent data is most useful when it confirms another signal. Are there other combinations where two signals together are more meaningful than either one alone?

**User:** Definitely. The most powerful compound we've seen: new CISO at a target account + they post for additional security hires within 60 days. That combination tells us the new leader is building their team, which means they have budget and mandate to make changes. It's much stronger than either signal alone.

Another one: competitive comparison page visit + the account is in an active sequence in Outreach. If someone at a company we're already working is actively comparing us to competitors on our site, that's a sign our outreach is landing and they're in evaluation mode.

And honestly, the breach + specific intent surge compound I mentioned earlier. Breach alone triggers outreach. Breach plus intent surge in EDR-specific topics means they're not just dealing with the incident -- they're actively researching alternatives.

**Interviewer:** Those are good compound signals, and they share an important feature: every component is an observable event. New CISO is an event. Hiring activity is an event. The comparison page visit is an event. None of them are just "time passed" -- they're all things you can actually detect.

Let me ask about timing durability for the key signals. How quickly do each of these go stale?

Breach announcements -- what's the window?

**User:** Two weeks to a month for the initial outreach window. After that, every vendor has called and they're either already in an evaluation process or they've decided not to change anything. You have to move fast.

**Interviewer:** Compliance deadlines?

**User:** The useful window is 3-6 months before the deadline. Once they're inside of 30 days, they've either solved it or they're in emergency mode and not evaluating new platforms.

**Interviewer:** Leadership changes?

**User:** 30-90 days after the person starts. Before they start, they're not reachable. After 90 days, they've usually made their vendor decisions or gotten locked into what was already there.

**Interviewer:** And warm intros?

**User:** Those are interesting because the intro itself is time-sensitive -- you need to follow up within a few days or it goes cold. But the underlying relationship signal is durable. If you know a CISO is connected to your network, that's persistent -- you're waiting for the right moment to activate it.

**Interviewer:** That's a helpful distinction. The relationship is stable context; the intro event is highly time-sensitive. They're actually two different signals in terms of how you operationalize them.

OK. I think we have enough to start building your signal map. Let me tell you what I'm working with, and then we'll build it out section by section.

What's clear: Your fit foundation is well-defined -- large enterprises in compliance-heavy verticals, ideally running legacy EDR, with contacts who have evaluation or budget authority in the security org. Your strongest action-driving signals are warm intros, breach events, compliance timing, and leadership transitions -- these are timing and approach signals that layer on top of fit. 6sense intent data has a role as a confirming signal, not a primary trigger. You have underused first-party signals in Outreach (reply sentiment, multi-threading) and website (competitive comparison pages). Firmographic fit is the foundation.

What's a bit fuzzy: I'm not sure how you want to handle the warm intro signal structurally, since it's part human intelligence, part CAB referral, and part executive event connections -- those might be different signals with different operationalization paths. I'm also not sure whether the government RFP monitoring signal is important enough to include or whether it's a niche edge case.

On the fuzzy items -- do you see the warm intro variants as one signal with different sources, or genuinely different signals?

**User:** I'd treat them as one signal category -- "community-sourced referrals" or something -- with different channels. The underlying dynamic is the same: a trusted peer recommends us. Whether that comes from a rep's personal network, the CAB, or our field CTO's speaking engagements, the signal value is the same. The operationalization differs, but the signal is one thing.

**Interviewer:** Makes sense. And the government RFP monitoring?

**User:** Include it, but it's segment-specific. It's a strong signal for our government vertical and doesn't apply anywhere else. Just call that out.

**Interviewer:** Good. Let me build the signal map now. I'll start with the fit foundation and work up through timing and engagement.

**Account fit signals -- the foundation.** These determine whether a company is in your addressable market.

First, company size -- minimum 10,000 employees, Fortune 1000 by revenue. Source: ZoomInfo firmographic data in Salesforce. This is your baseline filter. It's stable -- doesn't change frequently. It's foundational context, not an action trigger.

Second, industry vertical -- financial services, healthcare, critical infrastructure, government. Source: ZoomInfo industry classification. Same role: baseline filter, stable, foundational.

Third, legacy EDR presence -- companies running older EDR platforms (McAfee, Symantec, Trend Micro). Source: ZoomInfo technographic data, supplemented by rep intelligence from conversations. This is where fit starts to get interesting because it's also a precondition for your displacement play. It's more of a needle-mover than the other fit signals because it tells you not just "could they buy" but "do they have a reason to switch." I'd call this the strongest account fit signal.

A note on these: your warm intro signal can override this entire foundation. The logistics deal proved that. Worth documenting that the fit criteria are strong defaults, not hard gates.

How does that land?

**User:** That's right. I'd add one thing -- the TAL staleness problem. The legacy EDR data from ZoomInfo isn't always current. Companies switch and we don't always know. That's a data quality issue, not a signal mapping issue, but it's worth flagging because stale technographic data is one reason our model produces false positives.

**Interviewer:** Good flag. I'll note that as a data quality consideration under legacy EDR presence.

**Person fit signals -- the other half of the foundation.**

First, role and seniority -- VP of Security Operations, Director of Threat Intelligence, Head of SOC, senior security architects. Source: LinkedIn Sales Nav and ZoomInfo. The title is a starting point but evaluation authority matters more than exact title.

Second, decision chain position -- whether the contact has evaluation authority, budget authority, or both. Source: primarily rep judgment from conversations, sometimes visible from org charts in ZoomInfo. This is the harder signal to detect but the more important one.

Third, CISO community presence -- active in ISSA, ISACA, regional CISO roundtables. Source: LinkedIn, event attendee lists, rep knowledge. This tells you two things: the person is influential in their peer group, and they're reachable through community channels. It's both a person fit signal and an engagement approach signal.

How does that look?

**User:** Solid. The decision chain position one is the hardest to operationalize because it's almost always qualitative judgment from reps, not data from a tool. But it's the most important person fit signal we have. I wouldn't change anything.

**Interviewer:** Now the timing signals -- these layer on top of fit and tell you when to prioritize an account.

First: community-sourced referrals -- warm intros from CISO networks, CAB members, executive connections. Source: rep relationships, customer advisory board, field CTO speaking engagements. This is your single highest-conviction signal. On its own, it changes what you do immediately. Durability: the underlying relationship is persistent, but the intro event requires follow-up within days. Three channels feed this signal but the dynamic is the same.

Second: breach announcements at target accounts. Source: security news feeds (Krebs on Security, The Record), Google Alerts, sometimes lagging confirmation via 6sense intent surge. Action window: 2-4 weeks from public announcement. On its own, triggers immediate outreach with a value-add angle, not a pitch. Speed of response is the competitive edge.

Third: compliance deadline pressure. Source: regulatory calendar (SOX, CMMC, HIPAA, GDPR) combined with rep conversations to assess actual readiness. The calendar is systematizable; the qualification requires human judgment. Action window: 3-6 months before the deadline. Triggers a compliance-angle qualifying conversation.

Fourth: security leadership transitions -- new CISO or Head of Security appointment. Source: LinkedIn (manual monitoring), ZoomInfo alerts (inconsistent). Action window: 30-90 days after the new leader starts. Triggers a longer-term engagement plan targeting the new leader's evaluation window.

I'm presenting these four as the core timing signals without forcing a strict ranking. They do different jobs: warm intros and breaches are immediate action triggers; compliance deadlines and leadership changes shape timing over a longer window. The engagement approach differs for each one. Does that work, or do you want them ranked?

**User:** That works. Ranking them against each other would be artificial. They're all high-value, but they trigger different playbooks on different timelines. I like that you're distinguishing the engagement approach rather than just stacking them.

**Interviewer:** Good. Now the confirming and supporting signals:

6sense intent data -- specific topic surge (EDR, EDR migration topics) as confirmation of other signals. Source: 6sense integrated with Salesforce. This is supporting context, not an action trigger. When it confirms a signal you're already seeing (breach + intent surge, leadership change + intent surge), it increases conviction. Generic topic activity or the buying stage indicator is not reliable for your sales motion. Durability: intent surges typically last 2-4 weeks.

Outreach reply sentiment -- positive or "not now" replies to outreach sequences. Source: Outreach, with manual tagging. Timing signal -- a "not now" reply is a signal to come back, not to give up. Accounts with any positive sentiment convert at higher rates. Durability: a few weeks to months depending on the response.

Outreach multi-threading -- multiple contacts at an account engaging with sequences. Source: Outreach activity data. This tells you your name is circulating internally. It's an engagement signal that suggests organizational awareness. Durability: weeks.

Competitive comparison page visits from known accounts. Source: website analytics (HubSpot) cross-referenced with 6sense reverse IP lookup. Rare but high signal -- someone is actively comparing you to competitors. Durability: days to a week. Strongest as a compound signal: comparison page visit + active outreach sequence.

Government RFP postings in cybersecurity categories. Source: SAM.gov and state procurement portals. Segment-specific to government vertical only. Strong timing signal when it appears. Durability: follows RFP timeline, usually weeks to months.

Marketing email engagement patterns. Source: HubSpot/marketing automation. Weak individually but repeat clicks on specific topics can indicate problem awareness. Supporting context, not an action driver. Durability: patterns emerge over weeks.

**User:** That's a solid supporting layer. I'd push back slightly on marketing email engagement -- I almost wouldn't include it. It's so noisy for us at the enterprise level that nobody looks at it. The scoring model gives it 10 points and I think that's 10 points of noise.

**Interviewer:** Fair. I'll include it with a note that it's currently generating more noise than signal for enterprise accounts and may not be worth tracking until you have better attribution. Or I can drop it entirely -- your call.

**User:** Drop it. The map should reflect what actually matters, not what we technically have. We can always add it back if we find a use for it.

**Interviewer:** Dropped. Let me cover the compound signals before we finalize:

Compound one: new CISO + security hiring burst within 60 days. Tells you the new leader has budget and mandate. Both are observable events. Stronger than either signal alone.

Compound two: competitive comparison page visit + account is in active Outreach sequence. Someone you're actively working is evaluating you against competitors. Both are observable events.

Compound three: breach announcement + specific EDR intent surge. They're not just dealing with the incident -- they're actively researching alternatives. Both are observable events.

**User:** Those are right. I'd add one more: warm intro + legacy EDR presence. When a community referral points us at a company we already know is running Symantec or McAfee, that's our best possible situation. The intro opens the door and the displacement angle gives us a sharp wedge.

**Interviewer:** Good addition. That's fit plus timing compounding -- the displacement angle is the message, and the intro is the access.

Now the signals you want but don't have yet:

First: evaluation event detection -- knowing when a target account kicks off a formal EDR evaluation. The gap between what 6sense promises here and what you actually need. Potential sources: G2 Buyer Intent, Gartner Peer Insights data feeds, TrustRadius intent data.

Second: CISO network mapping at scale -- systematically tracking who in your network is connected to CISOs at target accounts. Would let you manufacture warm intros rather than relying on serendipity. Potential approach: structured LinkedIn Sales Nav analysis, CRM relationship mapping, event attendee cross-referencing.

**User:** Yes on both. The evaluation detection one is the bigger gap because it's the difference between showing up during an evaluation and showing up after one is over. The network mapping is a force multiplier on our best signal.

**Interviewer:** OK. Let me run the crystallization pass before we finalize.

First question: which signals are you least confident about? Where are we guessing about importance because we haven't tested it?

**User:** Competitive comparison page visits. It makes intuitive sense that it's a high signal, but it happens so rarely that I don't actually have enough data to know if it predicts anything. We've had maybe 10-15 known-account visits to comparison pages in the last year. I believe it matters but I haven't proven it.

Also the Outreach multi-threading signal. We just started tracking it, so I'm going by gut more than data.

**Interviewer:** Good. I'll note both as hypotheses that need validation rather than confirmed signals.

Second: look at the signals we tagged as big action-drivers -- community referrals, breach announcements, compliance deadlines, leadership transitions. Are those really the ones that change your behavior on their own? Or is any of them more like a strong supporting signal that we promoted because it sounded good during the conversation?

**User:** Honestly? Compliance deadlines might be a half-step below the other three. I said earlier that it triggers a qualifying conversation, not full pursuit. The compliance calendar tells you when to start a conversation. But whether that conversation leads to a deal depends entirely on what you learn in the conversation. So it's an action trigger, but a weaker one. Breach events and warm intros are unambiguous -- when those happen, we move. Compliance deadlines are more like "this is a good time to knock on the door and see if anyone's home."

**Interviewer:** That's an honest assessment. I'll adjust compliance deadlines to note that it's a strong timing signal that triggers qualifying outreach, but the qualifying conversation itself is where conviction forms. It's a "check the door" signal, not a "go in" signal. Different from breach events and warm intros, which are "go in" signals.

Third: for the time-sensitive signals, does the durability feel right? Anything we're treating as urgent that's actually more of a slow burn, or vice versa?

**User:** Leadership transitions might actually be a longer burn than I said. I said 30-90 days after they start, but honestly, some new CISOs take 6 months to get to vendor evaluation. The 30-90 day window is when you make initial contact, but the actual evaluation decision might not happen for 6 months. So the initial outreach window is 30-90 days, but the full opportunity window is more like 3-6 months.

**Interviewer:** Noted. I'll update the durability to distinguish between the initial contact window (30-90 days) and the full evaluation opportunity window (3-6 months).

Fourth: anything we missed entirely?

**User:** One thing. Negative signals -- we didn't talk about those. When a champion leaves a target account, that's a negative timing signal. The deal might be dead. Conversely, when a champion leaves and goes to a new company, that's a positive timing signal for the new company -- they might bring us with them. We've had that happen twice this year. Champion departure and arrival are different signals going in different directions.

**Interviewer:** That's a real gap in what we covered. Champion departure from a target account is a negative signal: the deal dynamics just changed, possibly for the worse. Champion arrival at a new account is a positive timing signal: they already know your product and might pull you in. I'll add both.

Where does that data come from?

**User:** LinkedIn Sales Nav alerts for the contacts we're tracking. It's one of the few things Sales Nav does really well -- the job change notifications are fairly real-time.

**Interviewer:** Good. Last question: if you handed this map to a rep tomorrow, what would confuse them or lead them in the wrong direction?

**User:** They might not understand the distinction between "this is a signal to act on" vs. "this is context that validates a decision." The whole reason the scoring model failed is that everything was treated the same -- 10 points here, 15 points there. If the map doesn't make it dead obvious which signals mean "do something now" vs. "this is background info," reps will blend them together the same way the score did.

**Interviewer:** That's the most important design point for the document. The hierarchy needs to be stark: fit is the foundation, timing signals drive action, supporting signals validate. And within timing, the action triggers (warm intros, breach events) are different from the timing windows (compliance deadlines, leadership transitions) in terms of what you do and how fast you do it.

I'll revise the map with all of this feedback -- the compliance deadline adjustment, the leadership transition durability update, the champion departure/arrival signals, the hypothesis flags on comparison page visits and multi-threading, and the emphasis on making action vs. context visually clear.

The map is a starting point. I'd recommend testing individual signals by picking one, building a small cohort, and seeing whether the signal actually predicts outcomes. Signals that perform well get more weight in whatever system you build next. Signals that don't predict outcomes get downgraded. Revisit the map after a few rounds of that, once you have data.

And the signals you want but don't have -- evaluation event detection and CISO network mapping -- those become your investment roadmap. If you can crack either one, you're adding signal your competitors can't see.

**User:** This is exactly what I needed. A clear picture of what actually matters before we try to put numbers on anything again. The next scoring model -- if we build one -- should be built on this foundation, not the other way around.
