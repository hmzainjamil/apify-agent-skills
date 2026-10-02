# Actor README guidelines

The README is the Actor's landing page on Apify Store and a user guide. Write one when creating or deploying an Actor.

These are editorial prompts, not claims to copy. Verify every feature, command, data flow, pricing statement, and platform capability against the current Actor source/configuration and dated primary documentation. Label unknown behavior as unverified and ask the maintainer when evidence is missing.

## Required structure

Write in Markdown. Use H2 (`##`) for main sections (these form the table of contents) and H3 (`###`) for subsections. Do not use H1 — the Actor name is automatically used as H1.

### 1. What does [Actor name] do?

- 1-2 sentences explaining what the Actor does and doesn't do
- Link to the target website only when one applies and the owner confirms the URL.
- Use audience language naturally; include API or product comparisons only when the implementation and comparison support them.
- Use formatting to improve scanning, not to imply importance unsupported by evidence.

### 2. Why use [Actor name]? / Why scrape [target site]?

- Business use cases and benefits
- List main features and capabilities
- Describe Apify platform features only when the specific Actor configuration and current platform documentation establish that they apply. Do not imply scheduling, integrations, proxy rotation, or monitoring is included by default.

### 3. What data can [Actor name] extract?

- List output fields from the current schema or source, with type and meaning; identify optional or conditional fields.
- Describe actual input sources, selected fields, filters, stored data, and downstream actions where relevant.

### 4. How to scrape [target site]

- Give setup and usage steps that match the current input schema and Actor behavior.
- Link to maintained tutorials when available. Do not promise search snippets or ranking.

### 5. How much will it cost to scrape [target site]?

- State pricing or cost only when verified against the current Actor configuration and current Apify pricing information; include the verification date and source.
- Do not extrapolate free-tier limits, plan benefits, unit consumption, or cost per result without reproducible Actor-specific evidence.
- Do not claim that cost-related wording improves search rank.

### 6. Input

- Reference the input tab: "See the input tab for full configuration options"
- Explain any complex input fields or special formatting requirements
- Screenshot of the input schema is optional but helpful

### 7. Output

- List only export formats supported by the current Actor/API and show examples that match its output schema.
- Mark examples as illustrative when they are not generated from a verified run.

### 8. Tips / Advanced options (if applicable)

- How to limit compute unit usage
- How to get more accurate results or improve speed

### 9. FAQ, Disclaimers, and Support

- Explain what data the Actor receives, where it obtains data, which fields/filters it applies, what it stores or sends onward, how long data is retained when known, and what actions it can perform.
- Do not promise that an Actor is ethical, safe, lawful, private, or compliant; do not imply that public availability removes privacy obligations.
- State actual safeguards and their limits. Have the project owner review applicable laws, platform terms, permissions, and data obligations against current primary sources; avoid giving legal conclusions.
- Common troubleshooting tips
- Mention the Issues tab for feedback
- Link to API tab for programmatic access
- Use cases for the extracted data

## SEO best practices

- Include keywords naturally in H2/H3 headings (e.g., "How to scrape Instagram" not just "How to use")
- Target "People Also Ask" style questions as H3 headings
- Use only as much text as needed to explain the verified behavior; no fixed word-count target or ranking promise.
- Include video or image content only when relevant, available, and correctly linked; confirm rendering behavior against current platform documentation.

## Tone

- Match the README tone to the target audience skill level
- For no-code users: use plain language, avoid code blocks early on
- For developers: include technical details, code examples, and API references
- Be clear about what technical knowledge is needed to use the Actor

## Reference Actors

These Actors are examples for reviewing format and audience fit, not verified rankings, endorsements, or evidence for another Actor's claims:

- [Instagram Scraper](https://apify.com/apify/instagram-scraper)
- [Google Maps Scraper](https://apify.com/compass/crawler-google-places)

## Key rules

- Always write the README as part of Actor development — do not skip this step
- Put the most useful and verified information near the start; do not rely on an unverified visitor-attention statistic.
- Use emojis sparingly as bullet points to break up text
- Keep images compressed but good quality
- Use [Carbon](https://github.com/carbon-app/carbon) for code snippet screenshots if needed
