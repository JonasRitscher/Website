---
title: "Über das Projekt"
description: "Entstehung und Ziele von rosa_qda."
layout: "page"
---
## Die Idee hinter rosa_qda

Proprietäre QDA-Programme (Qualitative Data Analysis) sind für Studierende und freie Forschende oft viel zu teuer. rosa_qda soll ähnlich wie PSPP für SPSS eine os Alternative sein, mit einer ähnlichen GUI wie die populären Programme.

Es gibt bereits einige tolle Open-Source-Projekte im QDA-Bereich:

- **Qualcoder**: Bietet exzellente Analyse- und KI-Funktionen, hat jedoch eine sehr klassische, teils technisch einschüchternde GUI.
- **OpenQDA** und **ReQual**: Bieten teils gute Ansätze, sind in der Einrichtung oder Benutzung jedoch ebenfalls eher technisch orientiert.

Das Problem: In Fachbereichen wie der **Sozialen Arbeit** oder den Sozialwissenschaften stehen viele Studierende Computern vorsichtig ausgedrückt eher distanziert gegenüber. Eine komplizierte oder technisch wirkende Benutzeroberfläche führt dann dazu, dass die Software nicht genutzt wird, weil sie für technisch weniger versierte MEnschen einfach eine zu große Zugangshürde darstellt.

### Das rosa_qda anders machen soll

- **Vertraute Oberfläche:** Orientierung am Aufbau von den populären Programmen und einer Tooleiste wie bei ms office, dadurch soll der Einsteig möglchst schnell gelingen
- **Einfache Installation:** Keine komplexen Datenbankkonfigurationen. Die Software wird als Desktop-App verpackt und nutzt lokale, tragbare Projektdateien (`.rqda` - ein komprimiertes Archiv aus SQLite-Datenbank und Medienordner).
- **Fokus auf das Wesentliche:** Überschaubare, gut strukturierte Werkzeuge statt überladener Menüs.

Mir geht es nicht darum, den vollen Funktionsumfang von kommerziellen Riesen zu kopieren, sondern die **essentiellen Analysefunktionen** bereitzustellen, die für studentische und praxisnahe Forschung benötigt werden, gepaart mit einer einfachen, verständlichen Benutzeroberfläche.

---

### Wer hat sich den Quatsch ausgedacht und wie ist der Code entstanden?

Mein Name ist **Jonas** und ich bin **Sozialarbeiter** und studiere derzeit im Master Soziale Arbeit – ich bin also kein ausgebildeter Informatiker. rosa_qda ist entstanden, weil es mich ärgert, wie teuer die üblichen Tools inzwischen sind und man sie auch nur noch als Abo kaufen kann. An Hochschulen werden dann gerne alte Versionen genutzt die noch ohne Abo auskommen, aber denen dann neue Funktionen fehlen und für Studierende sind die Preise eh zu hoch. Außerdem find ich es falsch, dass closed source Software dann zu großenteilen aus öffentlichen Geldern finanziert wird. Da ich kein Informatiker bin, ist dieses Projekt zu großen Teilen **gevibecodet**.

---

## Technische Highlights (Bereits implementiert)

Das Backend von **rosa_qda** ist bereits vollständig funktionsfähig und deckt wichtige methodologische Werkzeuge ab:

- **Fall- & Variablenmanagement (F-03):** Dynamische Fallzuordnungen und Attribute zur Auswertung nach soziodemografischen Variablen.
- **Mayring-Paraphrasen-Tabellen (F-14):** Eigene Workflows für qualitative Inhaltsanalysen (Generalisierung, erste und zweite Reduktion).
- **Dokumentarische Methode (F-40):** Strukturierte Erfassung von formulierender und reflektierender Interpretation für Sequenzanalysen nach Bohnsack.
- **Visuelle Werkzeuge (F-52):** Ein interaktives Whiteboard zur Konzeptarbeit, dessen Layouts direkt in den hierarchischen Codebaum überführt werden können.
- **Wortanalysen (F-51):** Wortfrequenztabellen mit Stoppwort-Filtern und Keyword-in-Context-Suchen (KWIC).
- **Intercoder-Agreement (F-60):** Automatische Berechnung des Cohen's Kappa Koeffizienten bei kollaborativer Codierung.
- **REFI-QDA Standard (F-61):** Uneingeschränkter Im- und Export von standardisierten XML-Projektdateien (`.qdpx` und `.qdc`) zur Interoperabilität mit MAXQDA und Atlas.ti.
- **Audit-Trail & Änderungslog (F-62):** Automatisches Logging aller Modifikationen zur Absicherung wissenschaftlicher Gütekriterien.
