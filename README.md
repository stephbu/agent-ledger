# agent-ledger

A daily and weekly newspaper for technically informed readers building
or using AI agents.

## Prompts

The shared research prompt is maintained separately in
`agent-ledger-sources.md`; the living shortlist of remembered sources
is `agent-ledger-source-registry.md`. Use the research prompt together
with one edition prompt:

- `agent-ledger-daily-edition.md` for the daily edition.
- `agent-ledger-weekend-edition.md` for the weekly review.

When using a model that cannot read the repository files directly,
include the full text of the shared research prompt and the chosen
edition prompt in the same request. If possible, also provide the
source registry as a discovery aid. The research prompt covers subject
scope, source discovery, curation, and verification; the edition prompt
controls the reporting window, selection, and presentation.
