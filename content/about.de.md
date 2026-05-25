---
title: "Über das Projekt"
description: "Erfahre mehr über die Vision, Entstehung und Ziele von rosa_qda."
layout: "page"
---

## Die Vision hinter rosa_qda

Die qualitative Sozialforschung ist ein zentraler Bestandteil sozial- und geisteswissenschaftlicher Studiengänge sowie der Praxisforschung. Doch wer heutzutage Daten qualitativ auswerten möchte (z. B. nach der Qualitativen Inhaltsanalyse nach Mayring, der Grounded Theory oder der Dokumentarischen Methode), stößt schnell auf finanzielle Barrieren: Die marktführenden Programme wie **MAXQDA** oder **Atlas.ti** sind proprietär und für Studierende und kleinere Träger mit erheblichen Lizenzkosten verbunden.

**rosa_qda** schließt diese Lücke. Ähnlich wie **PSPP** eine freie, leicht zugängliche Alternative zu SPSS im quantitativen Bereich darstellt, bietet rosa_qda Studierenden und Forschenden eine kostenfreie Desktop-Software.

Dabei geht es nicht darum, den vollen Funktionsumfang von kommerziellen Riesen zu kopieren, sondern die **essentiellen Analysefunktionen** bereitzustellen, die für studentische und praxisnahe Forschung benötigt werden, gepaart mit einer herausragenden, verständlichen Benutzererfahrung.

---

## Warum eine neue Software?

Es gibt bereits einige bemerkenswerte Open-Source-Projekte im QDA-Bereich:
- **Qualcoder**: Bietet exzellente Analyse- und KI-Funktionen, hat jedoch eine sehr klassische, teils technisch einschüchternde GUI.
- **OpenQDA** und **ReQual**: Bieten teils gute Ansätze, sind in der Einrichtung oder Benutzung jedoch ebenfalls eher technisch orientiert.

Das Problem: In Fachbereichen wie der **Sozialen Arbeit** oder den Sozialwissenschaften stehen viele Forschende und Studierende Computern eher distanziert gegenüber. Eine komplizierte oder technisch wirkende Benutzeroberfläche führt dazu, dass die Software nicht genutzt wird.

### Unser Lösungsansatz
* **Vertraute Oberfläche:** Ein durchdachtes 5-Zonen-Layout (macOS-Style MenuBar, ModuleTabs, ActionBar, DocArea mit Coding-Lanes, RightPanel mit Memos), das sich an bekannten Strukturen orientiert, um den Umstieg so einfach wie möglich zu machen.
* **Einfache Installation:** Keine komplexen Datenbankkonfigurationen. Die Software wird als Desktop-App verpackt und nutzt lokale, tragbare Projektdateien (`.rqda` - ein komprimiertes Archiv aus SQLite-Datenbank und Medienordner).
* **Fokus auf das Wesentliche:** Überschaubare, gut strukturierte Werkzeuge statt überladener Menüs.

---

## Wer steht hinter dem Projekt? (Vibecoding & Social Work)

Mein Name ist **Jonas Ritscher**. Ich bin **Sozialarbeiter** und studiere derzeit im Master Soziale Arbeit – ich bin also kein ausgebildeter Informatiker. Da es mich geärgert hat, dass im Studium standardmäßig auf proprietäre, teure Software gesetzt werden muss, habe ich beschlossen, rosa_qda selbst zu entwickeln.

Da ich keine formelle IT-Ausbildung besitze, ist dieses Projekt zu großen Teilen **gevibecodet**. Mithilfe moderner KI-Assistenten habe ich eine anspruchsvolle Software-Architektur aufgebaut, die sich vor professionellen Entwicklungen nicht verstecken muss:
* **Frontend:** React 18, TypeScript und Vite 6 mit einem pixelgenauen macOS-Sonoma-Design.
* **Backend:** Python 3.13 und FastAPI mit SQLite (WAL-Modus) für schnelle, transaktionssichere Datenoperationen.
* **Qualitätskontrolle:** Eine umfassende Testsuite mit 14 Integrationstests deckt alle komplexen Datenflüsse und statistischen Berechnungen ab.

Dieses Zusammenspiel zeigt, dass durch "Vibecoding" fachwissenschaftlicher Praxisbezug (was brauchen Sozialarbeitende wirklich?) und moderne Technologie barrierefrei verschmelzen können.

---

## Technische Highlights (Bereits implementiert)

Das Backend von **rosa_qda** ist bereits vollständig funktionsfähig und deckt wichtige methodologische Werkzeuge ab:

* **Fall- & Variablenmanagement (F-03):** Dynamische Fallzuordnungen und Attribute zur Auswertung nach soziodemografischen Variablen.
* **Mayring-Paraphrasen-Tabellen (F-14):** Eigene Workflows für qualitative Inhaltsanalysen (Generalisierung, erste und zweite Reduktion).
* **Dokumentarische Methode (F-40):** Strukturierte Erfassung von formulierender und reflektierender Interpretation für Sequenzanalysen nach Bohnsack.
* **Visuelle Werkzeuge (F-52):** Ein interaktives Whiteboard zur Konzeptarbeit, dessen Layouts direkt in den hierarchischen Codebaum überführt werden können.
* **Wortanalysen (F-51):** Wortfrequenztabellen mit Stoppwort-Filtern und Keyword-in-Context-Suchen (KWIC).
* **Intercoder-Agreement (F-60):** Automatische Berechnung des Cohen's Kappa Koeffizienten bei kollaborativer Codierung.
* **REFI-QDA Standard (F-61):** Uneingeschränkter Im- und Export von standardisierten XML-Projektdateien (`.qdpx` und `.qdc`) zur Interoperabilität mit MAXQDA und Atlas.ti.
* **Audit-Trail & Änderungslog (F-62):** Automatisches Logging aller Modifikationen zur Absicherung wissenschaftlicher Gütekriterien.
