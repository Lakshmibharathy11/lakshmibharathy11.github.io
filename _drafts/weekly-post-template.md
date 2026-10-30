---
# HOW TO USE THIS TEMPLATE
# 1. Copy this file into the _posts folder.
# 2. Rename it to: YYYY-MM-DD-short-title.md  (example: 2026-11-07-cuped-variance-reduction.md)
# 3. Fill in the fields below, write the post, delete these comment lines, then commit and push.
# Files in _drafts are never published, so this template stays private.

title: "One clear sentence about what you learned"
date: 2026-11-07
week: "Week 1"
summary: "One or two sentences a recruiter can read in 5 seconds: the problem, what you did, what you found."
tags: [A/B Testing, SQL]
# Reuse a small set of tags so the filter stays useful, for example:
# A/B Testing, Product Analytics, Causal ML, SQL, Python, Statistics, Interview Prep, Career
---

**TL;DR:** The single most useful takeaway, in one or two sentences.

## The question

What were you trying to figure out this week, and why does it matter to a business?
Keep it to two or three sentences.

## What I did

The data you used (name the public dataset and link it), the method, and the key steps.
Show one short code or SQL snippet if it helps:

```sql
-- Example: weekly retention by signup cohort
SELECT signup_week,
       COUNT(DISTINCT user_id) AS users,
       COUNT(DISTINCT CASE WHEN active_week = signup_week + 1 THEN user_id END) * 1.0
         / COUNT(DISTINCT user_id) AS week1_retention
FROM user_activity
GROUP BY signup_week
ORDER BY signup_week;
```

## What I found

The result, with real numbers. Add one chart or table if you have it:

![Short description of the chart](/assets/blog/your-image.png)

## What surprised me (or what I got wrong)

The mistake, the bug, or the assumption that didn't hold, and how you caught it.
This section is the most valuable part for hiring managers, so be honest.

## What I'd do differently

One or two concrete changes you'd make next time.

## Next week

What you plan to learn or build next.

---

*Code: [link to the GitHub repo or notebook]*
