# Retention Risk Analyst

*Higher Ed AI Cookbook · Recipe · Free to use*

A reusable AI recipe that reads first-year retention at the COHORT level — retained rate, DFW rate, and the gap to your retention goal — so leadership can target group-level supports. It never operates on individual students. Cohort aggregates only, by design (FERPA).

## What this recipe does

You give an AI assistant your cohort retention table and the agent instructions in this recipe. It returns a workbook student-success leadership can act on:

- Cohort Retention Scorecard — each entry cohort’s size, retained rate/count, DFW rate, and status vs. goal.

- Trend & Gap to Goal — retention and DFW by cohort, with the gap to the retention goal.

- Recommendations — group-level supports, each tagged research-backed, industry-practice, or analyst-judgment.

- Notes & Methodology — the hard limits (cohort-only, FERPA) and every rule.

## Who it’s for

Provosts, student-success and IR staff setting retention strategy at the cohort level.

## What’s in the recipe

- README (this file) — orients a human, configures the agent, onboards a contractor.

- Agent Instructions — the prompt you paste into the AI tool.

- Sample Output — a fully worked example on a fictional institution, so you see the finished shape.

- Input Template — the expected columns, accepted header aliases, and an example row.

## How to run it

1.  Export retention by entry cohort (cohort size, retained %, DFW rate) — aggregates only, no student rows.

2.  Shape it using the Input Template. An unobserved cohort is marked pending, never forecast.

3.  Open your AI assistant, paste the Agent Instructions, and attach your filled template.

4.  Review the workbook against the Sample Output. Confirm cohort definitions with IR.

5.  Decide — the recipe is scaffolding for a retention-strategy decision, not the decision.

## Configuration — the knobs that make it yours

Defaults are set for a small institution. Override in the Input Template’s Config tab if your scale differs:

- Retention goal: 75% (SG6 example)

- Approaching band: 70–75%

- Cohort definition: first-time UG; edit to yours

- Scope: cohort aggregates only — never individual rows

## What it deliberately does NOT do

- It does NOT accept, produce, or infer individual-student rows, risk scores, or predictions. Cohort aggregates only.

- It does NOT predict which students will leave — retention and DFW rates describe groups, not people.

- It does not create individual education records (FERPA). This is a design constraint, not a setting.

- It refuses a per-student risk score and explains why.

## /help

If you are holding this recipe with no author in the room, here is the orientation:

- help — what this is: a cohort-level retention recipe that reads an aggregate cohort table and returns a cohort-risk workbook. Never individual students.

- help inputs — what it needs: retention by entry cohort (size, retained %, DFW rate) — aggregates only (the Input Template shows the shape).

- help outputs — what it gives: a four-tab workbook; the human-legible source of truth is that workbook, not any hidden state.

- help trust — how far to lean on it: recommendations are labelled \[R\]/\[I\]/\[J\]; cohort level only. It will refuse individual-student prediction (FERPA).

Built by Renee Handy · Higher Ed AI Cookbook · build 2026-07. The human-legible source of truth is the returned workbook, not any hidden state. Before you trust this agent with a real decision, find a competent human — an IR director or student-success lead — and have them check the read against your institution’s reality. An orphaned agent should point you at a person, not at itself.

*License: free to use and adapt for your own institution. White-label / resale rights reserved — contact the Cookbook. Sample data is fictional.*

---

## Files in this recipe

- [`RRA_Agent_Instructions.docx`](RRA_Agent_Instructions.docx)
- [`RRA_Input_Template.xlsx`](RRA_Input_Template.xlsx)
- [`RRA_README.docx`](RRA_README.docx)
- [`RRA_Sample_Output.xlsx`](RRA_Sample_Output.xlsx)

*This page is generated from the README `.docx`, which remains the source of truth.*
