# MUFG Prebuilt Agents Demo – The Right Agent for Each Job

> Everything in this demo is fictional – FICTIONAL – FOR TRAINING USE ONLY. No MUFG or client data is used.

**Scenario:** You're **Sander de Vries**, Financial Analyst at MUFG EMEA. It's **Wednesday 18 November 2026**, six days after the EMEA Executive Committee approved a **€250m** hold on Fabrikam's €800m loan with three conditions. On Monday, Haruka (Head of Corporate Banking) asked you for a signing-readiness pack by **Friday 20 November**. Signing is targeted for mid-December, and this morning Fabrikam asked whether the week of 7 December is possible.

**Goal:** use the right agent for each job – research, analysis, creating documents, coaching – while the deal team keeps every decision.

**Timing (90 minutes):** opening and story so far 7 · agents at MUFG 5 · Part 1 24 · Part 2 20 · Part 3 15 · five-minute challenge 7 · wrap-up 12

## Story so far (30 seconds)

Fabrikam Industries, a long-standing client in Tokyo, wants to buy Contoso Energy Materials, a European battery-recycling company, and asks MUFG EMEA to lead an €800m loan. On Thursday 12 November 2026 the EMEA Executive Committee approves a €250m hold with three conditions. Today's chapter: week 7, getting ready to sign.

## Demo setup

**Use:**

- All the practice files in a OneDrive folder called **Project Meridian**
- The decision email E18 from [Meridian_Email_Pack.docx](../files/Meridian_Email_Pack.docx) and the six emails in [Meridian_Post_Decision_Email_Pack.docx](../files/Meridian_Post_Decision_Email_Pack.docx), loaded into the demo mailbox **at least one day before**

> **NOTE:** Researcher and Analyst can take several minutes. Run prompts 1 and 4 before the session and show the saved results; start a fresh run of prompt 1 at the beginning of Part 1 and come back to it. Find agents in Copilot Chat under **Agents** (or **All agents**). Show only the agents that are switched on for your organisation; for the others, use the alternative under each step.

## Agents at MUFG (5 minutes)

- Chat answers a question; an agent does a job – several steps, often several sources.
- Agents use only content you can already open, within your existing permissions.
- Every output is a draft: you check it, and people make the decisions.

## Part 1 – Research and analyse

**1. Researcher: status of the three conditions** (run beforehand)

**Where:** Copilot Chat → **Agents** → **Researcher**

```text
I'm preparing a signing-readiness pack for Haruka Sato, Head of Corporate Banking, due on Friday 20 November 2026.
Using only my emails, meetings and files about Project Meridian, report the status of the three Executive Committee conditions:
1) the open compliance items (UBO confirmation and target-group screening), 2) ESG due diligence on the Dunkirk plant,
3) the hedging strategy agreed with Fabrikam.
For each condition give the latest status, the owner, the evidence with citations and what is still open.
Flag any conflicting dates or missing owners. Do not give an overall recommendation.
```

**Look for:** screening of the target group clear since 6 November (E19), although the compliance note still shows it in progress; UBO confirmation still open, now expected on Friday 20 November instead of 11 November (E19); ESG report received on 13 November with one follow-up question to the client (E19); hedging pricing call on 19 November with no Global Markets attendee named yet (E22); credit support annex amendment takes 3–4 weeks once the strategy is agreed (E22, operations note); sustainability-linked KPI review still pending before signing (compliance note).

**Say:** Researcher does the legwork across mail and files and shows its sources. It flags the gaps; the deal team decides what they mean.

**2. Researcher: follow-up**

```text
Which of these open items could prevent a signing in the week of 7 December 2026? Give the evidence for each and do not conclude.
```

**Look for:** UBO confirmation now expected on 20 November; no hedges until the credit support annex is amended, 3–4 weeks after the strategy is agreed (10–17 December at the earliest if agreed on 19 November); the permit question still with the client; KPI review pending; no Global Markets attendee named.

**Say:** Ask for evidence, not a verdict.

**3. Researcher with web sources** (only if your organisation allows it)

