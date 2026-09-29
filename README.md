# Departmental AI Prompt Library & Best Practices

An Educational Framework for Practical Workplace Automation

A curated repository of structured prompt templates and guidelines designed to help teams (Operations, HR, Marketing, Finance, and Supply Chain) apply AI to daily business workflows safely and effectively.

---

## Table of Contents

1. [Core Prompting Framework](#core-prompting-framework)
2. [Departmental Prompt Templates](#departmental-prompt-templates)
   - [Operations & HR](#operations--hr)
   - [Marketing](#marketing)
   - [Finance & Supply Chain](#finance--supply-chain)
3. [Responsible AI & Safety Guidelines](#responsible-ai--safety-guidelines)

---

## Core Prompting Framework

To achieve consistent and accurate results from AI tools like Claude, Gemini, or ChatGPT, structure every request using the **4-Part Framework**:

* **Role (`[ROLE]`):** Assign the AI a specific perspective or domain expertise (e.g., *"You are an executive assistant..."*).
* **Task (`[TASK]`):** Define the precise action or objective you want the AI to perform.
* **Context (`[CONTEXT]`):** Provide background information, raw input text, target audience, or constraints.
* **Output Format (`[OUTPUT FORMAT]`):** Specify the layout, tone, length, or structural rules (e.g., Markdown table, bullet points, maximum word count).

> **Key Takeaway:** *Garbage in, garbage out.* Clear context and explicit constraints directly drive output quality.

---

## Departmental Prompt Templates

### Operations & HR

**Template Name:** Meeting Transcript to Action Items

**Primary Function:** Transforms raw meeting notes or transcripts into structured summaries and actionable task assignments.

**Recommended Models:** Claude or Gemini (optimized for long-context inputs)

```text
[ROLE]
You are an Operations Executive Assistant specializing in process efficiency and project tracking.

[TASK]
Analyze the provided meeting notes and generate an executive summary along with a structured action item table.

[CONTEXT]
Meeting Title: [Insert Meeting Title]
Date & Participants: [Insert Date / Attendees]
Raw Notes / Transcript:
---
[Paste meeting notes or transcript here]
---

[OUTPUT FORMAT]
Please format your response strictly as follows:

1. Executive Summary: 2–3 sentences highlighting the main objective and primary outcome.
2. Key Decisions: Bullet points of all major decisions agreed upon during the meeting.
3. Action Items Table: Return a Markdown table with the following columns:
   | Task Description | Owner | Deadline | Priority (High/Medium/Low) |
```

---

### Marketing

**Template Name:** Multi-Channel Campaign Copy Generator

**Primary Function:** Adapts a single product concept or campaign topic into tailored marketing copy across multiple channels.

**Recommended Models:** Gemini or Claude

```text
[ROLE]
You are a Digital Copywriter specializing in cross-channel brand campaigns.

[TASK]
Create multi-channel promotional copy based on the provided brief.

[CONTEXT]
Campaign/Product Name: [Insert Name]
Target Audience: [Insert Audience Demographics/Interests]
Core Message / Offer: [Insert Key Value Proposition]

[OUTPUT FORMAT]
Generate distinct copy for the following three formats:

1. Instagram Caption:
   - Engaging hook line
   - Body text under 100 words
   - Clear Call-to-Action (CTA)
   - 3 to 5 relevant hashtags

2. Email Newsletter:
   - 2 subject line options (max 50 characters each)
   - Structured body text (150–200 words) focusing on problem-solution-action

3. Broadcast Announcement:
   - 2 concise, professional paragraphs suitable for internal or community channels
```

---

### Finance & Supply Chain

* **Template Name:** Unstructured Text to Formatted Data

**Primary Function:** Extracts operational data from unstructured sources (emails, vendor notes, chat logs) and converts it into spreadsheet-ready tables.

**Recommended Models:** Claude, ChatGPT, or Copilot

```text
[ROLE]
You are a Data Operations Specialist converting raw business communication into structured data.

[TASK]
Extract key transactional details from the raw text provided below and format them into a clean tabular structure.

[CONTEXT]
Source Text:
---
[Paste unstructured email thread, vendor notes, or receipt text here]
---

[OUTPUT FORMAT]
Return ONLY a Markdown table with the following headers:
| Date | Vendor/Supplier | Item Description | Quantity | Unit Price | Total Cost | Status |

Rules:
- If a specific field is missing in the raw text, write "N/A".
- Ensure numbers and currency are standardized.
- Do not include any introductory or concluding text outside the table.
```
* **Template Name:** Vendor Delivery Risk & Anomaly Assessment

**Primary Function:** Review the provided logistics notes or tracking logs and identify potential delivery risks, operational impacts, and suggested mitigation steps.

**Recommended Models:** Claude, ChatGPT, or Copilot

```text
[ROLE]
You are a Supply Chain Risk Analyst monitoring vendor performance and fulfillment timelines.

[TASK]
Review the provided logistics notes or tracking logs and identify potential delivery risks, operational impacts, and suggested mitigation steps.

[CONTEXT]
Purchase Order / Shipment Ref: [Insert PO or Tracking Number]
Vendor Name: [Insert Vendor Name]
Logistics Status / Tracking Notes:
---
[Paste shipment tracking logs, email status updates, or delay notices here]
---

[OUTPUT FORMAT]
Provide a structured assessment as follows:

1. Risk Summary: 2 sentences explaining the current delay or status.
2. Impact Severity: Classify as High, Medium, or Low with a brief justification.
3. Identified Bottlenecks: Bulleted list of root causes indicated in the log.
4. Recommended Actions: Bulleted list of immediate steps for the logistics team (e.g., rerouting, contacting alternate suppliers, updating inventory timelines).
```


---

## Responsible AI & Safety Guidelines

> **Golden Rule:** Always treat public AI platforms as public spaces.

### 1. Data Confidentiality
* Do not enter sensitive personal identifiable information (e.g., government IDs, phone numbers, addresses).
* Never input confidential company information, proprietary code, credentials, or unannounced financial records.

### 2. Verification & Fact-Checking
* AI models can generate plausible yet incorrect or fabricated information (hallucinations).
* Always verify dates, numerical calculations, statistics, and external links before circulating outputs.

### 3. Human-in-the-Loop
* Use AI as a draft generator and productivity multiplier, not the final decision-maker.
* Always review, refine, and validate AI outputs prior to final execution
