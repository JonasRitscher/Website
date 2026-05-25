---
title: "About the Project"
description: "Learn more about the vision, origins, and goals of rosa_qda."
layout: "page"
---

## The Vision Behind rosa_qda

Qualitative social research is a core component of social science and humanities studies, as well as practice-based research. However, anyone wishing to analyze qualitative data today (e.g., following Mayring's Qualitative Content Analysis, Grounded Theory, or Bohnsack's Documentary Method) quickly encounters financial barriers: market-leading programs like **MAXQDA** or **Atlas.ti** are proprietary and carry significant licensing costs for students and smaller organizations.

**rosa_qda** aims to fill this gap. Just as **PSPP** represents a free, easily accessible alternative to SPSS in quantitative analysis, rosa_qda aims to offer students and researchers a free qualitative analysis software.

The goal is not to copy the full feature set of commercial giants, but to provide the **essential analysis tools** needed for student and practical research, paired with an outstanding, straightforward user experience.

---

## Why a New Software?

There are already some notable open-source projects in the QDA field:
- **Qualcoder**: Offers excellent analysis and even AI features, but has a very classic, sometimes technically intimidating GUI.
- **OpenQDA** and **ReQual**: Offer great approaches, but are also rather technical in setup or daily usage.

The problem: In fields like **Social Work** or general social sciences, many researchers and students are less tech-savvy. A complicated or technical user interface often prevents open-source software from being adopted.

### Our Approach
* **Familiar Interface:** A clean macOS-style 5-zone layout (macOS MenuBar, ModuleTabs, ActionBar, DocArea with Coding Lanes, RightPanel for Memos) modeled after familiar structures to make onboarding as smooth as possible.
* **Easy Installation:** No complex database setups. The software is packaged as a desktop application and uses local, portable project containers (`.rqda` – a zipped archive of an SQLite database and a media folder).
* **Focus on Essentials:** Clear, well-structured tools instead of overloaded menus.

---

## Who is Behind the Project? (Vibecoding & Social Work)

My name is **Jonas Ritscher**. I am a **social worker** currently writing my Master's thesis in Social Work. Frustrated by the standard academic requirement to purchase expensive proprietary software subscriptions, I decided to build rosa_qda myself.

Since I am not a trained computer scientist, this project is largely **vibecoded**. By collaborating with advanced AI assistants, I have built a sophisticated software architecture:
* **Frontend:** React 18, TypeScript, and Vite 6 implementing a pixel-perfect macOS-Sonoma design.
* **Backend:** Python 3.13 and FastAPI with SQLite (WAL mode) for fast, transaction-safe database operations.
* **Quality Assurance:** A comprehensive test suite with 14 integration tests covering complex data flows and statistical calculations.

This collaboration demonstrates how "Vibecoding" can seamlessly merge practical domain expertise (what do social workers actually need?) with modern, clean software engineering.

---

## Technical Highlights (Already Implemented)

The backend of **rosa_qda** is already fully functional and implements key methodological tools:

* **Case & Variable Management (F-03):** Dynamic case associations and attributes for analysis across sociodemographic variables.
* **Mayring Paraphrasing Tables (F-14):** Specialized workflows for qualitative content analysis (generalization, first and second reduction).
* **Documentary Method (F-40):** Structured recording of formulating and reflecting interpretation for sequence analysis according to Bohnsack.
* **Visual Tools (F-52):** An interactive concept whiteboard, whose layouts can be directly converted into the hierarchical code tree.
* **Text Analysis (F-51):** Word frequency tables with built-in stopword filtering (German/English) and Keyword-in-Context (KWIC) searches.
* **Intercoder Agreement (F-60):** Automated calculation of Cohen's Kappa to verify coding consensus.
* **REFI-QDA Standard (F-61):** Seamless import and export of standardized XML project files (`.qdpx` and `.qdc`) for interoperability with MAXQDA and Atlas.ti.
* **Audit Trail & Changelog (F-62):** Automated logging of all database modifications to ensure scientific rigor and transparency.
