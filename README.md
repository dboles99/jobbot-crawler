# JobBot crawler

JobBot is a small personal research tool. It reads public company information and
public job-board listings. This page is here so site owners know what it is and how
to reach me.

## What it fetches

- Public job-board APIs: Greenhouse, Lever, Ashby and Workable.
- A company's homepage and careers page, at most three pages per company.
- Wikidata, for basic company facts such as the founding year and headquarters.

## How it behaves

- It follows robots.txt. If robots.txt cannot be reached, it does not crawl the site.
- It waits at least 3 seconds between requests to the same site.
- It never logs in, fills in forms, or gets around bot checks.
- It collects no personal data. The only email addresses it keeps are the ones a
  company publishes for applications, such as jobs@ or careers@.

## User-Agent

    JobBot/0.1 (+https://github.com/dboles99/jobbot-crawler)

## Blocking it

Add this to your robots.txt:

    User-agent: JobBot
    Disallow: /

## Contact

Open an issue in this repository.
