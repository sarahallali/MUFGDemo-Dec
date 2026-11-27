# MUFG Copilot Demos – Project Meridian

Ready-to-run Microsoft 365 Copilot demos – **Outlook, Excel, Word and PowerPoint, and the prebuilt agents** – built around one simple banking story.

| Folder | What's inside |
|---|---|
| [`instructions/`](instructions) | One demo script per session, with copy-ready prompts |
| [`files/`](files) | The practice files and the two email packs the demos use |

> **Everything here is fictional.** The people, companies, deals and figures were invented for training and are labelled "FICTIONAL – FOR TRAINING USE ONLY". No real client or bank data is used.
> Please keep this repository **private**: it was prepared for MUFG training sessions.

## The story in one minute

Fabrikam Industries, a long-standing client based in Tokyo, wants to buy Contoso Energy Materials, a European battery-recycling company. It asks MUFG EMEA to lead an **€800m loan**.

The Corporate Banking team has **six weeks** to check the deal and propose how much of the loan the bank keeps on its own books: **€200m, €250m or €300m**. On **Thursday 12 November 2026** the EMEA Executive Committee approves **€250m with three conditions**: the open compliance checks, ESG due diligence on the Dunkirk plant and a hedging strategy agreed with Fabrikam. Then the team gets ready to sign.

## The four demos

Each demo stands alone and picks up one chapter of the story. Every script opens with a 30-second "story so far".

| Demo | Length | Chapter of the story | You play | Script |
|---|---|---|---|---|
| Outlook | 60 min | Week 1 – The request arrives | Thomas, Relationship Manager | [mufg_outlook.md](instructions/mufg_outlook.md) |
| Excel | 60 min | Week 3 – The numbers | Priya, Portfolio Manager | [mufg_excel.md](instructions/mufg_excel.md) |
| Word and PowerPoint | 90 min | Weeks 5 and 6 – The paper and the deck | Thomas, Relationship Manager | [mufg_word_ppt.md](instructions/mufg_word_ppt.md) |
| Prebuilt agents | 90 min | Week 7 – Getting ready to sign | Sander, Financial Analyst | [mufg_agents.md](instructions/mufg_agents.md) |

## Who's who

| Person | Role in the story |
|---|---|
| Haruka Sato | Head of Corporate Banking – the sponsor, presents to the Executive Committee |
| Thomas Brennan | Relationship Manager for Fabrikam – wants to keep €300m |
| Priya Raman | Portfolio Manager – checks the impact on the loan book |
| Sander de Vries | Financial Analyst – builds the numbers, then the signing-readiness pack |
| Elena Rossi | Credit Risk Manager – prefers €200m |
| Karim Benali | Compliance Officer – client checks (KYC) and ESG |
| Grace Mensah | Operations Manager – account opening and payments |
| Olivia Grant | Executive Assistant to Haruka – diary, notes and follow-ups |

The client: Yuki Hayashi (Chief Financial Officer, Fabrikam, Tokyo) and Markus Brandt (Group Treasurer Europe, Fabrikam).

## Get ready (the day before)

