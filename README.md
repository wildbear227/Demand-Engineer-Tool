# Demand Engineering Artifact Generator
### DoD / Government IT · ISSE + Zero Trust Pipeline · Powered by Google Gemini

> **Status:** Prototype — Pending Organizational Review & Approval

---

## What This Tool Does

Upload a demand or effort document (PDF, Word, or text) and automatically generate **15 professional engineering artifacts** using AI — organized into three groups:

| Group | Artifacts |
|-------|-----------|
| **Engineering** | Risk Register, Constraints & Opportunities, Technical Interview Questions, Kickoff Agenda & Minutes |
| **Resources** | Equipment & Technology List, Networks Affected, Applicable STIGs, Manpower & Resources, Points of Contact |
| **Cyber RMP / Zero Trust** | RMP Executive Overview, ZT Maturity Assessment (DoD ZTMM v2.0), ZT Control Mapping, Security Control Baseline (NIST 800-53 Rev 5), ZT Gap & Remediation Plan, Continuous Monitoring Strategy |

All artifacts use **DoD/Government IT terminology** and reference real frameworks:
- NIST SP 800-53 Rev 5
- NIST SP 800-207 (Zero Trust Architecture)
- DoD Zero Trust Maturity Model v2.0
- CISA Zero Trust Maturity Model
- NIST AI RMF 1.0
- RMF CA-7 / NIST SP 800-137
- DISA STIGs

---

## How to Use It

### 1. Get a Free Gemini API Key
1. Go to [aistudio.google.com](https://aistudio.google.com)
2. Sign in with a Google account
3. Click **Get API Key** → **Create API key**
4. Copy the key

### 2. Open the Tool
Visit the GitHub Pages URL:
```
https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/
```

### 3. Paste Your API Key
- Enter your Gemini API key in the yellow banner at the top
- Click **SAVE KEY**
- Your key stays in browser memory only — never stored, never logged

### 4. Upload Your Demand Document
- Drag and drop a `.txt`, `.pdf`, or `.docx` file onto the upload zone
- Click **RUN AI EXTRACTION** — AI reads and summarizes the document

### 5. Generate Artifacts
- Click **GENERATE** on individual cards, or
- Use **⚡ GENERATE ALL 15 ARTIFACTS AT ONCE**
- Click any card to preview the artifact inline
- Click **⬇ EXPORT** to download as a `.txt` file

---

## Deploying to GitHub Pages (Setup Instructions)

### Step 1 — Create a New GitHub Repo
1. Go to [github.com](https://github.com) → **New repository**
2. Name it: `demand-artifact-generator` (or any name)
3. Set to **Public** (required for free GitHub Pages)
4. Check **Add a README file**
5. Click **Create repository**

### Step 2 — Upload the Files
1. In your new repo, click **Add file → Upload files**
2. Upload `index.html` and `README.md`
3. Commit directly to `main`

### Step 3 — Enable GitHub Pages
1. Go to **Settings → Pages**
2. Under **Source**, select **Deploy from a branch**
3. Branch: `main` / Folder: `/ (root)`
4. Click **Save**
5. Wait ~60 seconds — your URL will appear at the top of the Pages settings

### Step 4 — Share the URL
Your tool is now live at:
```
https://YOUR-USERNAME.github.io/REPO-NAME/
```

Share this URL with your team. Anyone with the link and a Gemini API key can use it — no install required.

---

## Security Notes

- **API keys** are stored in browser session memory only — cleared when the tab closes
- **Document text** is sent to Google's Gemini API for processing — do not upload classified or sensitive documents
- This tool is intended for **UNCLASSIFIED / FOUO** demand documents only
- **Do not use** on SIPRNET or with any classified content
- All AI processing occurs via Google's API — ensure your organization's data handling policies permit use of Google AI services

---

## Technology Stack

| Component | Technology |
|-----------|-----------|
| Frontend | Vanilla HTML / CSS / JavaScript (zero dependencies) |
| AI Backend | Google Gemini 1.5 Flash API |
| Hosting | GitHub Pages (static) |
| Build Process | None — single `index.html` file |

---

## Roadmap (Post-Approval)

- [ ] DOCX export (Word document download)
- [ ] Editable artifact fields before export
- [ ] Manual input form (no document upload required)
- [ ] POA&M generator tied to ZT Gap output
- [ ] SSP section outline generator
- [ ] Ollama backend option for fully offline/intranet use
- [ ] Azure OpenAI backend option for enterprise deployment

---

## Developed By

Cyber Architecture & Systems Engineering  
USSTRATCOM / SCITLS  
*Prototype — For Review and Approval*

---

> **FOR OFFICIAL USE ONLY** — Do not upload classified information to this tool.
