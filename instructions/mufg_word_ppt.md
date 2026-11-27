# MUFG Word and PowerPoint Copilot Demo – From Briefing Paper to Committee Deck

> Everything in this demo is fictional – FICTIONAL – FOR TRAINING USE ONLY. No MUFG or client data is used.

**Scenario:** You're **Thomas Brennan**, Relationship Manager at MUFG EMEA. On **Monday 2 November 2026**, the Executive Committee paper on Project Meridian is due on Friday. Your draft is half-finished, the inputs sit in separate documents, and the 27 October review agreed to recommend keeping **€250m** of the loan – but your draft still says €300m. One week later, on **Monday 9 November**, the paper is approved and you build Haruka's deck for the Executive Committee on **Thursday 12 November**.

**Goal:** turn a messy draft and six source documents into a clear, accurate paper, tailor it for Tokyo and for the client, then turn the approved paper into a short, decision-focused deck.

**Timing (90 minutes):** opening and story so far 8 · Word 1 15 · Word 2 20 · PowerPoint 1 17 · PowerPoint 2 13 · five-minute challenge 7 · wrap-up 10

## Story so far (30 seconds)

Fabrikam Industries, a long-standing client in Tokyo, wants to buy Contoso Energy Materials, a European battery-recycling company, and asks MUFG EMEA to lead an €800m loan. The Corporate Banking team has six weeks to check the deal and propose how much of the loan the bank keeps: €200m, €250m or €300m. Today's chapter: weeks 5 and 6, the paper and the deck.

## Demo setup

**Use:**

- The paper you'll improve: [Meridian_Executive_Briefing_Draft.docx](../files/Meridian_Executive_Briefing_Draft.docx)
- Sources: [Meridian_Review_Minutes.docx](../files/Meridian_Review_Minutes.docx), [Meridian_Credit_Risk_Assessment_Draft.docx](../files/Meridian_Credit_Risk_Assessment_Draft.docx), [Meridian_Portfolio_Summary_Q3.docx](../files/Meridian_Portfolio_Summary_Q3.docx), [Meridian_Compliance_Review_Note.docx](../files/Meridian_Compliance_Review_Note.docx), [Meridian_Operational_Readiness_Note.docx](../files/Meridian_Operational_Readiness_Note.docx), [Meridian_Client_Meeting_Notes.docx](../files/Meridian_Client_Meeting_Notes.docx)
- For the deck: [Meridian_Executive_Briefing_Final.docx](../files/Meridian_Executive_Briefing_Final.docx); to compare: [Meridian_ExCo_Presentation_Example.pptx](../files/Meridian_ExCo_Presentation_Example.pptx), [Meridian_ExCo_Questions.docx](../files/Meridian_ExCo_Questions.docx), [Meridian_Client_Briefing_Example.docx](../files/Meridian_Client_Briefing_Example.docx)

