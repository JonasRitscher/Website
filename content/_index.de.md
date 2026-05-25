---
title: "rosa_qda — Freie QDA-Software"
description: "Die benutzerfreundliche Open-Source-Alternative zu MAXQDA & Co. für die qualitative Sozialforschung."
layout: "page"
---
{{< lead >}}
Eine **freie, benutzerfreundliche Open-Source-Alternative** zu proprietärer Software wie MAXQDA und Atlas.ti – speziell entwickelt für Studierende und Forschende in den Sozialwissenschaften.
{{< /lead >}}

<div class="flex flex-wrap gap-4 my-8 justify-center">
  {{< button href="https://github.com/JonasRitscher/rosa_qda" target="_blank" icon="github" >}}
    Zum GitHub Repository
  {{< /button >}}
  {{< button href="about/" outline=true >}}
    Mehr über das Projekt
  {{< /button >}}
</div>

---

## Kernmerkmale & Features

<div class="grid grid-cols-1 md:grid-cols-3 gap-6 my-8">
  <div class="p-6 border rounded-xl dark:border-neutral-800 bg-neutral-50 dark:bg-neutral-900 shadow-sm hover:shadow-md transition-shadow">
    <div class="text-3xl mb-3 text-primary-500">{{< icon "wand-magic-sparkles" >}}</div>
    <h3 class="text-xl font-bold mb-2">Moderne GUI (React)</h3>
    <p class="text-sm text-neutral-600 dark:text-neutral-400">
      Ein übersichtliches 5-Zonen-Layout im macOS-Stil mit einfacher Navigation, übersichtlicher Code-Hierarchie und bracket-basierten Codier-Lanes.
    </p>
  </div>

<div class="p-6 border rounded-xl dark:border-neutral-800 bg-neutral-50 dark:bg-neutral-900 shadow-sm hover:shadow-md transition-shadow">
    <div class="text-3xl mb-3 text-primary-500">{{< icon "graduation-cap" >}}</div>
    <h3 class="text-xl font-bold mb-2">Fürs Studium optimiert</h3>
    <p class="text-sm text-neutral-600 dark:text-neutral-400">
      Fokus auf Auswertung nach Mayrin, Kuckartz, Bohnsack und Grounded Theory.
    </p>
  </div>

`<div class="p-6 border rounded-xl dark:border-neutral-800 bg-neutral-50 dark:bg-neutral-900 shadow-sm hover:shadow-md transition-shadow">`
    `<div class="text-3xl mb-3 text-primary-500">`{{< icon "code" >}}`</div>`
    `<h3 class="text-xl font-bold mb-2">`Robustes Core-Backend `</h3>`
    `<p class="text-sm text-neutral-600 dark:text-neutral-400">`
      Datenhaltung als lokaler `.rqda`-Container (SQLite mit WAL, Fremdschlüssel-Sicherheit). REFI-QDA Standard-Im- und Export (.qdpx, .qdc) zur maximalen Interoperabilität.
    `</p>`

---

## Analytische Werkzeuge

* **Code-Retrieval & Segmentmatrix:** Rekursive Suche im Codebaum gefiltert nach Fallvariablen und vollautomatische Kreuztabellen-Generierung.
* **Wortfrequenzen & KWIC:** Vollständige Häufigkeitslisten mit deutscher und englischer Stoppwortliste sowie Keyword-in-Context-Suchen.
* **Whiteboard & Concept-Maps:** Visuelle Arbeitsbereiche zur relationalen Zuordnung von Codes und Segmenten (inkl. Code-Kookkurrenzen).
* **Intercoder-Agreement:** Automatische Berechnung von Cohen's Kappa zur Verifizierung von Übereinstimmungen.
* **Lückenloser Audit-Trail:** Ein vollständiges, strukturiertes Änderungslog sichert die wissenschaftliche Nachvollziehbarkeit.

---

## Roadmap & Status

{{< timeline >}}
  {{< timelineItem icon="code" header="Backend & Frontend Prototyping" badge="Abgeschlossen" >}}
    Entwicklung des vollen Feature-Sets (F-01 bis F-73) im Python/FastAPI Backend und des React/TypeScript Frontends. Erfolgreiches Bestehen aller 14 Integrationstests.
  {{< /timelineItem >}}

  {{< timelineItem icon="globe" header="Integration & Desktop-Wrapper" badge="Aktuell" >}}
    Verknüpfung von Frontend und Backend. Verpackung der Python/FastAPI-Anwendung und des React-Frontends in eine native Desktop-Shell (z. B. PySide6 QWebEngineView).
  {{< /timelineItem >}}

  {{< timelineItem icon="box-open" header="Lokale KI-Integration & v1.0 Release" badge="Geplant" >}}
    Einbindung lokaler KI-Modelle (Ollama) zur Unterstützung bei der Transkription und Kodierung. Erstes stabiles v1.0 Release.
  {{< /timelineItem >}}
{{< /timeline >}}
