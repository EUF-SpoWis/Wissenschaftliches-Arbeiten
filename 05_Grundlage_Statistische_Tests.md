<<<<<<< HEAD
<!--
author: Swantje Brandt
email: swantje.brandt@uni-flensburg.de
version: 0.0.1
language: de
narrator: Deutsch Female

import:  https://raw.githubusercontent.com/EUF-SpoWis/M1_Einfuehrung_Sportwissenschaft/refs/heads/main/config.md

link:   https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css
        https://cdn.jsdelivr.net/gh/EUF-SpoWis/Wissenschaftliches-Arbeiten@main/Lia-Anpassungen/Ausblendungen.css

-->

## Statistische Tests



[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/EUF-SpoWis/Wissenschaftliches-Arbeiten/main/05_Grundlage_Statistische_Tests.md)

| Parameter                | Kursinformationen |
| ------------------------ | ----------------- |
| **Veranstaltung:**       | Wissenschaftliches Arbeiten |
| **Semester:**            | |
| **Hochschule:**          | `Europa-Universität Flensburg` |
| **Inhalte:**             | `Statistische Tests mit JASP: Zusammenhänge zwischen Variablen` |
| **Link auf GitHub:**     | https://github.com/EUF-SpoWis/Wissenschaftliches-Arbeiten/blob/main/05_Grundlage_Statistische_Tests.md |
| **Autoren:**             | Tim Heemsoth & Swantje Brandt |

> (c) Alle Rechte vorbehalten.

 
---
 
## Überblick
 
<div style="border-left: 6px solid #2e9e5b; background: rgba(46,158,91,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
💡 <b>Lehrbuch Hinweis:</b> In diesem Kurs lernst du, wie du Daten mit <b>Kennwerten und Grafiken beschreibst</b>, wie du diese Kennwerte <b>in JASP berechnest</b> und <b>welcher statistische Test</b> zu welcher Fragestellung passt. Als Beispiel dient wie im Grundlagenkurs der 12-Minuten-Lauf mit und ohne Musik.
</div>
<div style="height: 15px;"></div>
<div style="display: flex; flex-direction: column; gap: 8px; margin: 12px 0;">
<div style="display: flex; gap: 12px; align-items: flex-start; background: #eef2fb; border-left: 6px solid #4e66bd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">📊</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Deskriptive Statistik</b></div>
<div style="font-size: 0.9em;">Du beschreibst die Daten mit Kennwerten und Grafiken und berechnest sie in JASP.</div>
</div>
</div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #eaf6ee; border-left: 6px solid #2a9a50; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">📋</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Reliabilität und Skalenmittelwerte</b></div>
<div style="font-size: 0.9em;">Du prüfst, ob die Items eines Fragebogens dasselbe messen, und fasst sie zu einem Wert zusammen.</div>
</div>
</div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #f6f1fa; border-left: 6px solid #a74ebd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">🧭</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Übersicht über statistische Tests</b></div>
<div style="font-size: 0.9em;">Du erfährst, welcher statistische Test für welche Fragestellung geeignet ist.</div>
</div>
</div>
</div>
 
---
## Das Beispiel: Musik und Ausdauerleistung
 
<div style="display: flex; flex-direction: column; gap: 8px; margin: 12px 0;">
<div style="display: flex; gap: 12px; align-items: flex-start; background: #eef2fb; border-left: 6px solid #4e66bd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">🎯</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Fragestellung</b></div>
<div style="font-size: 0.9em;">Laufen Sportstudierende <b>mit Musik</b> weiter als <b>ohne Musik</b>?</div>
</div>
</div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #eef2fb; border-left: 6px solid #4e66bd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">👥</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Studiendesign</b></div>
<div style="font-size: 0.9em;">20 Sportstudierende werden zufällig zwei Gruppen zugeteilt. Gruppe 1 läuft <b>ohne Musik</b>, Gruppe 2 <b>mit Musik</b>. Alle absolvieren einen <b>Cooper-Test</b> (12 Minuten Laufen).</div>
</div>
</div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #eef2fb; border-left: 6px solid #4e66bd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">📏</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Variablen</b></div>
<div style="font-size: 0.9em;"><b>UV:</b> Musik (ohne Musik / mit Musik), nominalskaliert<br><b>AV:</b> Ausdauerleistung = gelaufene Strecke in Metern, verhältnisskaliert</div>
</div>
</div>
</div>
<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
🏃🏾‍♀️ <b>Strecke (m)</b> 🏃🏾‍♀️<br>
Ausdauerleistung, <b>metrisch</b>. Sie ist in diesem Kurs die abhängige Variable.
</div>
<details>
<summary><b>👉 Rohdaten</b></summary>
Die gelaufene Strecke in Metern im Cooper-Test:
 
