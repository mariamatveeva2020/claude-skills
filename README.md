# Claude Skills

Custom skills for Claude Code that I built and use in my own work. This page describes what each
one does and shows sample output. The source is private.

| Skill | What it does |
|---|---|
| **ai-lawyer-ny** | Reads a contract with New York State and New York City rules in mind. Flags risky clauses, checks section and exhibit references, suggests better wording and produces a plain-English HTML report with color-coded risk levels. |
| **ai-yurist** | The same review for contracts under Russian law. *Yurist* is Russian for "lawyer". The report is written in the user's language. |
| **ai-text-critic-en** | Checks whether an English text reads as AI-written and rewrites it in plain American business English. Built for resumes, cover letters and LinkedIn posts. Includes a Python script that scores the text. |
| **ai-text-critic** | The same check for Russian texts. |

## Sample output

### Contract review (ai-lawyer-ny)

A review of a fictional freelance services agreement. Three risks, one broken exhibit reference,
three proposed rewrites and a numbering check.

[Open the full report](https://mariamatveeva2020.github.io/claude-skills/examples/contract-review-sample.html)

[![Contract review sample](examples/contract-review-sample.png)](https://mariamatveeva2020.github.io/claude-skills/examples/contract-review-sample.html)

### Text check (ai-text-critic-en)

A fictional resume summary and cover-letter opening, before and after: AI trace 68/100 → 6/100.

[See the before and after](examples/text-check-before-after.md)

## Note on the legal skills

The contract skills prepare facts for a conversation with a lawyer. They do not give legal advice,
do not say whether to sign, and do not replace a licensed attorney.

## Want to see one in action?

I'm happy to walk through a skill live. Reach out on LinkedIn.
