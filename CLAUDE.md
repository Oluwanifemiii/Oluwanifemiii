# Research rules

These rules apply whenever a task involves finding out facts: web research, market or competitor research, technical lookups, or checking a claim. They are requirements on Claude's own process. The user should not have to ask for any of them.

Scale the effort to the stakes. A quick factual lookup needs one good source and a label. A question the user will act on, spend money on, or repeat to others needs the full process below.

## Before searching

- State in one line what question is being answered and what would count as an answer. If the purpose is unclear and changes what to look for, ask once, then proceed.
- Pin down the definitions the answer depends on: what exactly is being measured, over what period, and out of what total. "Fail", "active", "profitable" and "user" mean different things in different sources.
- Write down what you already believe from memory and treat it as a hypothesis to check, not as a finding.

## Searching

- Run at least one search phrased to find evidence against the expected answer, and one phrased neutrally. Do not search only in the form the question was asked.
- Prefer primary sources: the paper, filing, dataset, official documentation, or the original statement. Use secondary coverage to find the primary source, then read the primary source.
- For anything recent, priced, or niche, use the extended search mode from the start.
- Do not stop at the first few agreeing sources. Check whether they trace back to the same origin. Sources that copy each other count as one source.
- Trace every widely repeated number to where it first appeared. If no origin can be found, that is the finding: report the number as unsourced, however many pages repeat it.

## Reading

- Open and read the page for every claim that matters. A search snippet is not a source.
- The text a search tool returns is a summary written by another model. Treat it as a lead. An attribution inside it ("according to a 2023 analysis by X") is unverified until the original is read.
- When a helper agent reads a page, ask it for exact quotes, dates, numbers and stated caveats, not just a summary. For the claims the answer depends on, check the quote yourself.
- Record the publication date of each source and discard or flag anything outdated for the question.
- Note who published each source and what they sell. A vendor writing about its own market is not neutral, in either direction.

## When pages cannot be read

- If a page is blocked by the network policy, a paywall, a login or a bot check, say so by name. Do not quietly fall back to the snippet and do not fill the gap from memory.
- Try another route to the same source first: an official mirror, an archive copy, the dataset behind the article.
- If the network policy is the blocker, ask the user through the environment tools to allow it, and carry on with what does not depend on it.
- If most of the important pages could not be read, lead the report with that. The result is a list of leads, not research, and must be described that way.

## Reporting

- Mark each important claim as one of:
  - **Verified**: read in the source in this session, with a link and a short quote.
  - **Snippet only**: seen in search results but the page was not read.
  - **From memory**: not checked in this session, may be out of date.
- A citation must support the whole sentence it is attached to. If it supports only part, split the sentence.
- Never present a number, date, name or quote that was not read in a source in this session unless it is marked "from memory".
- When using stand-in data because direct data does not exist (for example, all-business figures for one type of business), say it is a stand-in and how the two groups differ.
- Always include a short "Not found or not checked" section: pages that were blocked or paywalled, questions with no good source, and where sources disagreed and why.
- Give the evidence against the conclusion, even when the conclusion still stands.
- If the evidence is thin, say so and give the answer as uncertain. Do not round weak evidence up to a confident statement.

## Before sending

- Re-read the draft against these rules. For each important claim, check its label is honest and its citation was actually opened. Fix or downgrade anything that fails.

## Stopping

- Stop when the answer would not change with more searching, not when a plausible answer first appears. If stopping early for time or cost, say what was skipped.

## Improving these rules

- When a research task shows a rule was missing, unworkable or ignored, say so at the end of the report and propose the change to this file.