<!-- data-type="none" -->
| Person | Gruppe | Strecke (m) |
| :-: | :-- | :-: |
| 1 | ohne Musik | 2350 |
| 2 | ohne Musik | 2480 |
| 3 | ohne Musik | 2410 |
| 4 | ohne Musik | 2600 |
| 5 | ohne Musik | 2290 |
| 6 | ohne Musik | 2520 |
| 7 | ohne Musik | 2450 |
| 8 | ohne Musik | 2380 |
| 9 | ohne Musik | 2550 |
| 10 | ohne Musik | 2470 |
| 11 | mit Musik | 2500 |
| 12 | mit Musik | 2620 |
| 13 | mit Musik | 2480 |
| 14 | mit Musik | 2710 |
| 15 | mit Musik | 2440 |
| 16 | mit Musik | 2590 |
| 17 | mit Musik | 2650 |
| 18 | mit Musik | 2530 |
| 19 | mit Musik | 2760 |
| 20 | mit Musik | 2560 |
 
</details>
<div style="border-left: 6px solid #e08a1e; background: rgba(224,138,30,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
⚠️ <b>Problem:</b> Aus 20 einzelnen Zahlen lässt sich kaum ablesen, ob Musik einen Unterschied macht. Wir brauchen Kennwerte, die die Daten <b>zusammenfassen</b>.
</div>
 
---
## Deskriptive vs. inferenzielle Statistik
 
<div style="display: flex; flex-direction: column; gap: 8px; margin: 12px 0;">
<div style="display: flex; gap: 12px; align-items: flex-start; background: #eef2fb; border-left: 6px solid #4e66bd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">📊</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Deskriptive Statistik (beschreibend)</b></div>
<div style="font-size: 0.9em;">Fasst die Daten der <b>Stichprobe</b> zusammen, mit Kennwerten (z. B. Mittelwert) und Grafiken (z. B. Boxplot).</div>
<div style="margin-top: 6px; padding: 5px 10px; background: #ffffff; border-radius: 6px; font-size: 0.85em;">🏃🏾‍♀️ <i>„Die Gruppe mit Musik lief im Mittel 2584 m, die Gruppe ohne Musik 2450 m.“</i></div>
</div>
</div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #f6f1fa; border-left: 6px solid #a74ebd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">🔬</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Inferenzielle Statistik (schließend)</b></div>
<div style="font-size: 0.9em;">Überprüft, ob sich Ergebnisse auf die <b>Population</b> übertragen lassen, mit statistischen Tests (z. B. t-Test), p-Werten und Effektstärken.</div>
<div style="margin-top: 6px; padding: 5px 10px; background: #ffffff; border-radius: 6px; font-size: 0.85em;">🏃🏾‍♀️ <i>„Ist der Unterschied von 134 m groß genug, um nicht nur zufällig zu sein?“</i></div>
</div>
</div>
</div>
<div style="border-left: 6px solid #e0a526; background: rgba(224,165,38,0.14); border-radius: 8px; padding: 0.7rem 1.2rem;">
📌 <b>Merke:</b> Die deskriptive Statistik ist immer der erste Schritt. Bevor getestet wird, müssen die Daten beschrieben werden.
</div>
 
---
## Deskriptive Statistik in JASP
 
