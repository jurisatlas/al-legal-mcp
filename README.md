# Albania Legal Research MCP Server (`al-legal-mcp`)

**[Shqip](#lang-sq) | [English Documentation](#english-documentation)**

---

<a id="lang-sq"></a>
## Serveri Ligjor MCP (`al-legal-mcp`) — Shqip

### Rreth këtij depoje (Repository)

Ky depo përmban serverin Model Context Protocol (MCP) që lidh aplikacionin tuaj të inteligjencës artificiale (Claude Desktop, Cursor, Windsurf, VS Code / Copilot, Cline ose Antigravity) me fletoret zyrtare dhe bazat e të dhënave të vendimeve gjyqësore për **Albania** (gjykatat e shkallës së parë / themelore, gjykatat e apelit dhe gjykatat e larta / supreme e kushtetuese).

### Instalimi i shpejtë (Zgjedhja e aplikacionit AI)

1. **Shkarkimi:** Klikoni **`<> Code` -> `Download ZIP`** dhe nxirrni dosjen në kompjuterin tuaj.
2. **Nisja e instaluesit:** Klikoni dy herë mbi **`Click_Here_To_Install_Windows.bat`** (Windows) ose **`Click_Here_To_Install_Mac.command`** (macOS).
3. **Zgjedhja e AI:** Zgjidhni programet AI që përdorni (Claude, Cursor, Windsurf, VS Code, Antigravity), klikoni butonin e instalimit dhe rinisni aplikacionin tuaj AI.

**Shënim sigurie:** Ky mjet funksionon vetëm në mënyrë leximi (read-only) dhe nuk prek ose ndryshon asnjë skedar personal në kompjuterin tuaj.

### Shkallët e gjyqësorit dhe burimet zyrtare

| Shkalla gjyqësore | Gjykatat e mbuluara |
|:---|:---|
| **Shkalla e Parë** | Gjykatat e Shkallës së Parë të Juridiksionit të Përgjithshëm (13 District First Instance Courts), Gjykatat Administrative të Shkallës së Parë & GJKKO |
| **Gjykatat e Apelit** | Gjykata e Apelit të Juridiksionit të Përgjithshëm (Tiranë), Gjykata Administrative e Apelit & Gjykata e Posaçme e Apelit |
| **Gjykata e Lartë / Supreme & Kushtetuese** | Gjykata e Lartë e Republikës së Shqipërisë (gjykataelarte.gov.al) & Gjykata Kushtetuese (gjk.gov.al) |

- **Qendra e Botimeve Zyrtare - QBZ (qbz.gov.al Official Publications Center):** [https://qbz.gov.al](https://qbz.gov.al) (`qbz.gov.al`, `parlament.al`, `drejtesia.gov.al`)
- **Portali Gjyqësor Kombëtar Gjykatat.gov.al & Gjykata e Lartë Unifying Decisions:** [https://gjykatat.gov.al](https://gjykatat.gov.al) (`gjykataelarte.gov.al`, `gjk.gov.al`, `gjykatat.gov.al`)

---

<a id="english-documentation"></a>
## English Documentation

Model Context Protocol (MCP) server providing live, read-only access to **Albania (AL)** legislation, official gazettes, multi-tier judicial decisions (First Instance, Regional/Cantonal/Appellate, and Supreme/Constitutional courts, including HTML and PDF full-text extraction), and statutory citation verification across all major AI clients (**ChatGPT Desktop, OpenAI Codex CLI, Claude Desktop, Claude Code CLI, Cursor, Windsurf, VS Code / GitHub Copilot / Cline / Roo Code, Google Antigravity / Gemini CLI, Perplexity, and Continue.dev**).

---

### Interactive Desktop Setup (Select Your AI Assistant)

This package includes a graphical installer for legal practitioners and non-technical users that lets you select which AI application(s) you use:

1. **Download:** Click **`<> Code`** at the top right of this repository, select **`Download ZIP`**, and extract the folder to your computer.
2. **Run the Setup Utility:**
   - **Windows:** Double-click `Click_Here_To_Install_Windows.bat`
   - **macOS:** Double-click `Click_Here_To_Install_Mac.command`
3. **Select Your AI Client(s) & Connect:** Check the box(es) for the AI assistant(s) installed on your computer (**ChatGPT Desktop & OpenAI Codex CLI**, **Claude Desktop & Claude Code CLI**, **Cursor**, **Windsurf**, **VS Code / GitHub Copilot / Cline / Roo Code**, **Google Antigravity / Gemini CLI**, or **Perplexity / Continue.dev**), click **Install to Selected AI Clients**, and restart your selected AI application.

**System Integrity Note:** The setup utility operates strictly in read-only mode with respect to your personal files and documents. It installs an isolated Python runtime inside the extracted folder and registers the server entry only in the AI client configuration files you select.

---

### Multi-Tier Judicial Hierarchy & Live Indexed National Archives

This server performs live queries across the full judicial hierarchy and official legal archives of **Albania**, extracting full text from both HTML pages and official court/gazette PDF judgments:

| Judicial Tier | Covered Courts & Tribunals |
|:---|:---|
| **Tier 1 — First Instance** | Gjykatat e Shkallës së Parë të Juridiksionit të Përgjithshëm (13 District First Instance Courts), Gjykatat Administrative të Shkallës së Parë & GJKKO |
| **Tier 2 — Regional / Cantonal / Appellate** | Gjykata e Apelit të Juridiksionit të Përgjithshëm (Tiranë), Gjykata Administrative e Apelit & Gjykata e Posaçme e Apelit |
| **Tier 3 — Supreme & Constitutional** | Gjykata e Lartë e Republikës së Shqipërisë (gjykataelarte.gov.al) & Gjykata Kushtetuese (gjk.gov.al) |

#### Official Portals & Live Indexed Domains

- **National Legislation & Official Gazette:** Qendra e Botimeve Zyrtare - QBZ (qbz.gov.al Official Publications Center) — [https://qbz.gov.al](https://qbz.gov.al)
  - *Indexed Legislation Domains:* `qbz.gov.al`, `parlament.al`, `drejtesia.gov.al`
- **Court Decisions & Jurisprudence Archives:** Portali Gjyqësor Kombëtar Gjykatat.gov.al & Gjykata e Lartë Unifying Decisions — [https://gjykatat.gov.al](https://gjykatat.gov.al)
  - *Indexed Judicial & Open Case Law Domains:* `gjykataelarte.gov.al`, `gjk.gov.al`, `gjykatat.gov.al`

---

### Available MCP Tools

| Tool | Description |
|:---|:---|
| `search_legislation` | Searches enacted statutes, codes, decrees, and official gazette publications in Albania. |
| `search_case_law` | Searches national jurisprudence and open judicial archives for Albania. |
| `search_tiered_court_decisions` | Filters case law specifically by judicial instance (`first_instance`, `appellate_regional`, `supreme_constitutional`) or specific regional/cantonal/district court. |
| `list_court_hierarchy` | Returns the complete 3-tier court structure and supported regional court filters for Albania. |
| `get_legal_document_markdown` | Retrieves full statutory or judicial texts (both HTML and official `.pdf` court judgments) and converts them into clean Markdown. |
| `verify_citation` | Validates statutory and case law citations against official registries. |

---

<details>
<summary><b>Manual Configuration for Developers (Optional)</b></summary>

```json
{
  "mcpServers": {
    "al-legal-mcp": {
      "command": "uvx",
      "args": [
        "--from",
        "https://github.com/jurisatlas/al-legal-mcp/archive/refs/heads/main.zip",
        "al-legal-mcp"
      ]
    }
  }
}
```
</details>
