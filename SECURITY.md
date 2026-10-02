# Security and privacy

## Credentials

Use a scoped `APIFY_TOKEN` with only the permissions required. Prefer interactive authentication or a protected environment variable. Do not pass tokens as command-line arguments, commit them, paste them into prompts, or include them in logs and reports.

## External services and scraping

The skill guidance may run third-party Apify Actors. Review each Actor's publisher, source, pricing, permissions, data handling, and output before use. Actor runs may access external sites and store results in Apify datasets or key-value stores.

Scrape only sites and data you are authorized to access. Follow target-site terms and applicable privacy rules. Minimize personal data and do not collect sensitive data without approved legal basis and handling.

## Generated output

Review generated Actor code, schemas, and scraped data before deployment, publication, or onward sharing. Use synthetic data in examples and issues.

## Reporting

Report security concerns through a private GitHub Security Advisory for this repository. Do not post credentials or sensitive data in public issues.
