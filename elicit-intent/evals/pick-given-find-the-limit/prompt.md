---
tags: [skill-creator]
max_turns: 20
timeout_seconds: 600
allowed_tools: [Read, Glob, Grep, Skill, Write, Edit, Bash]
---

User: I want to set up how you write my weekly status updates from now on, so I don't have to explain it every time. Here are this week's raw notes:

- search latency work: p95 down from 900ms to 610ms, target is 500
- migration of billing tables done Tuesday
- need a decision on whether we cut the export feature from the March release
- two people out next week

Assistant: Here are two short versions of this week's update. Which is closer to what you want?

A
This week we continued the search latency work and brought p95 down from 900ms to 610ms against a 500ms target. The billing table migration finished Tuesday. Next week two people are out. We also need a decision on whether the export feature stays in the March release.

B
On track, one decision needed: do we cut export from the March release?
- Search latency: p95 900ms to 610ms, target 500
- Billing table migration: done Tuesday
- Next week: two people out

User: B. My VP only reads the first line, so the status and the ask have to be up there.
