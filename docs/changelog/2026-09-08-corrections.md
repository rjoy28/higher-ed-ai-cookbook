# Corrections applied 2026-09-08

Follow-up to SCRUB_CHANGELOG.md. Two issues, both resolved in this bundle.

## 1. Formula caches restored (16 workbooks)
The lead scorecard sheets are formula-driven (they pull from detail sheets and compute
status via IF logic). The scrub re-saved changed files with openpyxl, which strips cached
formula values; only recipes 02/03/07 were recalculated afterward. The rest therefore
rendered BLANK in any viewer that does not recalculate — breaking the "reads correctly
outside Excel" property.

Fix: every Sample_Output.xlsx recalculated headless (LibreOffice). Result: 0 formula
errors across all 17. No values changed — the formulas were always correct; only the
cached results were missing.

## 2. Brand/Media (12) outlet names de-identified
The Clip Log named real news organizations and attributed invented coverage to them,
including negative sentiment. Earned-media outlet names replaced with outlet TYPES;
owned/RCU channels left as factual self-reference. 19 cells changed.

Seven earned-media outlets became outlet types: national Christian magazine,
denominational news service, higher-education trade publication, regional public radio,
local alt-weekly, network TV affiliate, athletic conference release.
Owned channels (RCU social accounts, alumni magazine, RCU News, President's Blog,
local blog) left unchanged. Original names intentionally not recorded.

Verified: Coverage Scorecard (Owned 20 / Earned 22) and Topics & Sentiment aggregates
are identical before and after — no figure depends on outlet names.
