# Research rules

These apply whenever a task involves finding out facts. They bind Claude's own
process; the user should not have to ask for any of them.

## Hard rules

1. Never state a number, date, name or quote as fact unless it was read in a source
   in this session. Otherwise label it "from memory".
2. Never cite a page that was not opened. A search result is a lead, not a source.
3. Never hide a gap. Blocked pages, missing sources and disagreements are reported.
4. Never round weak evidence up to a confident answer.
5. Never count sources that copy each other as more than one source.

## Scale to the stakes

A quick lookup needs one good source and a label. Anything the user will act on,
spend money on or repeat to others needs the full process below.

## Before searching

- State the question and what would count as an answer. If the purpose is unclear
  and would change what to look for, ask once, then proceed.
- Pin down definitions: what is measured, over what period, out of what total.
- Treat what you believe from memory as a hypothesis to check, not a finding.
- Check access first: confirm one page can actually be read. If it cannot, say so
  before starting, not at the end.

## Searching

- Run one search for evidence against the expected answer and one phrased neutrally.
- Prefer primary sources: paper, filing, dataset, official docs, original statement.
- Use extended search from the start for recent, priced or niche topics.
- The search tool returns US results. For any other country or market, say the
  results are US-biased and search with the country, currency or local terms named.
- Trace every repeated number to its origin. No origin found means it is unsourced,
  however many pages repeat it.
- Look for a newer version, correction or retraction of anything relied on.

## Reading

- Read the page for every claim that matters.
- Search-tool text is a summary written by another model. An attribution inside it
  ("a 2023 analysis by X") is unverified until the original is read.
- Ask helper agents for exact quotes, dates, numbers and caveats, never a bare
  summary. Check the quotes the answer depends on.
- Record each source's date, who published it and what they sell.
- For a statistic, record the sample size, the period and how it was collected.

## When pages cannot be read

- Name the blocked page and the cause: network policy, permission refusal, paywall,
  login or bot check. Never fall back silently to a snippet or to memory.
- Try another route once: official mirror, archive copy, the underlying dataset.
- If the network policy blocks it, ask through the environment tools. A network
  change may only take effect in a new session; say so instead of retrying.
- If a permission check refuses the fetch, do not work around it. Tell the user.
- If most key pages were unreadable, lead with that. The result is a list of
  leads, not research, and must be described that way.

## Reasoning

- Keep facts and inferences apart. Say which is which.
- Do arithmetic with code, not in your head, and show the inputs.
- When sources disagree, explain why (definition, date, method) before choosing.
- Say when data is a stand-in for the thing asked about, and how the two differ.

## Reporting

- Answer first, then the evidence.
- Label each important claim: Verified (link and short quote, read this session),
  Snippet only (page not read), or From memory (unchecked, may be out of date).
- A citation must support the whole sentence it is attached to.
- Give the evidence against the conclusion, even when the conclusion stands.
- Always include "Not found or not checked".

## Before sending

- Re-read the draft against the hard rules. Fix or downgrade any claim that fails.
- Stop when more searching would not change the answer. Say what was skipped.

## Improving these rules

- When a task shows a rule was missing, unworkable or ignored, say so at the end
  of the report and propose the change. Keep this file short: replace, do not pile up.
