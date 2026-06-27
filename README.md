Automated Lead Scoring & Tagging (n8n)
<img width="959" height="413" alt="image" src="https://github.com/user-attachments/assets/a62a56b4-defe-4f0d-ac31-3d600535f555" />


An end-to-end n8n automation built for Salesifyme that replaces manual lead triage with instant, consistent lead qualification — scored against a weighted Ideal Customer Profile (ICP) across a database of ~37,000 leads.

Problem

Sales teams were manually reviewing and prioritizing leads from a growing Excel-based database. This doesn't scale — leads sit untouched, hot prospects get buried, and prioritization is inconsistent across reps.

What it does

Ingests lead data directly from an Excel/Google Sheets-based lead database
Scores each lead against a weighted ICP using custom JavaScript logic inside n8n Function nodes
Weighted criteria include:

Industry fit
Role / seniority
Geographic location



Auto-tags each lead (e.g. Hot / Warm / Cold) based on the computed composite score
Writes scored, tagged results back to the sheet — ready for sales to act on immediately, with no manual review step


Why it matters

Instead of a rep manually skimming thousands of rows, every lead is scored the moment it enters the sheet. Reps see a ranked, tagged list instead of a flat spreadsheet — turning a multi-hour weekly task into something that happens automatically in the background.

Stack


n8n — workflow orchestration
JavaScript (n8n Function nodes) — weighted ICP scoring logic
Google Sheets / Excel — lead data source and output
Custom JSON config defining ICP weights and thresholds


Scale

Built and tested against a live lead database of approximately 37,000 rows, with scoring logic designed to run reliably at that volume without manual intervention.