1. Download everything: **Code → Download ZIP**.
2. Upload the `files` folder to your OneDrive, into a folder called *Project Meridian*. Allow up to 10 minutes for the files to sync.
3. **Outlook demo:** load emails E1 to E17 from [Meridian_Email_Pack.docx](files/Meridian_Email_Pack.docx) into your demo mailbox and move them into a folder called *Project Meridian*. See [Demo setup](instructions/mufg_outlook.md#demo-setup).
4. **Agents demo:** use a second demo account, so the two chapters don't mix. Load E18 from the same pack, then E19 to E24 from [Meridian_Post_Decision_Email_Pack.docx](files/Meridian_Post_Decision_Email_Pack.docx), and upload the `files` folder to that account's OneDrive too. Run the Researcher and Analyst prompts once beforehand: they take a few minutes.
5. Keep a clean copy of `Meridian_Portfolio_Q3_2026.xlsx` and `Meridian_Executive_Briefing_Draft.docx`. The demos change them, so reset them between sessions.
6. Run each prompt once. Copilot's wording changes every time; the numbers should not.
7. Show only what is switched on for your organisation. Where an agent may not be available, the script gives an alternative.

## Files at a glance

| File | Used in | What it is |
|---|---|---|
| [Meridian_Email_Pack.docx](files/Meridian_Email_Pack.docx) | Outlook, agents | 18 emails to load into your demo mailbox (the agents demo uses E18 only) |
| [Meridian_Post_Decision_Email_Pack.docx](files/Meridian_Post_Decision_Email_Pack.docx) | Agents | Six emails from the week after the decision (E19 to E24) |
| [Meridian_Portfolio_Q3_2026.xlsx](files/Meridian_Portfolio_Q3_2026.xlsx) | Excel, agents | 150 fictional loans, with a few data errors on purpose |
| [Meridian_Fabrikam_Analysis.xlsx](files/Meridian_Fabrikam_Analysis.xlsx) | Excel, agents | The deal figures and the €200m / €250m / €300m options |
| [Meridian_Executive_Briefing_Draft.docx](files/Meridian_Executive_Briefing_Draft.docx) | Word | The half-finished paper you improve |
| [Meridian_Client_Meeting_Notes.docx](files/Meridian_Client_Meeting_Notes.docx) | Word | Notes from the client meeting on 13 October |
| [Meridian_Credit_Risk_Assessment_Draft.docx](files/Meridian_Credit_Risk_Assessment_Draft.docx) | Word | Credit Risk's view – uses out-of-date figures on purpose |
| [Meridian_Compliance_Review_Note.docx](files/Meridian_Compliance_Review_Note.docx) | Word, agents | Open compliance and ESG checks |
| [Meridian_Operational_Readiness_Note.docx](files/Meridian_Operational_Readiness_Note.docx) | Word, agents | Account-opening and payment readiness |
| [Meridian_Review_Minutes.docx](files/Meridian_Review_Minutes.docx) | Word | Minutes of the 27 October review – agreed to recommend €250m |
| [Meridian_Portfolio_Summary_Q3.docx](files/Meridian_Portfolio_Summary_Q3.docx) | Word | Two-page summary of the loan book |
| [Meridian_Executive_Briefing_Final.docx](files/Meridian_Executive_Briefing_Final.docx) | Word, PowerPoint, agents | The finished paper, and the source for the deck |
| [Meridian_Client_Briefing_Example.docx](files/Meridian_Client_Briefing_Example.docx) | Word | Example of a client-ready version |
| [Meridian_ExCo_Presentation_Example.pptx](files/Meridian_ExCo_Presentation_Example.pptx) | PowerPoint | Example finished deck, with speaker notes |
| [Meridian_ExCo_Questions.docx](files/Meridian_ExCo_Questions.docx) | PowerPoint | Likely Executive Committee questions, with answers |

## Good habits to show in every demo

- **Copilot drafts, you decide.** You stay accountable for what you send.
- **Check every number** against its source before you share it.
- **Check what Copilot used.** For a broad question it works from the most relevant items it finds, so narrow the question and open the sources.
- **Ask for evidence, not a verdict.** Agents prepare the evidence; people make the decisions.
- **Keep internal remarks out** of anything that goes to a client.
- **Copilot only uses content you can already open.** It works within your existing permissions.

## Banking words in plain English

- **Commitment / drawn:** the most a client can borrow / what they have actually borrowed.
- **Final hold:** the part of a shared loan the bank keeps on its own books.
- **Concentration limit:** the most the bank lends to one sector. Industrials: 15% of the loan book, with an early warning at 13.5%.
- **Leverage:** debt divided by yearly earnings (EBITDA). 2.7x means the debt equals 2.7 years of earnings.
- **Return on RWA:** yearly income divided by risk-weighted assets. The bank's hurdle for new loans is 2.5%.
- **KYC / ESG:** know-your-customer checks / environmental, social and governance review.
- **UBO:** ultimate beneficial owner – the people who in the end own or control a company, confirmed as part of KYC.
- **Credit support annex:** the part of a derivatives agreement that sets the collateral rules. Here it must be amended before any hedge is executed.
