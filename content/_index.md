---
title: "rosa_qda — Free QDA Software"
description: "The user-friendly open-source alternative to MAXQDA & Co. for qualitative social research."
layout: "page"
---

{{< lead >}}
A **free, user-friendly open-source alternative** to proprietary software like MAXQDA and Atlas.ti – specifically developed for students and researchers in the social sciences.
{{< /lead >}}

<div class="flex flex-wrap gap-4 my-8 justify-center">
  {{< button href="https://github.com/JonasRitscher/rosa_qda" target="_blank" icon="github" >}}
    Go to GitHub Repository
  {{< /button >}}
  {{< button href="about/" outline=true >}}
    More About the Project
  {{< /button >}}
</div>

---

## Why rosa_qda?

Proprietary QDA (Qualitative Data Analysis) tools are often unaffordable for students and independent researchers. While great open-source projects like *Qualcoder* or *OpenQDA* exist, their user interfaces (GUIs) are often highly technical and intimidating.

**rosa_qda** bridges this gap: It combines a **macOS-Sonoma-inspired, intuitive GUI** (built with React 18 & TypeScript) with a **robust, transaction-safe Python backend** (FastAPI & SQLite). The focus is on making qualitative analysis accessible and straightforward, even for computer-averse users.

---

## Core Features

<div class="grid grid-cols-1 md:grid-cols-3 gap-6 my-8">
  <div class="p-6 border rounded-xl dark:border-neutral-800 bg-neutral-50 dark:bg-neutral-900 shadow-sm hover:shadow-md transition-shadow">
    <div class="text-3xl mb-3 text-primary-500">{{< icon "wand-magic-sparkles" >}}</div>
    <h3 class="text-xl font-bold mb-2">Modern GUI (React)</h3>
    <p class="text-sm text-neutral-600 dark:text-neutral-400">
      A clean macOS-style 5-zone layout with simple navigation, a clear code hierarchy, and bracket-based coding lanes.
    </p>
  </div>

  <div class="p-6 border rounded-xl dark:border-neutral-800 bg-neutral-50 dark:bg-neutral-900 shadow-sm hover:shadow-md transition-shadow">
    <div class="text-3xl mb-3 text-primary-500">{{< icon "graduation-cap" >}}</div>
    <h3 class="text-xl font-bold mb-2">Academic Toolset</h3>
    <p class="text-sm text-neutral-600 dark:text-neutral-400">
      Built-in support for Mayring's paraphrasing (generalization & reduction), Bohnsack's Documentary Method, and typology comparisons.
    </p>
  </div>

  <div class="p-6 border rounded-xl dark:border-neutral-800 bg-neutral-50 dark:bg-neutral-900 shadow-sm hover:shadow-md transition-shadow">
    <div class="text-3xl mb-3 text-primary-500">{{< icon "code" >}}</div>
    <h3 class="text-xl font-bold mb-2">Robust Core Backend</h3>
    <p class="text-sm text-neutral-600 dark:text-neutral-400">
      Data storage as a local `.rqda` container (SQLite with WAL, foreign key safety). Full REFI-QDA standard import/export (.qdpx, .qdc) for maximum interoperability.
    </p>
  </div>
</div>

---

## Project Origins: Vibecoding & Practice

> {{< icon "circle-info" >}} **A statement on development:**
> I am a **social worker**, not a computer scientist. This project is being developed as part of my Master's thesis in Social Work. Irritated by the standard requirement to buy expensive software subscriptions for study research, I decided to build rosa_qda myself.
> 
> The entire project is largely **vibecoded** – driven by a clear vision, practical necessity, and powered by modern AI development tools to deliver professional-grade software architecture tailored for a non-technical audience.

---

## Analytical Tools

* **Code Retrieval & Segment Matrix:** Recursive code tree searches filtered by case variables, and automated cross-tabulation.
* **Word Frequencies & KWIC:** Word frequency lists with built-in stopword filtering (German/English) and Keyword-in-Context searches.
* **Whiteboard & Concept Maps:** Visual workspaces to model codes and segments (including code co-occurrence grids).
* **Intercoder Agreement:** Automated calculation of Cohen's Kappa to verify coding consensus.
* **Seamless Audit Trail:** A complete, structured changelog table ensures scientific traceability.

---

## Roadmap & Status

{{< timeline >}}
  {{< timelineItem icon="code" header="Backend & Frontend Prototyping" badge="Completed" >}}
    Development of the full feature set (F-01 to F-73) in the Python/FastAPI backend and the React/TypeScript frontend. 14 integration tests passing successfully.
  {{< /timelineItem >}}
  
  {{< timelineItem icon="globe" header="Integration & Desktop Wrapper" badge="Current" >}}
    Connecting frontend and backend. Packaging the FastAPI application and React frontend into a native desktop shell (e.g., PySide6 QWebEngineView).
  {{< /timelineItem >}}

  {{< timelineItem icon="box-open" header="Local AI Integration & v1.0 Release" badge="Planned" >}}
    Integrating local AI models (Ollama) to assist in transcription and coding tasks. First stable v1.0 release for student research.
  {{< /timelineItem >}}
{{< /timeline >}}
