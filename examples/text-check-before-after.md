# Sample output: ai-text-critic-en

A fictional resume summary, two bullets and a cover-letter opening, checked by the skill and
rewritten. The scores come from the skill's checker script, run on both versions.

## Before: AI trace 68/100

> Results-driven and detail-oriented Executive Assistant with a proven track record of providing
> world-class support in fast-paced environments. Passionate about leveraging cutting-edge AI
> tools to streamline workflows and drive impact.
>
> - Responsible for managing complex calendars for senior executives.
> - Spearheaded initiatives to foster seamless communication across teams.
>
> I am writing to express my interest in the Executive Assistant role. I am confident that my
> unique blend of skills makes me a perfect fit — and I would welcome the opportunity to discuss
> how I can add value.

**What the checker found:** 18 issues.

| Group | Found |
|---|---|
| Corporate buzzwords | results-driven, detail-oriented, world-class, leveraging, streamline, drive impact, spearheaded |
| Resume clichés | proven track record, passionate about, responsible for |
| Cover-letter clichés | I am writing to express my interest, unique blend of, perfect fit, I would welcome the opportunity |
| Generic AI words | seamless, foster, cutting-edge AI |
| Punctuation | 1 em dash |

## After: AI trace 6/100

> Executive Assistant to the founder of a 40-person fintech startup in New York. Runs investor
> meetings and the monthly board update. Uses Claude daily to draft and check documents.
>
> - Run calendars for the founder and two VPs across New York and London.
> - Prepare the monthly board update: metrics from finance, notes from each team lead, one deck.
>
> Your team is building AI for legal work. That is the work I want to do next. I support a
> founder who signs a dozen vendor contracts a quarter, and I already use AI to flag issues
> before they reach counsel.

**What changed:** adjectives replaced with facts (who, how many, where). Every bullet starts
with a verb and names its scope. The letter opens with the company, not with "I am writing".
The skill never invents numbers: when the facts are missing, it marks the spot and asks.
