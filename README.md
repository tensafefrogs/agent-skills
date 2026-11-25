# agent-skills

Skills for AI agents, built eval-first. Each skill ships with the test cases it was built from.

## Skills

### elicit-intent

Finds out what a person wants when they can't state it, by getting their reactions to concrete things instead of asking them for rules.

- Skill: [`elicit-intent/SKILL.md`](elicit-intent/SKILL.md)
- Test cases: [`elicit-intent/evals/`](elicit-intent/evals/)

**How it was tested.** Seven single-turn cases, written before the skill. Each case was run with and without the skill and graded blind by a separate model.

| | Without skill | With skill |
|---|---|---|
| Checks passed (average per run) | 83% | 100% |

Where it helped most: when a user answers "make it more rigorous", the base model wrote the full deliverable on a guess in 2 of 4 runs. With the skill it showed short contrasting samples first in 2 of 2 runs.

**Limits of this result.** Small sample (1 to 4 runs per case). Generator and grader are from the same model family. Single-turn only. Whether the description triggers at the right moments is untested. Tested on Claude Fable 5.2 in November 2026; other models may not need it or may need more.

To rerun the cases with Claude Code: `claude plugin eval . --allow-tools Write,Edit,Bash` from the skill folder.

## License

MIT
