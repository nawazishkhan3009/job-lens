## 1. Project Overview

**JobLens** is a cross-browser extension that assists job seekers while browsing job postings.

When a user opens a job post on LinkedIn, Indeed, or a company career page, the extension activates **passively** — it reads the current tab, parses the job post, summarises key information, and offers to generate a tailored cover letter using their chosen LLM.

**What the extension does NOT do:**
- Crawl or search job boards proactively
- Open new tabs or navigate on behalf of the user
- Send any data to any server other than the user's chosen LLM API

---

## 2. Supported Job Sources

| # | Source | Activation Condition |
|---|---|---|
| 1 | LinkedIn Jobs | URL matches `linkedin.com/jobs/view/*` |
| 2 | Indeed | URL matches `*.indeed.com/viewjob*` |
| 3 | Company career pages | Any other URL where structured job data is detected |