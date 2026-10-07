# The Agent Ledger — Source Registry

A maintained shortlist for discovering reporting leads. Inclusion is
not endorsement: verify each story against original evidence before
using it. Review entries periodically and update their status and
last-reviewed date.

## Registry

| Source | URL | Topics | Type | Use | Status | Last reviewed |
| --- | --- | --- | --- | --- | --- | --- |
| Hacker News | https://news.ycombinator.com/ | Models, agents, tooling | Discovery | Surface community discussion and emerging stories; never treat votes or comments as proof. | Candidate | Not yet reviewed |
| arXiv — Artificial Intelligence | https://arxiv.org/list/cs.AI/recent | Agents, AI research | Research index | Find recent papers; check the paper itself and note review status. | Candidate | Not yet reviewed |
| arXiv — Computation and Language | https://arxiv.org/list/cs.CL/recent | Models, language research | Research index | Find recent language-model papers; check the paper itself and note review status. | Candidate | Not yet reviewed |
| Hugging Face Papers | https://huggingface.co/papers | Models, research | Research discovery | Discover papers and discussion; verify claims in the paper and linked artifacts. | Candidate | Not yet reviewed |
| OpenReview | https://openreview.net/ | Models, agents, evaluation | Research and review platform | Find submissions and peer-review context; distinguish submissions from accepted work. | Candidate | Not yet reviewed |
| Simon Willison | https://simonwillison.net/ | Models, agents, tools | Independent technical analysis | Find hands-on analysis, release coverage, and links to primary sources. | Candidate | Not yet reviewed |
| Latent Space | https://www.latent.space/ | Models, agents, infrastructure | Technical reporting and interviews | Discover practitioner coverage and interviews; corroborate factual claims independently. | Candidate | Not yet reviewed |
| The Batch | https://www.deeplearning.ai/the-batch/ | AI research and industry | Newsletter and reporting | Discover research and industry developments; follow links to original sources. | Candidate | Not yet reviewed |

Add specific official blogs, documentation, release-note pages, code
repositories, and independent evaluations as they prove useful. Prefer
canonical topic or release pages over ephemeral links.

## Machine-Readable Access

Some pages render poorly or return nothing when fetched as plain pages
(observed in a dry run). Use these endpoints when the main URL fails,
and record new working endpoints here.

| Source | Endpoint | Notes |
| --- | --- | --- |
| Hacker News | https://hn.algolia.com/api/v1/search?tags=front_page&hitsPerPage=40 | JSON front page with points, comment counts, and ISO `created_at` timestamps. The `news.ycombinator.com/front` page returned only a title. |
| Hugging Face Papers | https://huggingface.co/api/daily_papers?limit=15 | JSON with abstracts, upvotes, `publishedAt`, and linked repositories. The `/papers` page returned only a subscribe prompt. |
| Latent Space | Not yet found | Home and archive pages returned only a title. Try the Substack feed (`/feed`) before relying on it. |
| Mistral docs | Not yet found | Model documentation page returned only a title; verify new Mistral releases through another official page. |

If no working endpoint exists, say the source could not be checked and
do not report claims that rest on it alone.

## Adding or Reviewing an Entry

Use one row per source. Record:

- **Source:** publication, project, organization, or feed name.
- **URL:** canonical source page, not an individual story.
- **Topics:** relevant Agent Ledger coverage areas.
- **Type:** for example, primary source, research index, independent
  evaluation, reporting, newsletter, or discovery forum.
- **Use:** what it reliably helps discover or verify, plus any
  limitation editors should remember.
- **Status:** Candidate, Active, Watch, or Retired.
- **Last reviewed:** date the URL and usefulness were last checked;
  use `Not yet reviewed` for an unverified entry.

## Status Guide

- **Candidate:** newly discovered; assess during two edition cycles.
- **Active:** repeatedly surfaces relevant, verifiable leads and adds
  useful coverage.
- **Watch:** occasionally useful, but inconsistent or overlapping.
- **Retired:** broken, inactive, low-signal, or no longer useful. Keep
  the record so the source is not accidentally re-added without reason.

When reviewing, check that the page still works, the source still
covers its recorded topics, and recent leads have been useful. Promote,
demote, correct, or retire the entry and update its review date.
