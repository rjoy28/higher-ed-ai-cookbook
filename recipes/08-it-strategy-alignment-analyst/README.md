# IT–Strategy Alignment Analyst

*Higher Ed AI Cookbook · Recipe · Free to use*

A reusable AI recipe that maps IT projects and spend to the strategic plan: which goals are backed by investment, which projects are orphaned from strategy, and where a goal has no IT support at all — with every recommendation labelled by how much you should trust it.

## What this recipe does

You give an AI assistant your IT project register and strategic plan, plus the agent instructions in this recipe. It returns a workbook a CIO or cabinet can act on:

- Alignment Map — every project mapped to a strategic goal, with budget, % spent, and on-track status.

- Spend by Strategic Goal — IT investment and project count per goal, with uncovered goals flagged.

- Orphaned Projects — projects with no strategic linkage.

- Recommendations — prioritized actions, each tagged research-backed, industry-practice, or analyst-judgment.

- Sources & Methodology — every rule and limit written down.

## Who it’s for

CIOs, PMO leads, and cabinet members reconciling an IT portfolio against strategic priorities.

## What’s in the recipe

- README (this file) — orients a human, configures the agent, onboards a contractor.

- Agent Instructions — the prompt you paste into the AI tool.

- Sample Output — a fully worked example on a fictional institution, so you see the finished shape.

- Input Template — the expected columns, accepted header aliases, and an example row.

## How to run it

1.  Export your IT project register (project, status, budget, spent, owner, mapped strategic-goal ID).

2.  Provide your strategic plan (goal IDs and descriptions). Shape both using the Input Template.

3.  Open your AI assistant, paste the Agent Instructions, and attach your filled template.

4.  Review the workbook against the Sample Output. Confirm mappings with project owners.

5.  Decide — the recipe is scaffolding for a portfolio-governance decision, not the decision.

## Configuration — the knobs that make it yours

Defaults are set for a small institution. Override in the Input Template’s Config tab if your scale differs:

- Goal set: SG1–SG7 (edit to your plan)

- Orphan rule: project with blank/none goal ID

- Coverage rule: goal with zero projects = uncovered

- Scope: include planned + in-progress + complete

## What it deliberately does NOT do

- It doesn’t reprioritize, fund, or cancel projects — those are governance decisions.

- Alignment is a mapping, not a verdict on a project’s merit.

- It doesn’t evaluate delivery quality; it reads status as reported.

- It doesn’t rename your data silently. Unmapped projects are flagged.

## /help

If you are holding this recipe with no author in the room, here is the orientation:

- help — what this is: an alignment recipe that maps IT projects to strategic goals and returns an alignment workbook.

- help inputs — what it needs: a project register with goal IDs and a strategic plan (the Input Template shows the shape).

- help outputs — what it gives: a five-tab workbook; the human-legible source of truth is that workbook, not any hidden state.

- help trust — how far to lean on it: recommendations are labelled \[R\]/\[I\]/\[J\]; the Sources & Methodology tab shows every rule. Mapping, not a merit verdict.

Built by Renee Handy · Higher Ed AI Cookbook · build 2026-07. The human-legible source of truth is the returned workbook, not any hidden state. Before you trust this agent with a real decision, find a competent human — a CIO or PMO lead — and have them check the read against your institution’s reality. An orphaned agent should point you at a person, not at itself.

*License: free to use and adapt for your own institution. White-label / resale rights reserved — contact the Cookbook. Sample data is fictional.*

---

## Files in this recipe

- [`ITS_Agent_Instructions.docx`](ITS_Agent_Instructions.docx)
- [`ITS_Input_Template.xlsx`](ITS_Input_Template.xlsx)
- [`ITS_README.docx`](ITS_README.docx)
- [`ITS_Sample_Output.xlsx`](ITS_Sample_Output.xlsx)

*This page is generated from the README `.docx`, which remains the source of truth.*