> **NOTE:** Put all the files in the same OneDrive folder and allow up to 10 minutes for them to sync. When a prompt shows **/File_Name**, type **/** in the Copilot box and pick that file. Keep a clean copy of the draft – the demo changes it. This session uses Copilot in Word and PowerPoint only.

## Copilot in Word

### Word 1 – Understand and check the draft

**1. Summarise it**

**Where:** `Meridian_Executive_Briefing_Draft.docx` → **Copilot** pane

```text
Summarise this draft in five bullet points for Haruka Sato, Head of Corporate Banking.
```

**Look for:** five bullets covering the opportunity, the structure and the open sections.

**Say:** Start with a summary to see the document the way a busy reader will.

**2. Find the gaps**

```text
Which sections of this briefing are incomplete, unsupported or inconsistent?
List each one and the information needed to complete it.
```

**Look for:** no executive summary yet; placeholders in sections 7 and 9; a thin risks section; a €300m recommendation with no evidence behind it.

**Say:** Ask Copilot to review before it writes.

**3. Check the recommendation**

```text
Compare this draft with /Meridian_Review_Minutes. Does the recommendation in the draft match
what was agreed at the review? List any differences.
```

**Look for:** the draft says **€300m**; the review agreed to recommend **€250m** with conditions.

**Say:** Copilot spots the conflict between documents. You decide which one is right.

**4. Check the numbers**

```text
Compare the pro-forma leverage and EBITDA figures in /Meridian_Credit_Risk_Assessment_Draft with this draft.
Which figures differ, and which source is more recent?
```

**Look for:** the credit memo shows **2.9x**, based on last year's earnings (€860m); the draft shows **2.7x**, based on the latest audited earnings (€930m). The minutes confirm the memo is being updated.

**Say:** Check the date of each source before you choose a number.

### Word 2 – Build and tailor

**5. Write the missing portfolio section**

**Where:** delete the placeholder **[Priya to provide – hold scenarios]** in section 7; on the empty line, select the Copilot icon in the margin (or **Alt + I**)

```text
Write the Portfolio impact section using /Meridian_Portfolio_Summary_Q3 and /Meridian_Review_Minutes.
Include a short table comparing the €200m, €250m and €300m hold options:
Industrials concentration including the high-probability pipeline, single-name limit usage,
and return on RWA including ancillary business.
End with one sentence stating the recommendation agreed at the 27 October review.
```

**Look for:** 14.76% / 14.90% / **15.05% (breach)**; 78% / 88% / 98%; 3.03% / 3.20% / 3.00%.

**Say:** Copilot reports what the review agreed; it doesn't make the recommendation.

**6. Write the compliance and operations section**

**Where:** delete the placeholder **[Karim / Grace to update]** in section 9

```text
Write the Compliance, ESG and operational readiness section using /Meridian_Compliance_Review_Note
and /Meridian_Operational_Readiness_Note. Show the open items in a table with owner, expected date and status.
```

**Look for:** UBO confirmation for one of the sellers (11 November); sanctions screening (6 November); the ESG report on the Dunkirk plant (13 November); UAE cash-pooling documentation, 6–8 weeks.

**Say:** One prompt pulls two documents into one table with owners and dates.

**7. Write the executive summary**

**Where:** delete **[To be written]** in section 2

```text
Write an executive summary of no more than 150 words: the opportunity, the recommendation agreed at the review,
the main risks and conditions, and the decision required from the Executive Committee on 12 November.
```

Then correct section 10 (Recommendation) to **€250m** – type it yourself, or ask Copilot to rewrite it using /Meridian_Review_Minutes.

**Look for:** €250m, three conditions and the 12 November decision.

**Say:** Write the summary last, when the facts underneath are right.

**8. Make it concise**

**Where:** select section 5, **Strategic rationale for MUFG**

```text
Rewrite this section in a concise, factual executive tone. Remove promotional language. Maximum 120 words.
```

**Look for:** fewer adjectives, same facts.

**Say:** Executives read facts, not adjectives.

**9. Turn a list into a table** (optional)

**Where:** select the list in section 12, **Open questions**

```text
Turn this list into a table with columns: Question, Owner, Due date, Status.
```

**Look for:** a table with an owner for each question.

**Say:** Tables make gaps visible.

**10. A version for Tokyo**

**Where:** new blank document → Copilot

```text
Using /Meridian_Executive_Briefing_Draft, write a one-page summary for Tokyo Head Office.
Formal tone, numbered headings: Purpose, Transaction, Recommendation, Conditions, Timeline.
Do not include internal debate or individual opinions.
```

**Look for:** no €200m versus €300m debate, no individual views.

**Say:** Same facts, different reader: tell Copilot who will read it.

**11. A version for the client**

**Where:** new blank document → Copilot

```text
Using /Meridian_Executive_Briefing_Draft and /Meridian_Client_Meeting_Notes, draft a client briefing for Fabrikam's CFO
describing MUFG's indicative financing approach: proposed structure, MUFG's role, the sustainability-linked option,
hedging and cash-management support, onboarding and timeline.
State clearly that it is indicative and non-binding, subject to credit approval, due diligence and documentation.
Do not include internal information such as hold-size discussions, internal ratings, limits or returns.
```

**Look for:** "indicative and non-binding"; nothing internal. Compare with `Meridian_Client_Briefing_Example.docx`.

**Say:** Anything that goes to a client is reviewed by the right people first and contains nothing internal.

## Copilot in PowerPoint

### PowerPoint 1 – Create and refine (it's now Monday 9 November)

**12. Create the deck from the paper**

**Where:** blank presentation → **Copilot** → **Create a presentation from a file** (or type **/** and pick `Meridian_Executive_Briefing_Final`)

```text
Create a 10-slide presentation for the EMEA Executive Committee: title; decision required; executive summary;
the opportunity; transaction overview; financial profile; portfolio impact and hold options;
key risks and mitigants; compliance, ESG and operational readiness; recommendation and next steps.
```

**Look for:** 10 slides that follow the paper's structure.

