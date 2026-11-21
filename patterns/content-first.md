# Content first, machinery behind

**The pattern:** The content area holds only the content: findings, the views that show them, the controls that change them, and the caveats a reader needs to read them correctly. Everything about the page itself goes behind it, below the content and outside the tabs. That includes the source file, the schema, which recipe produced it, how the AI fits in, and links to the next demo or to GitHub.

| In the content area | Behind the page |
|---|---|
| Findings, charts, tables | Source file and schema |
| Controls that change what the reader sees (rules, scenarios) | Which recipes the page draws on, and the AI's role in them |
| Caveats about the data: "seat share is not cost" | Notes about the page: "this demo does not…" |
| Plain names: "Defaults," "Sections flagged" | Build terms: "recipe defaults," "Recipe 16's flags" |
| | Links to the source repository and to the next demo |

**Why it matters:** The audience is cabinet members, deans, and registrars, not developers. A Source tab placed beside the views reads as a fourth view and costs a click that teaches nothing. Meta-commentary mixed into findings makes the reader sort two kinds of text at once. Once the machinery moves behind the page, the page reads as an answer instead of a demonstration.

**It doesn't hide anything.** Moving the machinery behind the page is not [suppression](anti-suppression.md). The source stays one click away, every view still draws from it, and a link to `#source` opens it. The test is placement: a reader who wants the machinery can reach it, and a reader who doesn't never has to step over it.

**The test for a sentence:** Would it still be true and useful if this were a real institution's dashboard and not a Cookbook demo? If yes, it's content. If it only makes sense because this is a demo, it goes behind.

**Caveats stay with the data.** A limit on what the numbers can say belongs next to the numbers. "Seat share is not cost" stays in the content area. "This page does not recommend Sunset; in the recipe an AI drafts that" goes behind.

**In practice:** Each demo has its analysis tabs, then a "Behind the page" section with a short note on where the page comes from and a collapsible **Source file** drawer holding the YAML editor and schema. The footer links to `#source`, and loading the page with `#source` in the address opens the drawer.

**Worked examples:** [RCU Portfolio Explorer](https://rjoy28.github.io/higher-ed-ai-cookbook/demos/rcu-portfolio/), [RCU Program Economics](https://rjoy28.github.io/higher-ed-ai-cookbook/demos/rcu-economics/), and [RCU IT Service Health](https://rjoy28.github.io/higher-ed-ai-cookbook/demos/rcu-service-health/). In the last one the pre-flight check stays in the content area: data quality is a finding about the export, and a real service desk would want to see it.

*Status: draft, in the Test Kitchen.*
