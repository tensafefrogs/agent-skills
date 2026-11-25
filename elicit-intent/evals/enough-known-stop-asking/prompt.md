---
tags: [skill-creator]
max_turns: 20
timeout_seconds: 600
allowed_tools: [Read, Glob, Grep, Skill, Write, Edit, Bash]
---

User: I want to set up how you write my weekly status updates from now on, so I don't have to explain it every time.

Assistant: Here are two short versions of last week's update. Which is closer to what you want? [version A: a narrative paragraph. version B: a first line with overall status and the decision needed, then three bullets.]

User: B. My VP only reads the first line, so the status and the ask have to be up there.

Assistant: So the rule is: line one carries the status and the ask, because your VP stops there. What about a week with no ask? Do you still want a slot for it on line one, or just the status?

User: Just status then. Don't invent an ask.

Assistant: Got it. And when the news is bad, a slipped date for example, does it still go on line one, or do you soften the lead?

User: Still line one, plainly. She hates being surprised later. Ok here are this week's notes, go ahead:

- checkout redesign launch slips from Dec 8 to Dec 15, QA found a tax rounding bug
- need her to approve one contractor for two weeks to hold the new date
- mobile crash rate down from 1.2% to 0.7%
- holiday on-call rota is set
