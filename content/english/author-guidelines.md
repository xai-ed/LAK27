---
title: "Author Guidelines"
meta_title: "Author Guidelines — XAI-Ed 2027"
description: "Paper template, formatting rules, and submission checklist for the XAI-Ed 2027 workshop at LAK27 (CEUR-WS CEURART template)"
draft: false
---

Accepted papers of XAI-Ed 2027 will be submitted for publication in the [CEUR Workshop Proceedings](https://ceur-ws.org/) (CEUR-WS.org). CEUR-WS only accepts papers written in its current **one-column CEURART template**, and it has tightened several rules since 2025. Please use the template from your first submission. The steps below take you from template to camera-ready.

| | |
|---|---|
| **Template** | CEURART, one column (LaTeX or LibreOffice) |
| **Full papers** | 10–14 pages, including references |
| **Short papers** | 6–8 pages, including references |
| **Review** | Double-blind, at least two reviewers |
| **Submission deadline** | 4 December 2026 |
| **Camera-ready deadline** | 28 February 2027 |
| **Submit via** | [EasyChair](https://easychair.org/conferences/?conf=xaiedlak2027) |

All dates are listed in the [Call for Papers]({{< relref "cfp" >}}).

### Step 1 — Get the template

Use one of the official CEURART templates below. They are the current version (CEURART V 0.62, July 2026) and already contain everything CEUR-WS checks for, including the licence footnote and the Declaration on Generative AI.

| You write in | Use this template |
|---|---|
| LaTeX on Overleaf (recommended) | [Official CEURART Overleaf template](https://www.overleaf.com/latex/templates/template-for-submissions-to-ceur-workshop-proceedings-ceur-ws-dot-org/wqyfdgftmcfw). Choose *Open as Template*. Overleaf already has the required fonts. |
| LaTeX on your own computer | [CEURART.zip](https://ceur-ws.org/Vol-XXX/CEURART.zip) (contains the LaTeX class and the LibreOffice template) |
| LibreOffice Writer | [CEUR-Template-1col.odt](https://ceur-ws.org/Vol-XXX/CEUR-Template-1col.odt) |

More background and sample papers are on the [CEUR-WS template page](https://ceur-ws.org/Vol-XXX/).

**Fonts.** The template requires the **Libertinus** font family.

- LaTeX on your own computer: use TeX Live 2020 or later and install the fonts, for example with `tlmgr install libertinus libertinus-fonts libertinus-otf libertinus-type1` (Windows/macOS) or `sudo apt install texlive-fonts-extra` (Linux).
- LibreOffice: install Libertinus on your computer before you open the template. The template explains how.

**Please don't use:**

- **Microsoft Word or Microsoft 365.** CEUR-WS advises against them because they tend to produce PDFs it cannot accept. Do not open the ODT template in Word. If you cannot use LaTeX, use LibreOffice.
- **Cloud editors** such as Google Docs or Office Online. They cannot use the Libertinus font.
- **The old two-column layout**, or the `twocolumn` option of the LaTeX class. CEUR-WS stopped accepting two-column papers in 2025.
- **Older copies of the template**, such as Overleaf copies made by other conferences or the old `CEUR-Template-1col.docx` Word file. Many are out of date and lack the Declaration on Generative AI.

### Step 2 — Set up page 1

Replace the template's sample metadata with the lines below. The conference line and copyright year must be identical in every paper of our volume and must match the author agreement, so please copy them exactly.

```latex
\documentclass{ceurart}   % one column; do not add twocolumn or hf

\copyrightyear{2027}
\copyrightclause{Copyright for this paper by its authors.
  Use permitted under Creative Commons License Attribution 4.0
  International (CC BY 4.0).}

\conference{XAI-Ed 2027: 4th International Workshop on Explainable AI
  in Education, co-located with the 17th International Learning
  Analytics and Knowledge Conference (LAK27), March 2027,
  Recife, Brazil}

\title{Your Paper Title in Title Case}

\author[1]{Firstname Lastname}[%
  orcid=0000-0000-0000-0000,
  email=firstname.lastname@university.edu,
]
\cormark[1]
\address[1]{Department, University, City, Country}
\cortext[1]{Corresponding author.}

\begin{keywords}
  explainable AI \sep
  learning analytics \sep
  your keyword
\end{keywords}
```

If you use the LibreOffice template, put the same conference text in the first-page footnote and set the copyright year to 2027. In both templates, the bottom of page 1 should read:

> *XAI-Ed 2027: 4th International Workshop on Explainable AI in Education, co-located with the 17th International Learning Analytics and Knowledge Conference (LAK27), March 2027, Recife, Brazil*<br>
> \* Corresponding author.<br>
> © 2027 Copyright for this paper by its authors. Use permitted under Creative Commons License Attribution 4.0 International (CC BY 4.0).

For the review version, replace the author block as described in [Step 5](#step-5--anonymise-for-double-blind-review).

### Step 3 — Formatting rules

**Do:**

- Write the title in **Title Case**, so that all titles in the volume match.
- Give every author's full name (*Maria Silva*, not *M. Silva*). Check the spelling against [DBLP](https://dblp.org/) if the author is listed there. Transliterate non-Latin names into Latin script.
- Give each affiliation with organisation, city, and country. Add ORCID iDs where available.
- Write in English.

**Don't:**

- Change margins, font sizes, line spacing, or list styles.
- Use `\vspace` or similar tricks to gain space.
- Add page numbers, headers, or footers (the `hf` option).
- Remove or reword the CC BY 4.0 licence footnote.
- Include figures created with generative AI (see [Step 4](#step-4--declaration-on-generative-ai)).

XAI-Ed accepts two types of submissions: full papers and short papers. Stay within the page limit for your submission type. The limits are counted in the CEURART template and **include references**.

| Submission type | Pages |
|---|---|
| Full paper | 10–14 |
| Short paper | 6–8 |

CEUR-WS also classifies papers by "standard pages" of 2,500 characters (about 380–400 words). It lists papers with 10 or more standard pages as regular papers and papers with 5–9 standard pages as short papers.

### Step 4 — Declaration on Generative AI

CEUR-WS requires every paper to include a section titled **Declaration on Generative AI**, placed after the acknowledgements and before the references. It is required **even if you used no AI tools**. The template already contains the section. Keep the version that applies and delete the other.

If you used no generative AI tools:

```latex
\section*{Declaration on Generative AI}
The author(s) have not employed any Generative AI tools.
```

If you used generative AI tools (edit the tools and tasks):

```latex
\section*{Declaration on Generative AI}
During the preparation of this work, the author(s) used ChatGPT and
Grammarly in order to: Grammar and spelling check; Paraphrase and
reword. After using these tools/services, the author(s) reviewed and
edited the content as needed and take(s) full responsibility for the
publication's content.
```

- Name **every** tool you used, and describe each task with the activities of the CEUR-WS [GenAI Usage Taxonomy](https://ceur-ws.org/GenAI/Taxonomy.html), for example *Grammar and spelling check*, *Paraphrase and reword*, *Improve writing style*, or *Text translation*.
- **Acceptable:** checking grammar and spelling, rephrasing your own sentences, and translating text that you then check and edit.
- **Not acceptable:** generating new text, such as paragraphs or whole sections, and generating diagrams, charts, or illustrations. AI-generated images are only allowed when image generation is the topic of the paper.
- AI tools cannot be listed as authors.

Please read the full [CEUR-WS Policy on AI-Assisting Tools](https://ceur-ws.org/GenAI/Policy.html). CEUR-WS removes published papers that violate it.

### Step 5 — Anonymise for double-blind review

The CEURART template has no anonymous mode and shows the authors on page 1, so the version you submit for review needs a few temporary changes. Keep the conference line, copyright footnote, and Declaration on Generative AI as they are.

```latex
\author[1]{Anonymous Author(s)}
\address[1]{Anonymous Institution, Country}
```

- Remove names, emails, ORCID iDs, and affiliations, and delete the `\cormark` and `\cortext` lines.
- Leave out the acknowledgements and any funding or project names.
- Cite your own earlier work in the third person (*"Silva et al. [4] showed…"*, not *"In our previous work [4]…"*).
- Remove identifying links (for example to GitHub repositories or project pages) or replace them with an anonymised version.
- Check the PDF's document properties: the author field must be empty.

### Step 6 — Submit

Upload your PDF to [EasyChair](https://easychair.org/conferences/?conf=xaiedlak2027) by **4 December 2026**. Before you upload, check that:

- [ ] The paper uses the official one-column CEURART template (LaTeX or LibreOffice, not Word), with the layout unchanged.
- [ ] Page 1 shows the XAI-Ed 2027 conference line and the © 2027 CC BY 4.0 footnote.
- [ ] The title is in Title Case.
- [ ] The paper has a **Declaration on Generative AI** section before the references.
- [ ] No text or figures were generated with AI.
- [ ] The length, including references, is within the limit for your submission type (full paper: 10–14 pages; short paper: 6–8 pages).
- [ ] The paper is anonymised: no names, affiliations, acknowledgements, identifying links, or PDF author metadata.
- [ ] All fonts are embedded in the PDF (the official templates do this by default).

### Step 7 — After acceptance: camera-ready version

Upload the final version by **28 February 2027**. This is the version CEUR-WS will publish. After publication, only typos in the title, author names, and affiliations can be corrected, and only within two working days, so please check it carefully.

- Restore the full author block: full names, affiliations with country, emails, and ORCID iDs.
- Add back the acknowledgements and funding information.
- Address the reviewers' comments, keeping the template and the conference line unchanged.
- Update the Declaration on Generative AI if anything changed during the revision.
- Check that the title and author names in EasyChair exactly match the PDF.

**Author agreement.** For each paper, one author signs a CEUR-WS author agreement on behalf of all authors. Please download a fresh copy, since CEUR-WS revised the forms in September 2026:

- [No third-party material (NTP)](https://ceur-ws.org/ceur-author-agreement-ccby-ntp.pdf?ver=2026-09-03): for most papers, where all text, figures, and data are your own.
- [Third-party material (TP)](https://ceur-ws.org/ceur-author-agreement-ccby-tp.pdf?ver=2026-09-03): if your paper or its accompanying material reuses copyrighted material from others. Attach a copy of each permission.

**The agreement must be signed by hand with a pen on paper.** Print the form, sign it, and send a scan or photo of it as PDF or JPG. CEUR-WS does not accept typed signatures, pasted signature images, or signatures drawn with a digital pen or on a touchscreen. Write the event name on the form exactly as:

```text
XAI-Ed 2027: 4th International Workshop on Explainable AI in Education
```

We will send instructions on where to upload the camera-ready version and the signed agreement with the acceptance notification.

---

Questions about the template or the submission process? Please contact the [organisers]({{< relref "organisers" >}}).

*Based on the CEUR-WS requirements as of October 2026: [Publishing at CEUR-WS.org](https://ceur-ws.org/HOWTOSUBMIT.html) · [CEURART template page](https://ceur-ws.org/Vol-XXX/) · [Policy on AI-Assisting Tools](https://ceur-ws.org/GenAI/Policy.html).*
