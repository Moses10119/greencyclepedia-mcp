# Changelog

What each version of the Greencyclepedia MCP server gives an agent. Newest first. Dates are the day the version went live; the tool counts are the counts of the server's own `tools/list`.

## 1.11.0 (2026-11-24)

Conditions release. `search_conditions` now returns 45 conditions graded on an evidence ladder, and 8 risk topics answered as risk research with the reviews behind them and no grade. Some risk topics list trials testing a cannabis medicine, kept apart from the research. Never doses.

## 1.10.0 (2026-11-14)

23 tools. An agent gains:

- `check_claim`: give one sentence you were told and get it checked against the records: the compounds and conditions it names, the studies held by kind (trial, human, animal, cell, review) and one plain level. Never true or false.
- Questions we could not answer: when a call finds nothing, the server counts the missed name (never who asked), so the records grow where agents ask.
- View links: every compound and terpene record carries a `view` object with its 3D page, a still picture and a drawing, ready to show a person.
- A least studied ranking, the resource `greencyclepedia://rankings/least-studied`: the body parts, where cannabinoid targets are found, with the least research.
- Version 1.9.0 changes (below) are part of this release.

## 1.9.0 (2026-11-14)

22 tools. The first call for a plain question is now `ask_greencyclepedia`, and it is listed first. An agent gains:

- Eight more tools: `studies_by_region` (how much research exists per body part), `market_signals` (facts from cannabis industry news, each with its number and a publisher link), `list_new_studies` (the newest PubMed studies, sorted by kind of evidence), `list_topics_without_home` (new research topics no condition covers yet), `list_brain_regions` and `get_brain_region` (measured PET binding and RNA levels per brain region), `get_pain_pathway` (the pain route from the fingertip to the brain) and `lookup_many` (up to 20 names in one call).
- Two prompts: `where_in_the_brain` and `follow_the_nerve`.
- German and everyday names find the right record in every tool.
- A missing or vague argument gets a helpful answer with a note, not an error.
- Every study carries how it was done: a quality label, a band and the rule that set it.
- Every link a result gives is tagged with the tool that produced it.
- The old name of the first tool keeps answering, so assistants that stored it still work.

## 1.2.0 (2026-10-24)

14 tools. An agent gains:

- `ask_greencyclepedia`: one argument, a plain question such as "does CBD help epilepsy", answered only from the records it names.
- `cite_as` on every result: the title, the address, the licence and the date it was read.
- Four prompts that name the tools to call and how to cite: `evidence_summary_for_condition`, `compare_two_compounds`, `where_a_compound_acts` and `whats_new_this_week`.
- A resource with this week's dataset changes.

## 1.1.1 (2026-10-22)

The server card names this repository as the source of the listing.

## 1.1.0 (2026-10-22)

13 tools, resources and prompts. An agent gains:

- `search` and `fetch`, the pair ChatGPT apps and deep research expect.
- `compare_compounds` (two to four compounds side by side), `find_studies` (the PubMed studies behind a finding) and `cite` (a ready citation with BibTeX).
- Open access from browsers and a server card for directories.

## 1.0.0 (2026-10-16)

The first release: nine read-only tools over the open Greencyclepedia data files, at `https://greencyclepedia.com/mcp`, Streamable HTTP, no key.
