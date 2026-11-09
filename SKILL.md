---
name: al-legal-mcp-skill
description: Official Albania (AL) legislation, multi-tier court precedent research, and citation verification skill.
version: 2.0.0
author: JurisAtlas
license: MIT
---

# Albania Legal Research & Multi-Tier Case Law Skill (`al-legal-mcp`)

Use this skill whenever the user asks a legal question, drafts a pleading or contract, or researches case law across any judicial instance in **Albania (AL)**.

## Verification & Research Rules

1. **Citation Verification:** Never fabricate a statutory provision or case citation. Query `search_legislation`, `search_case_law`, `search_tiered_court_decisions`, or `verify_citation` before citing any authority (e.g., `Vendimi Nr. 123/2024 or Fletorja Zyrtare Nr. 15/2024`).
2. **Multi-Tier Judicial Coverage:**
   - **First Instance (Trial / Municipal / District):** Gjykatat e Shkallës së Parë të Juridiksionit të Përgjithshëm (13 District First Instance Courts), Gjykatat Administrative të Shkallës së Parë & GJKKO
   - **Second Instance (Cantonal / Regional / Appellate):** Gjykata e Apelit të Juridiksionit të Përgjithshëm (Tiranë), Gjykata Administrative e Apelit & Gjykata e Posaçme e Apelit
   - **Supreme & Constitutional Instance:** Gjykata e Lartë e Republikës së Shqipërisë (gjykataelarte.gov.al) & Gjykata Kushtetuese (gjk.gov.al)
   - **Primary Tiered Database:** Portali Gjyqësor Kombëtar Gjykatat.gov.al & Gjykata e Lartë Unifying Decisions (`https://gjykatat.gov.al`)
