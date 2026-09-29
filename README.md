# Departmental AI Prompt Library & Best Practices

An Educational Framework for Practical Workplace Automation
A curated repository of structured prompt templates and guidelines designed to help non-technical teams (Operations, HR, Marketing, Finance, and Supply Chain) apply Generative AI to daily business workflows safely and effectively.

---

## Table of Contents
- [Core Prompting Framework](#core-prompting-framework)
- [Departmental Prompt Templates](#departmental-prompt-templates)
  - [Operations & HR: Meeting Transcript to Action Items](#operations--hr-meeting-transcript-to-action-items)
  - [Marketing: Multi-Channel Campaign Copy Generator](#marketing-multi-channel-campaign-copy-generator)
  - [Finance & Supply Chain: Unstructured Text to Formatted Data](#finance--supply-chain-unstructured-text-to-formatted-data)
- [Responsible AI & Safety Guidelines](#responsible-ai--safety-guidelines)

---

## Core Prompting Framework

To get consistent and accurate results from AI tools like Claude, Gemini, or ChatGPT, avoid using short or vague requests. Instead, structure every prompt using the 4-Part Framework:

1. Role ([ROLE]): Assign the AI a specific perspective or expertise (e.g., "You are an executive assistant...").
2. Task ([TASK]): Define the exact action you want the AI to perform.
3. Context ([CONTEXT]): Provide background information, raw input text, target audience, or constraints.
4. Output Format ([OUTPUT FORMAT]): Specify the layout, tone, length, or structural requirements (e.g., Markdown table, bulleted list, maximum word count).

Key Concept: Garbage in, garbage out. The clearer your context and constraints, the better the output quality.

---

## Departmental Prompt Templates

### Operations & HR: Meeting Transcript to Action Items

Primary Function: Transforming raw meeting notes or transcripts into structured summaries and clear task assignments.
Best Suited For: Claude or Gemini (ideal for handling large blocks of text).

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

---

### Marketing: Multi-Channel Campaign Copy Generator

Primary Function: Adapting a single product idea or campaign topic into tailored marketing copy across various channels.
Best Suited For: Gemini or Claude.

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

---

### Finance & Supply Chain: Unstructured Text to Formatted Data

Primary Function: Extracting operational data from unstructured sources (emails, vendor notes, chat logs) and converting it into clean, spreadsheet-ready tables.
Best Suited For: Claude, ChatGPT, or Copilot.

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

---

## Responsible AI & Safety Guidelines

Critical Rule for Workplace AI Usage: Always treat public AI platforms as public spaces.

1. Data Confidentiality:
   - Never input sensitive personal data (e.g., government IDs, phone numbers, personal addresses).
   - Do not input confidential company information, proprietary code, passwords, or financial records into unvetted tools.

2. Verification & Fact-Checking:
   - AI models can occasionally output incorrect or fabricated information (hallucinations).
   - Always double-check dates, financial calculations, statistics, and external links before submitting work to stakeholders.

3. Human-in-the-Loop:
   - AI should serve as a draft generator and productivity assistant, not the final decision-maker. Always review, edit, and adjust tone before sending AI-assisted work.