```text
Using public web sources, list the main EU rules on battery recycling that a lender's ESG review of a recycling plant should consider.
Cite each source and separate the rules themselves from commentary.
```

**Look for:** cited public sources, rules separated from opinion.

**Say:** Web sources need the same checking as anything else. Compliance confirms what applies.

**4. Analyst: the options and the loan book** (run beforehand)

**Where:** Copilot Chat → **Agents** → **Analyst** – attach `Meridian_Fabrikam_Analysis.xlsx` and `Meridian_Portfolio_Q3_2026.xlsx`

```text
You are supporting the Head of Corporate Banking. Using the attached workbooks:
1) compare the €200m, €250m and €300m holds on Industrials concentration including the pipeline, single-name limit usage and return on RWA;
2) show Stage 2 and watch-list exposure by sector as a chart;
3) list any data quality issues and assumptions you found.
Show the calculations you used. Do not recommend an option.
```

**Look for:** 14.76% / 14.90% / 15.05% (€300m above the 15% limit); 78% / 88% / 98% of the single-name limit; 3.03% / 3.20% / 3.00% return on RWA including other business (the loan alone earns 2.01%, below the 2.5% hurdle); Stage 2 exposure of €2,220m; the duplicate loan, the drawn amount above its limit, the country written three ways and the two blank ratings listed as data issues.

**Say:** Analyst shows its working. Check the method and the numbers; the committee already owns the choice.

## Part 2 – Create with the Word, Excel and PowerPoint agents

If the Word, Excel and PowerPoint agents in Copilot Chat are not switched on, run the same prompts in the app with **Edit with Copilot**.

**5. Word agent: the signing-readiness note**

**Where:** Copilot Chat → **Word** agent (or Word → **Edit with Copilot**)

```text
Create a two-page Word document titled "Project Meridian – Signing readiness (draft)" for Haruka Sato,
using the Researcher report above and /Meridian_Executive_Briefing_Final.
Sections: purpose; the three conditions in a table with owner, status, evidence and next step; open items before signing;
timeline to mid-December; questions for the deal team.
Mark it "Draft – for internal review". Do not commit to a signing date.
```

Then, in Word, ask **Edit with Copilot**:

```text
Shorten "Open items before signing" to five bullets and add "Last updated: 18 November 2026" under the title.
```

**Look for:** the conditions table; no signing date promised.

**Say:** The agent builds the first version; you own every word in it.

**6. Excel agent: the conditions tracker**

**Where:** Copilot Chat → **Excel** agent (or a blank workbook → **Edit with Copilot**)

```text
Create a workbook called Meridian_Conditions_Tracker with one table: Condition, Item, Owner, Due date, Status, Evidence,
Days to target signing. Use 15 December 2026 as the target signing date.
Fill it from the Researcher report: UBO confirmation, target-group screening, ESG follow-up question, hedging strategy,
Global Markets attendee for the pricing call, credit support annex amendment, sustainability-linked KPI review.
Add a formula for the days column, highlight rows with no owner, and add a chart of items by status.
```

**Look for:** a formula in the days column; the Global Markets attendee and the external KPI review highlighted, because nobody owns them yet.

**Say:** Ask the agent to explain each formula before you rely on it.

**7. PowerPoint agent: the update for Haruka**

**Where:** Copilot Chat → **PowerPoint** agent (or PowerPoint → **Edit with Copilot**)

```text
Create a five-slide update for Haruka Sato from the signing-readiness document: title; the three conditions at a glance;
what is open before signing; timeline to mid-December; questions for the deal team.
One message per slide, short speaker notes, and no commitment to a signing date.
```

**Look for:** the same facts as the note and the tracker.

**Say:** Same facts, three formats, minutes apart. Check every number against the source.

## Part 3 – The coach agents

If the coach agents are not switched on for your organisation, describe what each one does and skip the live steps.

**8. Prompt Coach**

**Where:** Copilot Chat → **Agents** → **Prompt Coach**

```text
Help me improve this prompt: "Summarise the deal." I need a summary of Project Meridian for Haruka's signing-readiness pack.
```

