# Enrollment Funnel Analyst

*Higher Ed AI Cookbook · Recipe · Free to use*

A reusable AI recipe that turns a recruitment funnel export into a conversion read: inquiry → application → admit → deposit → enrolled by segment, where each segment leaks, and which stage is most worth the marginal dollar — with every recommendation labelled by how much you should trust it.

## What this recipe does

You give an AI assistant your funnel export and the agent instructions in this recipe. It returns a workbook an enrollment leader can act on:

- Funnel Scorecard — each segment’s inquiry→enroll funnel with application, admit, yield, and melt rates for the latest term.

- Segment Comparison — yield and melt by segment with the weakest stage flagged.

- Trend — inquiries, admits, enrolled, yield, and melt by year.

- Recommendations — prioritized actions, each tagged research-backed, industry-practice, or analyst-judgment.

- Sources & Methodology — every rule, ratio, and limit written down.

## Who it’s for

VPs of enrollment, admissions directors, and IR staff at small institutions that manage a segmented funnel without a dedicated enrollment-analytics team.

## What’s in the recipe

- README (this file) — orients a human, configures the agent, onboards a contractor.

- Agent Instructions — the prompt you paste into the AI tool.

- Sample Output — a fully worked example on a fictional institution, so you see the finished shape.

- Input Template — the expected columns, accepted header aliases, and an example row.

## How to run it

1.  Export your funnel by term and segment (inquiries, applications, admits, deposits, melt).

2.  Shape it using the Input Template. Fill what you have; a missing stage is flagged, not back-filled.

3.  Open your AI assistant, paste the Agent Instructions, and attach your filled template.

4.  Review the workbook against the Sample Output. Sanity-check the ratios before circulating.

5.  Decide — the recipe is scaffolding for an enrollment-strategy decision, not the decision.

## Configuration — the knobs that make it yours

Defaults are set for a small institution. Override in the Input Template’s Config tab if your scale differs:

- Segments: Traditional UG / Online UG / Graduate / Transfer (edit to your segments)

- Yield definition: Enrolled ÷ Admits

- Melt definition: Melt ÷ Deposits

- Scope: which populations to include (e.g. exclude non-degree)

## What it deliberately does NOT do

- It doesn’t set enrollment targets or allocate the marketing budget — those are leadership decisions.

- It doesn’t predict individual applicants. Segment-level only.

- It doesn’t read applicant PII. Stage counts by segment only.

- It doesn’t rename your data silently. Unrecognized columns are flagged.

## /help

If you are holding this recipe with no author in the room, here is the orientation:

- help — what this is: an enrollment-funnel recipe that reads a term×segment export and returns a conversion assessment workbook.

- help inputs — what it needs: a funnel export with inquiries, applications, admits, deposits, and melt (the Input Template shows the shape).

- help outputs — what it gives: a five-tab workbook; the human-legible source of truth is that workbook, not any hidden state.

- help trust — how far to lean on it: recommendations are labelled \[R\]/\[I\]/\[J\]; the Sources & Methodology tab shows every ratio. It assembles and flags — it does not forecast.

Built by Renee Handy · Higher Ed AI Cookbook · build 2026-07. The human-legible source of truth is the returned workbook, not any hidden state. Before you trust this agent with a real decision, find a competent human — a VP of enrollment or admissions director — and have them check the read against your institution’s reality. An orphaned agent should point you at a person, not at itself.

*License: free to use and adapt for your own institution. White-label / resale rights reserved — contact the Cookbook. Sample data is fictional.*

---

## Files in this recipe

- [`EFA_Agent_Instructions.docx`](EFA_Agent_Instructions.docx)
- [`EFA_Input_Template.xlsx`](EFA_Input_Template.xlsx)
- [`EFA_README.docx`](EFA_README.docx)
- [`EFA_Sample_Output.xlsx`](EFA_Sample_Output.xlsx)

*This page is generated from the README `.docx`, which remains the source of truth.*
