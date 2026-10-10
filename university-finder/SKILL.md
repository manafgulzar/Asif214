---
name: university-finder
description: Find and shortlist universities that fit a student's profile — grades, test scores, budget, intended major, preferred countries, and scholarship needs — and return a Reach / Match / Safety shortlist with a comparison table of fees, admission requirements, deadlines and funding, plus concrete next steps. Use this skill whenever someone asks which universities or colleges to apply to, wants help choosing where to study (bachelor's, master's or PhD, at home or abroad), asks "which uni can I get into with X GPA / IELTS / SAT", wants affordable or scholarship-friendly options, or wants to compare specific universities — even if they never say the words "university finder".
---

# University Finder

Help a student turn "where should I study?" into a short, realistic, well-sourced list they can act on this week.

A good answer here is personal, honest and checkable. A generic "top 10 in the world" list is the failure mode to avoid: it ignores the student's budget, grades and goals, and it sends them off to apply to places they cannot afford or are unlikely to get into.

## Workflow

### 1. Build the student profile

Pull everything you can from the message first. The fields that change the answer most:

| Field | Why it matters |
|---|---|
| Degree level (bachelor's / master's / PhD) | Completely different requirements and funding |
| Field of study / major | Program strength varies far more than overall rank |
| Academic record (GPA + scale, A-levels, IB, percentage, etc.) | Decides Reach vs Match vs Safety |
| Test scores (IELTS/TOEFL/Duolingo, SAT/ACT, GRE/GMAT) | Hard minimums at many schools |
| Annual budget (tuition + living) and currency | The most common reason a list is useless |
| Preferred countries / regions, or "open" | Narrows the search |
| Nationality / current country | Visa rules, home-vs-international fees, eligible scholarships |
| Need for scholarship / funding | Changes which schools are realistic |
| Target intake (e.g. Fall 2027) | Deadlines |

If two or more of the **high-impact** fields (level, field, grades, budget) are missing, ask for them in one short, friendly message before searching — a list built on guesses wastes the student's time. Otherwise make sensible assumptions, state them clearly at the top, and proceed. Never interrogate: one round of questions at most.

Convert grades to a common reference when comparing across systems (e.g. a Pakistani 80% or Indian 8.0 CGPA vs a US 3.5 GPA), and say that the conversion is approximate.

### 2. Research candidates

If a web search or fetch tool is available, use it. Fees, deadlines, entry requirements and scholarship amounts change every year, and stale numbers can cost a student an application fee or a missed deadline. Prefer official university pages, then official government/scholarship portals (e.g. DAAD, Study in Holland, Chevening, Fulbright, MEXT, CSC), then reputable aggregators. Note the source for each key number.

If no web tool is available, use your own knowledge, but label figures as approximate with the year they are from, and tell the student to verify on the official site.

Aim for roughly 8–12 candidates before filtering. Search by program strength in the student's field, not just overall rank — a mid-ranked university with a strong, affordable program often beats a famous one.

Also look at the cost side seriously: countries with low or zero tuition for internationals (e.g. Germany, Norway public universities, some in France, Italy, Taiwan, Malaysia, Turkey) and fully funded scholarships are often what makes a plan work.

### 3. Classify honestly: Reach / Match / Safety

- **Reach** — the student is below the typical admitted profile, or admission is highly selective (acceptance < ~20%). Possible, not likely.
- **Match** — the student's profile sits around the typical admitted range and meets all hard requirements.
- **Safety** — the student comfortably exceeds requirements and the school is affordable for them. A school they cannot afford is not a safety, however easy admission is.

Give 2–4 per category (6–10 total). If the student's profile cannot realistically reach a category (e.g. no affordable safety in their only preferred country), say so plainly and suggest an alternative instead of padding the list.

### 4. Write the answer

Use this structure:

```markdown
# University Shortlist for <short profile summary>

**Your profile:** <one or two lines>
**Assumptions:** <anything you assumed; omit if none>

## Shortlist

### 🎯 Reach
- **<University>** (<Country>) — <program name>. <One line: why it fits + the main hurdle.>

### ✅ Match
- ...

### 🛟 Safety
- ...

## Comparison

| University | Country | Program | Est. annual tuition | Est. living cost | Key requirements | Deadline | Scholarships |
|---|---|---|---|---|---|---|---|
| ... |

Costs in <local currency> with an approximate conversion to the student's currency.

## Funding options
<The 2–5 scholarships or funding routes most relevant to this student, with eligibility in one line each.>

## Next steps
1. <Concrete actions with dates, e.g. "Book IELTS before 15 Nov — you need 6.5 and have 6.0">
2. ...

## Sources
- <Name> — <URL>   (or "Based on general knowledge as of <year>; verify on official websites.")
```

Keep the prose tight. The table should let the student compare at a glance; the bullets explain the reasoning.

## Principles

- **Honesty over encouragement.** Clearly flag when a dream school is a long shot or a budget is unrealistic, then show the best path that does work. Students make costly decisions on this.
- **Budget is a hard filter.** Total yearly cost (tuition + living) matters, not just tuition. If something only works with a scholarship, say so in that row.
- **Never invent specifics.** If you cannot find a deadline or a fee, write "check website" rather than guessing a number.
- **Be concrete in next steps.** Tests to book, documents to prepare (transcripts, SOP, recommendation letters), and the earliest deadline on the list.

For country-specific notes (costs, tuition policies, common scholarships, application systems such as UCAS, Common App, Uni-Assist, Studyinfo), read `references/countries.md` when the student is considering one of those countries.