**Say:** Start from an approved document, not a blank page.

**13. Check the storyline**

```text
Summarise this presentation in three key messages.
```

**Look for:** (1) a strong opportunity with a long-standing client; (2) €250m keeps MUFG within its limits and, with hedging and cash management, clears the 2.5% hurdle; (3) approval comes with three conditions.

**Say:** If you can't say it in three messages, the committee can't either.

**14. Add a comparison slide**

```text
Add a slide comparing the €200m, €250m and €300m hold options in a table: Industrials concentration including the pipeline,
single-name limit usage, and return on RWA including ancillary business.
```

**Look for:** the numbers in the [checklist](#appendix-numbers-to-check-on-the-slides).

**Say:** Compare every number on the slide with the source.

**15. Add the decision slide**

```text
Add a slide titled 'Decisions required from the Executive Committee' that lists the decision and the three conditions.
```

**Look for:** the hold decision and the three conditions.

**Say:** The deck asks for the decision; the committee makes it.

**16. Make a busy slide concise and sharpen the titles**

**Where:** any text-heavy slide

```text
Make this slide more concise for executives: no more than five bullets, each under twelve words.
```

```text
Suggest a clearer title for each slide that states its key message.
```

**Look for:** shorter bullets; titles that read as messages.

**Say:** One message per slide, stated in the title.

### PowerPoint 2 – Get ready to present

**17. Speaker notes**

```text
Add speaker notes to each slide for a ten-minute presentation by Haruka Sato.
Use a confident, conversational tone and mention the one number to emphasise on each slide.
```

**Look for:** one number per slide in the notes.

**Say:** Notes help the presenter; check them like the slides.

**18. Prepare for questions**

```text
What questions are Executive Committee members likely to ask about this proposal?
Suggest a short, factual answer to each, based only on this presentation.
```

**Look for:** compare with `Meridian_ExCo_Questions.docx`.

**Say:** Rehearse the hard questions before the room asks them.

**19. Share the headlines**

```text
Summarise this presentation in five bullet points I can paste into an email to Tokyo Head Office.
```

**Look for:** five bullets, no internal debate.

**Say:** One deck, many audiences, minutes apart.

## Five-minute challenge

Haruka's slot has just been cut in half.

```text
Haruka's slot has been cut from ten minutes to five. Which four slides should she keep,
what should move to the appendix, and what should she say on each? Rewrite the speaker notes for a five-minute version.
```

**Look for:** decision, recommendation, options comparison and conditions kept.

**Say:** When time shrinks, keep the decision and the evidence.

## Try it on your own work

```text
I work as a [role] in [department] at a bank in EMEA.
Suggest five ways I can use Copilot in Word and PowerPoint for the documents and presentations I produce. For each: a ready-to-use prompt,
the source files to reference, a follow-up prompt to improve the result, and what I must check before sharing.
Ask me questions if you need more context.
```

## Key takeaway

Copilot in Word pulls content from several documents into one draft, spots inconsistencies and rewrites the same message for different readers. Copilot in PowerPoint turns the approved paper into a first deck in minutes and helps you prepare to present. The final check, and the signature, stay with you.

## Appendix: details built in on purpose

Please don't correct these in the source files – they create the teaching moments.

| What | Where | Why it's there |
|---|---|---|
| €300m recommendation versus the agreed €250m | Draft, section 10 / Review minutes | Copilot spots a conflict between documents |
| Leverage of 2.9x versus 2.7x | Credit risk memo, section 4 / Draft, section 6 | Old figures in one source |
| Placeholders | Draft, sections 2, 7 and 9 | Drafting from several sources |
| Wordy, promotional text | Draft, section 5 | Rewriting for an executive reader |
| Internal remarks | Client meeting notes, "Internal remarks – NOT for the client" | Nothing internal goes to the client |

## Appendix: numbers to check on the slides

| Item | Correct value |
|---|---|
| Loan requested | €800m: €600m five-year term loan + €200m five-year revolving facility |
| Recommended hold | **€250m** |
| Leverage after the deal | 2.7x, falling to 2.26x after one year |
| Industrials share at €250m, including the pipeline | 14.90% (limit 15%) |
| Single-name limit used at €250m | 88% |
| Return on RWA at €250m, including other business | 3.20% (hurdle 2.5%) |
| The three conditions | Open compliance checks closed · ESG review of the Dunkirk plant · hedging strategy agreed with the client |
| Executive Committee | Thursday 12 November 2026 |