[JASP](https://jasp-stats.org/) ist eine kostenlose Open-Source-Statistiksoftware. Sie ist für Windows, macOS und Linux verfügbar.
 
<span style="font-size: 1.1em;"><b>Die Daten</b></span>
 
<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
📋 <b>Datenformat</b> 📋<br>
Jede Zeile ist eine Person, jede Spalte eine Variable. Speichere die Daten als CSV-Datei (z. B. <code>ausdauer_musik.csv</code>). Die Spalten M1 bis M4 enthalten die Antworten auf den Motivationsfragebogen (siehe Zusatzbeispiel), M3 ist noch <b>nicht</b> umgepolt.
</div>
<details>
<summary><b>👉 CSV-Datei</b></summary>
``` text
Person,Gruppe,Strecke,M1,M2,M3,M4
1,ohne Musik,2350,1,2,4,2
2,ohne Musik,2480,4,3,2,3
3,ohne Musik,2410,4,2,2,3
4,ohne Musik,2600,5,5,3,4
5,ohne Musik,2290,4,4,2,4
6,ohne Musik,2520,3,3,3,3
7,ohne Musik,2450,4,3,2,4
8,ohne Musik,2380,3,2,4,3
9,ohne Musik,2550,2,1,4,3
10,ohne Musik,2470,2,2,3,2
11,mit Musik,2500,5,3,3,4
12,mit Musik,2620,2,3,3,2
13,mit Musik,2480,3,3,3,3
14,mit Musik,2710,5,5,1,4
15,mit Musik,2440,4,4,2,3
16,mit Musik,2590,4,4,3,5
17,mit Musik,2650,5,4,3,5
18,mit Musik,2530,4,4,3,5
19,mit Musik,2760,3,4,4,3
20,mit Musik,2560,4,3,2,3
```
 
</details>
<span style="font-size: 1.1em;"><b>Durchführung in JASP</b></span>
 
<div style="display: flex; flex-direction: column; gap: 8px; margin: 12px 0;">
<div style="display: flex; gap: 12px; align-items: flex-start; background: #f6f1fa; border-left: 6px solid #a74ebd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">🏷️</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>1. Variablen einstellen</b></div>
<div style="font-size: 0.9em;">Gruppe als nominal, Strecke als scale.</div>
</div>
</div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #f6f1fa; border-left: 6px solid #a74ebd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">🧪</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>2. Analyse öffnen</b></div>
<div style="font-size: 0.9em;">Descriptives ➜ Descriptive Statistics.</div>
</div>
</div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #f6f1fa; border-left: 6px solid #a74ebd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">🔗</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>3. Variablen zuweisen</b></div>
<div style="font-size: 0.9em;">Strecke in „Variables“, Gruppe in „Split“.</div>
</div>
</div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #f6f1fa; border-left: 6px solid #a74ebd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">📈</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>4. Kennwerte und Grafiken</b></div>
<div style="font-size: 0.9em;">Unter „Statistics“ Lage- und Streuungsmaße anhaken, unter „Plots“ Histogramme und Boxplots.</div>
</div>
</div>
</div>

<div style="height: 10px;"></div>
!?[Allgemeine Einführung in JASP](https://youtu.be/2lGMEnK6f2A)

 
<span style="font-size: 1.1em;"><b>Ergebnis lesen</b></span>
 
<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Descriptive Statistics</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;"></th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Strecke (ohne Musik)</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Strecke (mit Musik)</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Valid</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">10</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">10</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Median</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2460,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2575,00</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Mean</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2450,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2584,00</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Std. Deviation</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">94,75</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">102,55</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Variance</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">8977,78</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">10515,56</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Range</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">310,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">320,00</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Minimum</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2290,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2440,00</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Maximum</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2600,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2760,00</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">25th percentile</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2387,50</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2507,50</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">50th percentile</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2460,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2575,00</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">75th percentile</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2510,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2642,50</td></tr>
</table>
</div>
<div style="font-size: 0.8em; opacity: 0.7; margin-bottom: 10px;">Fiktive Daten, nachgebaut im Stil der JASP-Ausgabe.</div>
<ul style="font-size: 0.95em;">
<li><b>Mittelwert:</b> Die Gruppe <b>mit Musik</b> lief im Mittel <b>134 m weiter</b> (<i>M</i> = 2584 m) als die Gruppe <b>ohne Musik</b> (<i>M</i> = 2450 m).</li>
<li><b>Median:</b> Mittelwert und Median liegen in beiden Gruppen nah beieinander ➜ kein Hinweis auf eine stark schiefe Verteilung.</li>
<li><b>Streuung:</b> Die Standardabweichungen sind in beiden Gruppen ähnlich (<i>SD</i> = 94,75 m vs. <i>SD</i> = 102,55 m).</li>
</ul>
<div style="border-left: 6px solid #e08a1e; background: rgba(224,138,30,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
⚠️ <b>Aber:</b> Ob dieser Unterschied von 134 m nur zufällig zustande gekommen ist, kann die deskriptive Statistik <b>nicht</b> beantworten. Dafür brauchen wir einen <b>statistischen Test</b>.
</div>
<span style="font-size: 1.1em;"><b>So berichtest du das Ergebnis</b></span>
 
<div style="border-left: 6px solid #a74ebd; background: #f6f1fa; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
✍️ <b>Musterbericht (APA):</b><br>
<i>Die Teilnehmenden, die mit Musik liefen, legten im Cooper-Test im Mittel eine größere Strecke zurück (M = 2584 m, SD = 102,55) als die Teilnehmenden ohne Musik (M = 2450 m, SD = 94,75).</i>
</div>
<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Döring & Bortz (2016); JASP Team (2024)
</div>
 
---
## Zusatzbeispiel: Fragebogen, Reliabilität und Skalenmittelwerte
 
<div style="border: 2px solid #2a9a50; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
📋 <b>Zusätzlich erhobener Fragebogen</b> 📋<br>
Nach dem Cooper-Test füllen alle 20 Personen einen kurzen Fragebogen zur <b>Laufmotivation</b> aus. Die vier Items werden auf einer Likert-Skala von 1 (<i>trifft gar nicht zu</i>) bis 5 (<i>trifft voll zu</i>) beantwortet.
</div>
| Item | Aussage |
| :-: | :-- |
| M1 | Ich hatte Lust, weiterzulaufen. |
| M2 | Das Laufen hat mir Spaß gemacht. |
| M3 | Ich wollte möglichst schnell aufhören. *(invertiert)* |
| M4 | Ich habe mich beim Laufen angestrengt, weil ich es wollte. |
 
<div style="display: flex; flex-direction: column; gap: 8px; margin: 12px 0;">
<div style="display: flex; gap: 12px; align-items: flex-start; background: #eaf6ee; border-left: 6px solid #2a9a50; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">🔗</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Reliabilität: Messen die Items dasselbe?</b></div>
<div style="font-size: 0.9em;">Bevor die Items zu einem Wert zusammengefasst werden, wird die <b>interne Konsistenz</b> geprüft. <b>Cronbachs Alpha</b> (α) liegt zwischen 0 und 1: ab <b>,70 akzeptabel</b>, ab <b>,80 gut</b>, ab <b>,90 sehr gut</b>. Die Werte <i>„if item dropped“</i> zeigen, ob ein einzelnes Item die Reliabilität verschlechtert.</div>
</div>
</div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #fdf3e7; border-left: 6px solid #e08a1e; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">🔄</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Achtung: invertierte Items!</b></div>
<div style="font-size: 0.9em;">Item M3 ist negativ formuliert. Es muss <b>vor</b> der Reliabilitätsanalyse umgepolt werden (1 ➜ 5, 2 ➜ 4, …), sonst sinkt die Reliabilität deutlich.</div>
<div style="margin-top: 6px; padding: 5px 10px; background: #ffffff; border-radius: 6px; font-size: 0.85em;">Formel: M3<sub>neu</sub> = 6 − M3</div>
</div>
</div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #f6f1fa; border-left: 6px solid #a74ebd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">➗</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Skalenmittelwert bilden</b></div>
<div style="font-size: 0.9em;">Ist die Reliabilität ausreichend, wird pro Person der Mittelwert über alle Items berechnet: Motivation = (M1 + M2 + M3<sub>neu</sub> + M4) / 4. Der Skalenmittelwert kann anschließend wie die Strecke deskriptiv beschrieben werden.</div>
<div style="margin-top: 6px; padding: 5px 10px; background: #ffffff; border-radius: 6px; font-size: 0.85em;">Beispiel: M1 = 4, M2 = 5, M3 = 2 (umgepolt: 4), M4 = 3 ➜ Motivation = (4 + 5 + 4 + 3) / 4 = 4</div>
</div>
</div>
</div>
<span style="font-size: 1.1em;"><b>Durchführung in JASP</b></span>
 
<div style="display: flex; flex-direction: column; gap: 8px; margin: 12px 0;">
<div style="display: flex; gap: 12px; align-items: flex-start; background: #f6f1fa; border-left: 6px solid #a74ebd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">🔄</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>1. Item umpolen</b></div>
<div style="font-size: 0.9em;">Neue berechnete Spalte für M3<sub>neu</sub> = 6 − M3 anlegen (oder M3 in der Analyse als „reverse-scaled item“ angeben).</div>
</div>
</div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #f6f1fa; border-left: 6px solid #a74ebd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">🧪</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>2. Reliabilität berechnen</b></div>
<div style="font-size: 0.9em;">Reliability ➜ Unidimensional Reliability, M1, M2, M3<sub>neu</sub> und M4 zuweisen, Cronbach’s α und „If item dropped“ anhaken.</div>
</div>
</div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #f6f1fa; border-left: 6px solid #a74ebd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">➗</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>3. Skalenmittelwert bilden</b></div>
<div style="font-size: 0.9em;">Über „Compute column“ eine neue Spalte mit dem Mittelwert der vier Items anlegen.</div>
</div>
</div>
</div>
!?[Allgemeine Einführung in JASP](https://youtu.be/golKIhL8eDk)

!?[Allgemeine Einführung in JASP](https://youtu.be/Xa5Hdfb9NBc)

<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Döring & Bortz (2016); JASP Team (2024)
</div>
 
---
## Übersicht: Welcher statistische Test?
 
<div style="border-left: 6px solid #2e9e5b; background: rgba(46,158,91,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
💡 <b>Lehrbuch Hinweis:</b> Die Wahl des Tests hängt von drei Fragen ab: der <b>Fragestellung</b>, dem <b>Studiendesign</b> und den <b>Eigenschaften der abhängigen Variable</b>.
</div>
<div style="display: flex; flex-direction: column; gap: 8px; margin: 12px 0;">
<div style="display: flex; gap: 12px; align-items: flex-start; background: #eef2fb; border-left: 6px solid #4e66bd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">🎯</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>1. Was ist die Fragestellung?</b></div>
<div style="font-size: 0.9em;"><b>Unterschied:</b> Unterscheiden sich Gruppen oder Messzeitpunkte?<br><b>Zusammenhang:</b> Hängen zwei Variablen zusammen?</div>
<div style="margin-top: 6px; padding: 5px 10px; background: #ffffff; border-radius: 6px; font-size: 0.85em;">🏃🏾‍♀️ Laufen Personen mit Musik weiter als ohne? / Hängt das Musiktempo mit der Strecke zusammen?</div>
</div>
</div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #eaf6ee; border-left: 6px solid #2a9a50; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">👥</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>2. Wie sind die Daten erhoben worden?</b></div>
<div style="font-size: 0.9em;"><b>Unabhängige Stichproben:</b> verschiedene Personen in den Gruppen<br><b>Abhängige Stichproben:</b> dieselben Personen werden mehrfach gemessen<br><b>Anzahl:</b> zwei oder mehr als zwei Gruppen bzw. Messzeitpunkte?</div>
<div style="margin-top: 6px; padding: 5px 10px; background: #ffffff; border-radius: 6px; font-size: 0.85em;">🏃🏾‍♀️ Gruppe A ohne, Gruppe B mit Musik / alle laufen einmal ohne und einmal mit Musik</div>
</div>
</div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #f6f1fa; border-left: 6px solid #a74ebd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">📏</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>3. Welches Skalenniveau und welche Verteilung hat die AV?</b></div>
<div style="font-size: 0.9em;"><b>Metrisch und annähernd normalverteilt</b> ➜ parametrische Tests<br><b>Ordinal oder nicht normalverteilt</b> (bei kleinen Stichproben) ➜ nichtparametrische Tests</div>
</div>
</div>
</div>
<span style="font-size: 1.1em;"><b>Entscheidungsbaum</b></span>
 
``` ascii
                          Fragestellung?
                                |
             +------------------+------------------+
             |                                     |
        Unterschied                           Zusammenhang
             |                                     |
     Wie viele Gruppen /               +-----------+-----------+
     Messzeitpunkte?                   |                       |
             |                  metrisch, normal-       ordinal / nicht
     +-------+-------+          verteilt                normalverteilt
     |               |                 |                       |
   zwei        mehr als zwei      Pearson-r              Spearman-rho
     |               |
 unabhängig?     unabhängig?
  |       |       |       |
 ja      nein    ja      nein
  |       |       |       |
 t-Test  t-Test  ANOVA   ANOVA mit
 (unab-  (ab-    (ein-   Messwieder-
 hängig) hängig) fakt.)  holung
```
 
*Nichtparametrische Alternativen findest du in den folgenden Tabellen.*
 
---
### Nicht-parametrische Tests

<div style="display: flex; gap: 12px; align-items: flex-start; background: #eef2fb; border-left: 6px solid #4e66bd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">🔢</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Was sind nichtparametrische Tests?</b></div>
<div style="font-size: 0.9em;">Sie setzen <b>keine Normalverteilung</b> voraus. Statt mit den Messwerten selbst rechnen sie mit deren **Rangplätzen**</div>
<div style="margin-top: 6px; padding: 5px 10px; background: #ffffff; border-radius: 6px; font-size: 0.85em;">🏃🏾‍♀️ Die größte Strecke (2760 m) erhält Rang 20, die kleinste (2290 m) Rang 1.</div>
</div> 
</div>
<div style="height: 10px;"></div>

<div style="display: flex; gap: 12px; align-items: flex-start; background: #eef2fb; border-left: 6px solid #4e66bd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">🎯</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Wann werden sie eingesetzt?</b></div>
<div style="font-size: 0.9em;">Bei <b>ordinalskalierten</b> Daten (z. B. Rangplätze, einzelne Likert-Items), wenn metrische Daten <b>nicht normalverteilt</b> sind (vor allem bei kleinen Stichproben) und bei deutlichen <b>Ausreißern</b></div>
</div> 
</div>
<div style="height: 10px;"></div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #eef2fb; border-left: 6px solid #4e66bd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">⚖️</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Vor- und Nachteile</b></div>
<div style="font-size: 0.9em;"><b>+</b> robust gegenüber Ausreißern und schiefen Verteilungen<br><b>−</b> geringere Teststärke: Sind die Voraussetzungen für einen parametrischen Test erfüllt, findet dieser einen tatsächlichen Effekt eher.</div>
</div> 
</div>


---
 
### Normalverteilung prüfen
 
<div style="display: flex; flex-direction: column; gap: 8px; margin: 12px 0;">
<div style="display: flex; gap: 12px; align-items: flex-start; background: #eef2fb; border-left: 6px solid #4e66bd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">📊</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Grafisch</b></div>
<div style="font-size: 0.9em;"><b>Histogramm:</b> Ist die Verteilung annähernd glockenförmig und symmetrisch?<br><b>Q-Q-Plot:</b> Liegen die Punkte nah an der Diagonalen? Systematische Abweichungen (z. B. Bögen oder Ausreißer an den Enden) sprechen gegen eine Normalverteilung.</div>
</div>
</div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #f6f1fa; border-left: 6px solid #a74ebd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">🧪</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Statistisch: Shapiro-Wilk-Test</b></div>
<div style="font-size: 0.9em;"><b>H0:</b> Die Daten sind normalverteilt.<br><i>p</i> ≤ ,05 ➜ signifikante Abweichung ➜ nichtparametrischen Test erwägen<br><i>p</i> ≥ ,05 ➜ keine signifikante Abweichung ➜ parametrischer Test möglich</div>
<div style="margin-top: 6px; padding: 5px 10px; background: #ffffff; border-radius: 6px; font-size: 0.85em;">🏃🏾‍♀️ Ohne Musik <i>W</i> = 0,99, <i>p</i> = ,998; mit Musik <i>W</i> = 0,97, <i>p</i> = ,928 ➜ in beiden Gruppen keine Abweichung von der Normalverteilung.</div>
</div>
</div>
</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> Descriptives ➜ Descriptive Statistics ➜ Statistics: Shapiro-Wilk test, Plots: Q-Q plots<br>Alternativ im t-Test bzw. in der ANOVA unter „Assumption Checks“ ➜ Normality</div>
<div style="height: 10px;"></div>
<div style="border-left: 6px solid #e0a526; background: rgba(224,165,38,0.14); border-radius: 8px; padding: 0.7rem 1.2rem;">
📌 <b>Merke:</b> Die Normalverteilung wird <b>getrennt für jede Gruppe</b> geprüft (bei abhängigen Stichproben für die Differenzen). Bei <b>kleinen</b> Stichproben erkennt der Shapiro-Wilk-Test Abweichungen kaum, bei <b>großen</b> wird er schon bei kleinen Abweichungen signifikant. Betrachte deshalb immer zusätzlich die Grafiken. Ab etwa 30 Personen pro Gruppe sind t-Test und ANOVA relativ robust.
</div>


** VIDEO JASP EINFÜGEN**
 
---
### Unterschiedshypothesen
 
<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 12px; padding: 10px; color: #1f2933;">
<table style="width: 100%; border-collapse: collapse; font-size: 0.9em;">
<tr><th style="text-align: left; padding: 8px;">Situation</th><th style="padding: 8px; background: #2f6f57; color: #ffffff;">Parametrisch</th><th style="padding: 8px; background: #e08a1e; color: #ffffff;">Nichtparametrisch</th><th style="text-align: left; padding: 8px;">Beispiel</th></tr>
<tr style="border-bottom: 1px solid #cbd5e1;"><td style="padding: 8px;"><b>Unabhängig</b><br><span style="font-size: 0.85em;">2 Gruppen</span></td><td style="padding: 8px; background: #e3efe9;">t-Test für unabhängige Stichproben</td><td style="padding: 8px; background: #fdf3e7;">Mann-Whitney-U-Test</td><td style="padding: 8px; font-size: 0.9em;">Gruppe ohne Musik vs. Gruppe mit Musik</td></tr>
<tr style="border-bottom: 1px solid #cbd5e1;"><td style="padding: 8px;"><b>Abhängig</b><br><span style="font-size: 0.85em;">2 Messungen</span></td><td style="padding: 8px; background: #e3efe9;">t-Test für verbundene Stichproben</td><td style="padding: 8px; background: #fdf3e7;">Wilcoxon-Test</td><td style="padding: 8px; font-size: 0.9em;">Dieselben Personen laufen einmal ohne und einmal mit Musik</td></tr>
<tr style="border-bottom: 1px solid #cbd5e1;"><td style="padding: 8px;"><b>Unabhängig</b><br><span style="font-size: 0.85em;">mehr als 2 Gruppen</span></td><td style="padding: 8px; background: #e3efe9;">einfaktorielle ANOVA</td><td style="padding: 8px; background: #fdf3e7;">Kruskal-Wallis-Test</td><td style="padding: 8px; font-size: 0.9em;">Ohne Musik vs. langsame Musik vs. schnelle Musik</td></tr>
<tr style="border-bottom: 1px solid #cbd5e1;"><td style="padding: 8px;"><b>Abhängig</b><br><span style="font-size: 0.85em;">mehr als 2 Messungen</span></td><td style="padding: 8px; background: #e3efe9;">ANOVA mit Messwiederholung</td><td style="padding: 8px; background: #fdf3e7;">Friedman-Test</td><td style="padding: 8px; font-size: 0.9em;">Dieselben Personen laufen ohne, mit langsamer und mit schneller Musik</td></tr>
<tr style="border-bottom: 1px solid #cbd5e1;"><td style="padding: 8px;"><b>Mehrere UV</b></td><td style="padding: 8px; background: #e3efe9;">mehrfaktorielle ANOVA</td><td style="padding: 8px; background: #fdf3e7;">–</td><td style="padding: 8px; font-size: 0.9em;">Musik (ohne / mit) × Geschlecht</td></tr>
</table>
</div>
 
### Zusammenhangshypothesen
 
<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 12px; padding: 10px; color: #1f2933;">
<table style="width: 100%; border-collapse: collapse; font-size: 0.9em;">
<tr><th style="text-align: left; padding: 8px;">Situation</th><th style="padding: 8px; background: #2f6f57; color: #ffffff;">Parametrisch</th><th style="padding: 8px; background: #e08a1e; color: #ffffff;">Nichtparametrisch</th><th style="text-align: left; padding: 8px;">Beispiel</th></tr>
<tr style="border-bottom: 1px solid #cbd5e1;"><td style="padding: 8px;">2 metrische Variablen</td><td style="padding: 8px; background: #e3efe9;">Pearson-Korrelation (<i>r</i>)</td><td style="padding: 8px; background: #fdf3e7;">Spearman-Rangkorrelation (ρ)</td><td style="padding: 8px; font-size: 0.9em;">Musiktempo (BPM) und gelaufene Strecke</td></tr>
<tr style="border-bottom: 1px solid #cbd5e1;"><td style="padding: 8px;">Vorhersage einer AV durch eine oder mehrere UV</td><td style="padding: 8px; background: #e3efe9;">(multiple) lineare Regression</td><td style="padding: 8px; background: #fdf3e7;">–</td><td style="padding: 8px; font-size: 0.9em;">Vorhersage der Strecke durch Musiktempo und Trainingsumfang</td></tr>
<tr style="border-bottom: 1px solid #cbd5e1;"><td style="padding: 8px;">2 nominale Variablen</td><td style="padding: 8px; background: #e3efe9;">–</td><td style="padding: 8px; background: #fdf3e7;">Chi²-Test</td><td style="padding: 8px; font-size: 0.9em;">Musik (ohne / mit) und Cooper-Test bestanden (ja / nein)</td></tr>
</table>
</div>
 
---
 
### Und für unser Beispiel?
 
<div style="display: flex; flex-direction: column; gap: 8px; margin: 12px 0;">
<div style="display: flex; gap: 12px; align-items: flex-start; background: #eef2fb; border-left: 6px solid #4e66bd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">🎯</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Fragestellung</b></div>
<div style="font-size: 0.9em;">Unterschied: Laufen Personen mit Musik weiter?</div>
</div>
</div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #eaf6ee; border-left: 6px solid #2a9a50; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">👥</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Stichproben</b></div>
<div style="font-size: 0.9em;">Zwei unabhängige Gruppen (verschiedene Personen).</div>
</div>
</div>
<div style="display: flex; gap: 12px; align-items: flex-start; background: #f6f1fa; border-left: 6px solid #a74ebd; border-radius: 8px; padding: 10px 14px; color: #1f2933;">
<div style="font-size: 1.6em; line-height: 1;">📏</div>
<div style="flex: 1;">
<div style="font-size: 1em; margin-bottom: 2px;"><b>Abhängige Variable</b></div>
<div style="font-size: 0.9em;">Strecke in Metern ➜ metrisch, in beiden Gruppen normalverteilt.</div>
</div>
</div>
</div>
<div style="border-left: 6px solid #e0a526; background: rgba(224,165,38,0.14); border-radius: 8px; padding: 0.7rem 1.2rem;">
📌 <b>Merke:</b> Geeigneter Test: <b>t-Test für unabhängige Stichproben</b> (bzw. Mann-Whitney-U-Test, falls die Voraussetzungen nicht erfüllt sind).
</div>
<div style="height: 15px;"></div>
<div style="border-left: 6px solid #4e66bd; background: rgba(78,102,189,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
🔜 <b>Ausblick:</b> Im nächsten Kurs <i>Unterschiede analysieren</i> führst du den t-Test für unabhängige Stichproben in JASP durch und prüfst vorher seine Voraussetzungen (Normalverteilung, Varianzhomogenität).
</div>
 
---
## Zusammenfassung
 
<div style="border: 2px solid #2b6cb0; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Deskriptive Statistik**
 
Beschreibt die Stichprobe mit Lagemaßen (Mittelwert, Median), Streuungsmaßen (Standardabweichung, IQR) und Grafiken (Histogramm, Boxplot).
 
</div>
<div style="border: 2px solid #2f855a; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**JASP**
 
*Descriptives → Descriptive Statistics*: AV in *Variables*, Gruppenvariable in *Split*, Kennwerte unter *Statistics*, Grafiken unter *Plots*.
 
</div>
<div style="border: 2px solid #c05621; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Reliabilität und Skalenmittelwerte**
 
Invertierte Items umpolen, interne Konsistenz mit Cronbachs Alpha prüfen (ab .70 akzeptabel), dann den Mittelwert über die Items bilden.
 
</div>


<div style="border: 2px solid #805ad5; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Testauswahl**

Abhängig von Fragestellung (Unterschied / Zusammenhang), Stichprobenart (unabhängig / abhängig), Anzahl der Gruppen und Skalenniveau bzw. Verteilung der AV.
 
</div>

 
---
 
## Check-Up: Grundlagen statistischer Tests
 
 
Beantworte die Fragen. Nach dem Beantworten bekommst du eine kurze Erklärung.
 
**Frage 1:** Welche Aussage gehört zur <b>deskriptiven</b> Statistik?
 
- [( )] Musik verbessert die Ausdauerleistung von Sportstudierenden signifikant (p < ,05).
- [(X)] Die Standardabweichung der Gruppe ohne Musik beträgt 94,75 m.
- [( )] Der Unterschied zwischen den Gruppen lässt sich auf alle Sportstudierenden übertragen.
[[?]] Beschreibt die Aussage nur die Stichprobe?
 
<details>
<summary><b>👉 Erklärung</b></summary>
Die Standardabweichung beschreibt nur die Streuung <b>in der vorliegenden Stichprobe</b>. Aussagen über Signifikanz oder die Übertragbarkeit gehören zur inferenziellen Statistik.
 
</details>
**Frage 2:** In welches Feld ziehst du in JASP die Variable <b>Gruppe</b>, um die Kennwerte getrennt nach Gruppen zu erhalten?
 
- [( )] Variables
- [(X)] Split
- [( )] Frequency tables
<details>
<summary><b>👉 Erklärung</b></summary>
Über das Feld <b>Split</b> werden alle Kennwerte und Grafiken getrennt für jede Gruppe ausgegeben.
 
</details>
**Frage 3:** Die Reliabilitätsanalyse der Motivationsskala ergibt nach dem Umpolen von M3 α = ,84. Wie ist dieser Wert einzuschätzen?
 
- [( )] nicht akzeptabel
- [( )] gerade noch akzeptabel
- [(X)] gut
[[?]] Faustregel: ,70 / ,80 / ,90
 
<details>
<summary><b>👉 Erklärung</b></summary>
Werte ab ,80 gelten als gut. Die Items erfassen weitgehend dasselbe Merkmal, ein Skalenmittelwert kann gebildet werden.
 
</details>
**Frage 4:** Was passiert, wenn das invertierte Item <b>nicht</b> umgepolt wird?
 
- [(X)] Die Reliabilität sinkt, weil das Item den anderen Items entgegenläuft.
- [( )] Die Reliabilität steigt, weil die Items unterschiedlicher werden.
- [( )] Nichts, JASP polt invertierte Items automatisch um.
<details>
<summary><b>👉 Erklärung</b></summary>
Ein nicht umgepoltes Item korreliert negativ mit den übrigen Items und senkt die interne Konsistenz. JASP erkennt invertierte Items nicht automatisch.
 
</details>
**Frage 5:** Der Shapiro-Wilk-Test ergibt in einer Gruppe <i>p</i> = ,012. Was bedeutet das?
 
- [( )] Die Daten sind normalverteilt.
- [(X)] Die Daten weichen signifikant von der Normalverteilung ab.
- [( )] Der Unterschied zwischen den Gruppen ist signifikant.
[[?]] Wie lautet die H0 des Tests?
 
<details>
<summary><b>👉 Erklärung</b></summary>
Die H0 des Shapiro-Wilk-Tests lautet „Die Daten sind normalverteilt“. Bei <i>p</i> &lt; ,05 wird sie verworfen. Prüfe zusätzlich den Q-Q-Plot und erwäge einen nichtparametrischen Test.
 
</details>
**Frage 6:** Alle 20 Personen laufen den Cooper-Test <b>einmal ohne und einmal mit Musik</b>. Welcher Test passt, wenn die Daten normalverteilt sind?
 
- [( )] t-Test für unabhängige Stichproben
- [(X)] t-Test für verbundene Stichproben
- [( )] einfaktorielle ANOVA
- [( )] Pearson-Korrelation
[[?]] Dieselben oder verschiedene Personen?
 
<details>
<summary><b>👉 Erklärung</b></summary>
Dieselben Personen werden zweimal gemessen ➜ abhängige Stichproben ➜ t-Test für verbundene Stichproben.
 
</details>
**Frage 7:** Drei Gruppen laufen <b>ohne Musik, mit langsamer und mit schneller Musik</b>. Die Daten sind <b>nicht</b> normalverteilt. Welcher Test passt?
 
- [( )] einfaktorielle ANOVA
- [( )] Friedman-Test
- [(X)] Kruskal-Wallis-Test
- [( )] Wilcoxon-Test
<details>
<summary><b>👉 Erklärung</b></summary>
Mehr als zwei unabhängige Gruppen mit nicht normalverteilten Daten ➜ Kruskal-Wallis-Test.
 
</details>
**Frage 8:** Es soll untersucht werden, ob das <b>Musiktempo (BPM)</b> mit der <b>gelaufenen Strecke</b> zusammenhängt. Beide Variablen sind metrisch und normalverteilt. Welcher Test passt?
 
- [(X)] Pearson-Korrelation
- [( )] Chi²-Test
- [( )] t-Test für unabhängige Stichproben
<details>
<summary><b>👉 Erklärung</b></summary>
Zusammenhang zwischen zwei metrischen, normalverteilten Variablen ➜ Pearson-Korrelation.
 
</details>
---
 
## Literatur
 
* Cohen, J. (1988). <i>Statistical power analysis for the behavioral sciences</i> (2nd ed.). Lawrence Erlbaum.
* Döring, N. & Bortz, J. (2016). <i>Forschungsmethoden und Evaluation in den Sozial- und Humanwissenschaften</i> (5. Aufl.). Springer.
* Eid, M., Gollwitzer, M. & Schmitt, M. (2017). <i>Statistik und Forschungsmethoden</i> (5. Aufl.). Beltz.
* JASP Team (2024). <i>JASP</i> (Version 0.19) [Computer software]. https://jasp-stats.org/
 








