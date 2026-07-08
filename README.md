Here it is as tables:

### 1. Cell colors (one cell = one user in one period)

| Color | Label | Exact rule | Example |
|-------|-------|-----------|---------|
| 🟡 Yellow | Not Used | Documents = 0 **and** Queries = 0 | 0 docs, 0 queries |
| 🔵 Blue | Used, but potential for more | At least 1 activity, but Documents ≤ 8 **and** Queries ≤ 8 | 3 docs, 5 queries |
| 🟢 Green | Good usage | Documents ≥ 9 **or** Queries ≥ 9 (either one alone is enough) | 12 docs, 2 queries |

*The only threshold is 9, and it's the same for 7-day and 14-day periods.*

### 2. Overall column (one label per user)

A period is **"active"** if its cell is not yellow (blue and green both count equally).

| Color | Label | Exact rule | Example (4 periods) |
|-------|-------|-----------|---------------------|
| 🟡 Yellow | Not Used | Active in 0 periods | 0 of 4 active |
| 🔵 Blue | Intermittent Usage | Active in at least 1 period, but 50% or fewer (exactly half = intermittent) | 2 of 4 active |
| 🟢 Green | Good / Regular Usage | Active in more than 50% of periods | 3 of 4 active |

### 3. Statistics in the Final Report

| Statistic | What it shows | Affects colors? |
|-----------|---------------|-----------------|
| Overall Summary table | Headcount of users in each overall category + total | No — just counts |
| Overall Organisation Usage Behaviour | The category with the most users wins (majority vote) | No — derived from counts |
| Absolute Report sheet | Raw documents & queries per user per period, per-user totals, Organization Total row | No — reference only |

### 4. What the two numbers mean

| Number | Source | How it's calculated |
|--------|--------|---------------------|
| Documents | 13 feature tabs (Assistant, Briefcase, OCR, Sorting Hat, Redline Issues, Consent Tracker, Redaction, Chat, Translator, Workflow Builder, Chronologies, Dataroom Insights, Snapshot) | All values summed per user per period |
| Queries | 3 query tabs (Assistant Queries, Briefcase Queries, Chat Queries) | All values summed per user per period |
