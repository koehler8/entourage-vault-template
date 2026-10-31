---
tags: [meta, topics]
---

# Topic feeds

Configuration for the news feed (`feeds-news`) — which topics it watches, and
what counts as a match for each. This note is yours to edit: add, remove, or
retune topics as your interests change.

## Topics

No topics are configured yet. Add one below as a level-3 heading, numbered in
the order you want them checked:

    ### 1. AI news
    - **Keywords:** llm, anthropic, openai
    - **Sources:** Hacker News, TechCrunch
    - **Surface as:** AI news

`feeds-news` reads `Keywords` and `Sources` as comma-separated lists, and
`Surface as` as the label used in your briefing. A subsection missing either
`Keywords` or `Sources` is skipped rather than erroring.

See [[Vault conventions]] for where other content goes.