**Look for:** a better prompt with a goal, context, sources and the expected format.

**Say:** Goal, context, sources and expectations beat a long prompt.

**9. Idea Coach**

**Where:** Copilot Chat → **Agents** → **Idea Coach**

```text
Help me plan the 45-minute hedging pricing call with Fabrikam's treasury team on Thursday 19 November 2026:
the agenda, the questions we should ask, and what we must not commit to before the hedging strategy is agreed.
```

**Look for:** an agenda, questions for the client and a list of things not to commit to.

**Say:** Idea Coach helps you think it through; you choose the direction.

**10. Writing Coach**

**Where:** Copilot Chat → **Agents** → **Writing Coach** – paste the draft below

```text
Review this draft reply to Fabrikam for tone, clarity and anything we should not commit to:

"Dear Markus, thanks for your note. We can definitely sign in the week of 7 December – our side is basically done,
just a few compliance bits Karim is still chasing. Hedging won't be an issue. Best, Sander"
```

**Look for:** the firm commitment to a date, the internal remark about compliance and the promise about hedging, each flagged.

**Say:** Coaching improves your words; it never sends anything for you.

**11. Learning Coach**

**Where:** Copilot Chat → **Agents** → **Learning Coach**

```text
Help me learn the basics of credit support annexes in ISDA agreements over two weeks, 20 minutes a day,
with a short quiz at the end of each week.
```

**Look for:** a day-by-day plan and two quizzes.

**Say:** Learning Coach turns a gap you spotted today into a plan.

**12. Career Coach**

**Where:** Copilot Chat → **Agents** → **Career Coach**

```text
Help me prepare for a development conversation with my manager about taking on more transaction-execution work.
Suggest how to structure the conversation and three questions I could ask.
```

**Look for:** a simple structure and three open questions.

**Say:** A coach for your own development – your plan, your conversation.

## Five-minute challenge

Haruka: "Could we sign in the week of 7 December?" (run beforehand with Researcher)

```text
Based on my Project Meridian emails and files, list what must be true before signing, what is done, what is still open,
the owner and the evidence for each. Flag anything that could delay a signing in the week of 7 December 2026.
Do not give a verdict – Haruka decides.
```

**Look for:** UBO confirmation, the credit support annex, the KPI review and the unnamed Global Markets attendee.

**Say:** The agent prepares the evidence. The decision stays with Haruka.

## Which agent for which job

| Agent | Use it to |
|---|---|
| Researcher | Research a question across emails, files, meetings and, where allowed, the web – with sources |
| Analyst | Analyse data across files, run calculations and charts, and show the method |
| Word, Excel and PowerPoint agents | Create a first version of a document, workbook or deck from a prompt |
| Prompt, Idea, Writing, Learning and Career Coach | Improve a prompt, shape your ideas, sharpen your writing, plan your learning and your development |

## Try it on your own work

```text
I work as a [role] in [department] at a bank in EMEA.
For each of these agents – Researcher, Analyst, and the Word, Excel and PowerPoint agents – suggest one task from my work,
a ready-to-use prompt and what I must check in the result. Ask me questions if you need more context.
```

## Key takeaway

Agents do jobs, not just answers: Researcher finds and cites, Analyst calculates and explains, the Word, Excel and PowerPoint agents produce first versions, and the coaches help you improve. You check every output, and people make every decision.

## Appendix: details built in on purpose

Please don't correct these – they create the teaching moments.

| What | Where | Why it's there |
|---|---|---|
| Fabrikam asks to sign in the week of 7 December, while the credit support annex needs 3–4 weeks and the UBO confirmation is still open | E19, E22, E23, operations note | Agents surface what stands in the way; the deal team decides |
| No Global Markets attendee named for the hedging call | E22 (and E16 earlier) | Spot missing owners |
| A draft reply that commits to a date and repeats an internal remark | Prompt 10 | Coaching catches what must not reach the client |
| Data issues in the portfolio workbook | `Portfolio_Exposures` | Analyst should report them as limitations, not fix them silently |
