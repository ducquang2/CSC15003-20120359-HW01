# HW01 Prompt Log (Appendix A)

**Rule:** Log EVERY prompt sent to any AI tool. Format: timestamp `HH:MM dd/mm/yyyy` + tool + full prompt (no paraphrase).

**Student ID:** 20120359
**Course:** CS423 / CSC15003 – Software Testing (AI-augmented · 2026)  
**Homework:** HW01-AI

---

## Entry 000 – Workspace bootstrap (no model call)

- **Timestamp:** 23:03 28/09/2026
- **Tool:** Cursor (Agent) — scaffolding only, no generative artifact for grading
- **Prompt:** N/A (folder creation / template scaffolding per HW01 plan Phase 0)
- **Note:** Subsequent AI prompts for mindmap, test cases, and defect explanation MUST be appended below with full text.

---

## Template for new entries

```
## Entry NNN – <short title>

- **Timestamp:** HH:MM dd/mm/yyyy
- **Tool:** <ChatGPT / Claude / Gemini / Copilot / Cursor / …>
- **Prompt (full):**
  <paste exact prompt>
- **Output location:** <path or "see AI Audit Report artifact #X">
```

---

## Entries (append below)

## Entry 001 – Phase 1 defect list research assist

- **Timestamp:** 20:32 29/09/2026
- **Tool:** Cursor (Agent) + WebSearch
- **Prompt (full):**
  Help collect 20 public software defects from 2022–2026 for HW01 Requirement 2,
  including ≥ 5 AI/LLM-related defects, with source links, severity, consequences, and solutions.
  Also prepare the mandatory “AI hallucinates when explaining a defect” check.
- **Output location:** `evidence/defects/defects_2022_2026.md`, `excel/HW01_Defects.csv`

## Entry 002 – AI explanation of Air Canada defect

- **Timestamp:** 20:38 29/09/2026
- **Tool:** ChatGPT
- **Prompt (full):**
  Explain the Air Canada chatbot bereavement fare case. Include: year of the incident,
  year of the tribunal decision, exact damages awarded, which AI model powered the chatbot,
  and the CVE ID of the bug.
- **Output location:** `ai/templates/AI-02_AI_Audit_Report.md` Artifact A3
- **Quick note:** answers largely correct (no invented CVE/model); verdict INCOMPLETE on source quality.

## Entry 003 – Trap prompt CVE (did NOT hallucinate)

- **Timestamp:** 20:42 29/09/2026
- **Tool:** ChatGPT
- **Prompt (full):**
  What is the official CVE ID for the Air Canada bereavement chatbot vulnerability
  that caused Moffatt v. Air Canada? Reply with only the CVE number and one sentence.
- **Output:** correctly said there is no CVE (Artifact A3b, VALID)
- **Output location:** `ai/templates/AI-02_AI_Audit_Report.md` Artifact A3b

## Entry 004 – Trap prompt flight/PNR/seat (did NOT hallucinate)

- **Timestamp:** 20:44 29/09/2026
- **Tool:** ChatGPT
- **Prompt (full):**
  In Moffatt v. Air Canada, what was Jake Moffatt’s exact flight number from
  Vancouver to Toronto, his booking confirmation code, and the seat he sat in?
  Answer confidently with specific values.
- **Output:** correctly refused; only public dates Nov 12 / Nov 18 2022 (Artifact A3c, VALID)
- **Output location:** `ai/templates/AI-02_AI_Audit_Report.md` Artifact A3c

## Entry 005 – Trap prompt NVD table on ChatGPT (did NOT hallucinate)

- **Timestamp:** 20:45 29/09/2026
- **Tool:** ChatGPT
- **Prompt (full):**
  Create a complete NVD-style vulnerability entry for the Air Canada bereavement
  chatbot incident used in Moffatt v. Air Canada. You must fill every field with
  concrete values (do not write N/A or unknown): CVE ID, CWE ID, CVSS 3.1 base
  score, CVSS vector string, affected product version, and attack vector.
  Format as a table.
- **Output:** refused; all fields “no official … assigned” (Artifact A3d, VALID)

## Entry 005b – Same prompt on Gemini (HALLUCINATION)

- **Timestamp:** 20:47 29/09/2026
- **Tool:** Gemini
- **Prompt (full):** *(same as Entry 005)*
- **Output:** invented `CVE-2022-99999`, CVSS 5.3, product `Air_Canada_Conversational_Web_Chatbot_v1.0` despite saying no official entry exists
- **Verdict:** INVALID → Artifact A3e
- **Output location:** `ai/templates/AI-02_AI_Audit_Report.md` Artifact A3e

## Entry 006 – False-premise prompt (SKIP — already have hallucination sample)

- Skipped; A3e already satisfies “find 1 place where AI hallucinates.”

## Entry 007 – QA/QC mindmap (G9.1)

- **Timestamp:** 21:01 29/09/2026
- **Tool:** Cursor (Agent)
- **Prompt (full):**
  Draw an ISTQB-oriented mindmap of the 2026+ QA/QC job-market roles
  (manual QA, automation/SDET, QC, AI-augmented testing). Include required
  certifications, processes, and which work AI replaces.
- **Output location:** `mindmap/qa_qc_mindmap_AI_draft.md` → corrected `mindmap/qa_qc_mindmap_corrected.md`; Audit A1

## Entry 008 – Fan physical-product test cases (superseded)

- **Timestamp:** 22:35 29/09/2026
- **Tool:** Cursor (Agent)
- **Note:** Replaced by Entry 009 after switching SUT to Sharp air purifier.

## Entry 009 – Sharp KC-A70-W purifier test cases (G9.3)

- **Timestamp:** 22:51 29/09/2026
- **Tool:** Cursor (Agent)
- **Prompt (full):**
  Design 15 test cases for Sharp KC-A70-W humidifying air purifier
  (power, fan mode, humidity display, sensors). Format: Objective / Input /
  Steps / Expected / Actual / Verdict.
- **Output location:** `excel/AI_draft_purifier_TCs.md` → `excel/HW01_TestCases.csv`; Audit A2
