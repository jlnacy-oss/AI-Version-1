# Swap the data, keep the layout

`index.html` is format only. Every number, table row, score, price, and news card is painted from `data.js`.

## Publish

Upload BOTH files to the repo root:

- index.html
- data.js

If data.js is missing, the dashboard shows an error instead of empty tables.

## Weekly refresh

1. Run the prompt below.
2. Overwrite data.js only.
3. Commit. Pages rebuilds in about a minute.

## Prompt

Today is [DATE]. Rebuild data.js for the AI Tools Comparison dashboard (window.DASH).
Do not edit index.html.

Keep this shape:
- generated (YYYY-MM-DD)
- vendorOrder (A-Z ids)
- capOrder: grok, openai, copilot, perplexity, claude, gemini, deepseek, metaai, mistral
- vendors[id]: name, company, url, domain, score, note, color,
  maturity{score,label,note}, adoption{score,label,note}, pricingTier{score,label,note}
- capabilities[]: {name, scores:{grok: n, ...}}  // 0-10
- jobs[]: [job, firstPick, runnerUp, buySpecialistWhen, specialist]
- licenseInd[]: [tool, free, everydayPaid, powerUser]
- licenseEnt[]: [tool, team, enterprise, allInNote, dataTraining]
- apiPrices[]: [model, vendor, inputPer1M, outputPer1M, note]
- whatsNew: {eyebrow, headline, lede, featured[titles]}
- news[]: {vendor, title, summary, date, type, impact}
- newsTypes[], newsImpacts[[id,label]], newsVendors[]

News window: last 60 days only.
Vendors: OpenAI, ChatGPT, Claude, Perplexity, Grok, Microsoft, Google, AWS, NVIDIA, Meta, IBM, SAP, ServiceNow, Oracle, Salesforce, Workday, Adobe, Databricks, Snowflake, Palantir, UiPath, CrowdStrike.
Types: Model release, New feature, Platform, Partnership, Integration, Pricing, Security & privacy, Governance, Event, Release notes.
Impact: ga | now | announced | soon.
API prices from official list pages. Do not invent events.
