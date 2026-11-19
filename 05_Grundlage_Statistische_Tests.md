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



[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/EUF-SpoWis/Wissenschaftliches-Arbeiten/main/06_Zusammenhaenge_analysieren.md)

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


# Grundlagen statistischer Tests
 
**Teil 1: Deskriptive Statistik mit JASP und Übersicht über statistische Tests**
 
<div style="border: 2px solid #2b6cb0; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem; background-color: #ebf4ff;">
**Was erwartet dich in diesem Kurs?**
 
Du lernst, wie man Daten mithilfe von Kennwerten und Grafiken beschreibt und diese Kennwerte in JASP berechnet.
 
</div>
<div style="border: 2px solid #2f855a; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem; background-color: #f0fff4;">
**Beispiel**
 
Wir arbeiten weiterhin mit der Fragestellung aus dem Grundlagenkurs: *Hat Musik einen Effekt auf die Ausdauerleistung?*
 
</div>
<div style="border: 2px solid #c05621; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem; background-color: #fffaf0;">
**Was kommt danach?**
 
Am Ende erhälst du eine Übersicht darüber, welcher statistische Test für welche Fragestellung geeignet ist.
 
</div>

 
## Das Beispiel: Musik und Ausdauerleistung
 
<div style="border: 2px solid #2f855a; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Fragestellung**
 
Laufen Sportstudierende mit Musik weiter als ohne Musik?
 
</div>
<div style="border: 2px solid #2f855a; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Studiendesign**
 
* 20 Sportstudierende werden zufällig zwei Gruppen zugeteilt.
* Gruppe 1 läuft **ohne Musik**, Gruppe 2 läuft **mit Musik**.
* Alle absolvieren einen **Cooper-Test** (12 Minuten Laufen).
</div>
<div style="border: 2px solid #2f855a; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Variablen**
 
* **Unabhängige Variable (UV):** Musik (ohne Musik / mit Musik) – nominalskaliert
* **Abhängige Variable (AV):** Ausdauerleistung = gelaufene Strecke in Metern – verhältnisskaliert
</div>
 
<details>
<summary><b>👉 Rohdaten</b></summary>

Die gelaufene Strecke in Metern im Cooper-Test:
 
<!-- data-type="none" -->
| Person | Gruppe      | Strecke (m) |
| :----: | :---------- | ----------: |
|   1    | ohne Musik  |        2350 |
|   2    | ohne Musik  |        2480 |
|   3    | ohne Musik  |        2410 |
|   4    | ohne Musik  |        2600 |
|   5    | ohne Musik  |        2290 |
|   6    | ohne Musik  |        2520 |
|   7    | ohne Musik  |        2450 |
|   8    | ohne Musik  |        2380 |
|   9    | ohne Musik  |        2550 |
|   10   | ohne Musik  |        2470 |
|   11   | mit Musik   |        2500 |
|   12   | mit Musik   |        2620 |
|   13   | mit Musik   |        2480 |
|   14   | mit Musik   |        2710 |
|   15   | mit Musik   |        2440 |
|   16   | mit Musik   |        2590 |
|   17   | mit Musik   |        2650 |
|   18   | mit Musik   |        2530 |
|   19   | mit Musik   |        2760 |
|   20   | mit Musik   |        2560 |

</details>
 
<div style="border: 2px solid #c05621; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem; background-color: #fffaf0;">
**Problem:** Aus 20 einzelnen Zahlen lässt sich kaum ablesen, ob Musik einen Unterschied macht. Wir brauchen Kennwerte, die die Daten **zusammenfassen**.
 
</div>
 
## Deskriptive vs. inferenzielle Statistik
 
<div style="border: 2px solid #2b6cb0; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Deskriptive Statistik (beschreibend)**
 
* fasst die Daten der **Stichprobe** zusammen
* nutzt Kennwerte (z. B. Mittelwert) und Grafiken (z. B. Boxplot)
* Beispiel: *„Die Gruppe mit Musik lief im Mittel 2584 m, die Gruppe ohne Musik 2450 m.“*
</div>
<div style="border: 2px solid #805ad5; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Inferenzielle Statistik (schließend)**
 
* überprüft, ob sich Ergebnisse auf die **Population** übertragen lassen
* nutzt statistische Tests (z. B. t-Test) und liefert p-Werte und Effektstärken
* Beispiel: *„Ist der Unterschied von 134 m groß genug, um nicht nur zufällig zu sein?“*
</div>
**Merke:** Die deskriptive Statistik ist immer der erste Schritt – bevor getestet wird, müssen die Daten beschrieben werden.
 
 
## Deskriptive Statistik in JASP
 
[JASP](https://jasp-stats.org/) ist eine kostenlose Open-Source-Statistiksoftware. Sie ist für Windows, macOS und Linux verfügbar.
 
 
### Die Daten
 
<div style="border: 2px solid #2b6cb0; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Datenformat**
 
Jede Zeile ist eine Person, jede Spalte eine Variable. Speichern Sie die Daten als CSV-Datei (z. B. `ausdauer_musik.csv`):
 
``` text
Person,Gruppe,Strecke
1,ohne Musik,2350
2,ohne Musik,2480
3,ohne Musik,2410
4,ohne Musik,2600
5,ohne Musik,2290
6,ohne Musik,2520
7,ohne Musik,2450
8,ohne Musik,2380
9,ohne Musik,2550
10,ohne Musik,2470
11,mit Musik,2500
12,mit Musik,2620
13,mit Musik,2480
14,mit Musik,2710
15,mit Musik,2440
16,mit Musik,2590
17,mit Musik,2650
18,mit Musik,2530
19,mit Musik,2760
20,mit Musik,2560
```
 
</div>
 
### Video: Deskriptive Statistik in JASP berechnen
 
<!-- TODO: Platzhalter durch den Link zum JASP-Video ersetzen -->
!?[Deskriptive Statistik in JASP](https://www.youtube.com/watch?v=VIDEO-ID)
 
<div style="border: 2px solid #2b6cb0; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Im Video sehen Sie, wie Sie …**
 
1. die Datei `ausdauer_musik.csv` in JASP öffnen und das Skalenniveau prüfen,
2. unter *Descriptives → Descriptive Statistics* die Kennwerte getrennt nach Gruppe (*Split*) anfordern,
3. Histogramme und Boxplots erstellen.
</div>
 
### Ergebnisse lesen
 
So sieht die Ausgabe in JASP aus:
 
<!-- data-type="none" -->
| Descriptive Statistics |  Strecke (ohne Musik) | Strecke (mit Musik) |
| :--------------------- | --------------------: | ------------------: |
| Valid                  |                    10 |                  10 |
| Median                 |              2460.000 |            2575.000 |
| Mean                   |              2450.000 |            2584.000 |
| Std. Deviation         |                94.751 |             102.546 |
| Variance               |              8977.778 |           10515.556 |
| Range                  |               310.000 |             320.000 |
| Minimum                |              2290.000 |            2440.000 |
| Maximum                |              2600.000 |            2760.000 |
| 25th percentile        |              2387.500 |            2507.500 |
| 50th percentile        |              2460.000 |            2575.000 |
| 75th percentile        |              2510.000 |            2642.500 |
 
<div style="border: 2px solid #2f855a; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem; background-color: #f0fff4;">
**Interpretation**
 
* Die Gruppe **mit Musik** lief im Mittel **134 m weiter** ($M = 2584$ m) als die Gruppe **ohne Musik** ($M = 2450$ m).
* Mittelwert und Median liegen in beiden Gruppen nah beieinander → kein Hinweis auf eine stark schiefe Verteilung.
* Die Streuung ist in beiden Gruppen ähnlich ($SD = 94{,}75$ m vs. $SD = 102{,}55$ m).
</div>
<div style="border: 2px solid #c05621; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem; background-color: #fffaf0;">
**Aber:** Ob dieser Unterschied von 134 m nur zufällig zustande gekommen ist, kann die deskriptive Statistik **nicht** beantworten. Dafür benötigen wir einen **statistischen Test**.
 
</div>
 
### Ergebnisse berichten (APA-Stil)
 
<div style="border: 2px solid #2b6cb0; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Formulierungsbeispiel**
 
*Die Teilnehmenden, die mit Musik liefen, legten im Cooper-Test im Mittel eine größere Strecke zurück (M = 2584 m, SD = 102.55) als die Teilnehmenden ohne Musik (M = 2450 m, SD = 94.75).*
 
</div>
 
## Zusatzbeispiel: Fragebogen, Reliabilität und Skalenmittelwerte
 
<div style="border: 2px solid #2f855a; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Zusätzlich erhobener Fragebogen**
 
Nach dem Cooper-Test füllen alle 20 Personen einen kurzen Fragebogen zur **Laufmotivation** aus. Die Skala besteht aus vier Items, die auf einer Likert-Skala von 1 (*trifft gar nicht zu*) bis 5 (*trifft voll zu*) beantwortet werden:
 
| Item | Aussage                                          |
| :--: | :----------------------------------------------- |
| M1   | Ich hatte Lust, weiterzulaufen.                  |
| M2   | Das Laufen hat mir Spaß gemacht.                 |
| M3   | Ich wollte möglichst schnell aufhören. *(invertiert)* |
| M4   | Ich habe mich beim Laufen angestrengt, weil ich es wollte. |
 
</div>
<div style="border: 2px solid #2b6cb0; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Reliabilität: Messen die Items dasselbe?**
 
Bevor wir die Items zu einem Wert zusammenfassen, prüfen wir die **interne Konsistenz** der Skala – also, ob die Items dasselbe Merkmal erfassen.
 
* **Cronbachs Alpha ($\alpha$)** liegt zwischen 0 und 1.
* Faustregel: ab **.70 akzeptabel**, ab **.80 gut**, ab **.90 sehr gut**.
* Die Kennwerte *„if item dropped“* zeigen, ob ein einzelnes Item die Reliabilität verschlechtert.
</div>
<div style="border: 2px solid #c05621; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem; background-color: #fffaf0;">
**Achtung: invertierte Items!**
 
Item M3 ist negativ formuliert. Es muss **vor** der Reliabilitätsanalyse umgepolt werden (1 → 5, 2 → 4, …), sonst sinkt die Reliabilität deutlich. Formel: $M3_{neu} = 6 - M3$
 
</div>
<div style="border: 2px solid #805ad5; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Skalenmittelwert bilden**
 
Ist die Reliabilität ausreichend, wird pro Person der Mittelwert über alle Items berechnet:
 
$$
\text{Motivation} = \frac{M1 + M2 + M3_{neu} + M4}{4}
$$
 
*Beispiel:* Eine Person antwortet M1 = 4, M2 = 5, M3 = 2 (umgepolt: 4) und M4 = 3 → Motivation = $\frac{4 + 5 + 4 + 3}{4} = 4$
 
Der Skalenmittelwert kann anschließend wie die Strecke deskriptiv beschrieben werden (z. B. getrennt nach Gruppe).
 
</div>
 
### Video: Reliabilitätsanalyse und Skalenmittelwerte in JASP
 
<!-- TODO: Platzhalter durch den Link zum JASP-Tutorial ersetzen -->
!?[Reliabilitätsanalyse und Skalenmittelwerte in JASP](https://www.youtube.com/watch?v=VIDEO-ID)
 
<div style="border: 2px solid #2b6cb0; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Im Tutorial sehen Sie, wie Sie …**
 
1. das invertierte Item M3 umpolen,
2. unter *Reliability → Unidimensional Reliability* Cronbachs Alpha berechnen und die Werte *if item dropped* ablesen,
3. über eine neue berechnete Spalte (*Compute column*) den Skalenmittelwert bilden.
</div>
 
## Übersicht: Welcher statistische Test?
 
Die Wahl des Tests hängt von drei Fragen ab:
 
<div style="border: 2px solid #2b6cb0; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**1. Was ist die Fragestellung?**
 
* **Unterschied:** Unterscheiden sich Gruppen oder Messzeitpunkte? (z. B. Laufen Personen mit Musik weiter als ohne?)
* **Zusammenhang:** Hängen zwei Variablen zusammen? (z. B. Hängt das Musiktempo mit der gelaufenen Strecke zusammen?)
</div>
<div style="border: 2px solid #2f855a; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**2. Wie sind die Daten erhoben worden?**
 
* **Unabhängige Stichproben:** verschiedene Personen in den Gruppen (z. B. Gruppe A ohne Musik, Gruppe B mit Musik)
* **Abhängige Stichproben:** dieselben Personen werden mehrfach gemessen (z. B. alle laufen einmal ohne und einmal mit Musik)
* **Anzahl der Gruppen bzw. Messzeitpunkte:** zwei oder mehr als zwei?
</div>
<div style="border: 2px solid #805ad5; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**3. Welches Skalenniveau und welche Verteilung hat die AV?**
 
* **Metrisch und annähernd normalverteilt** → **parametrische** Tests
* **Ordinal oder nicht normalverteilt** (bei kleinen Stichproben) → **nicht-parametrische** Tests
</div>
 
### Entscheidungsbaum
 
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
 
*Nicht-parametrische Alternativen findest du in den folgenden Tabellen.*

### Nicht-Parametrische Tests


<div style="border: 2px solid #2f855a; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Wann werden sie eingesetzt?**
 
* bei **ordinalskalierten** Daten (z. B. Rangplätze, einzelne Likert-Items)
* wenn metrische Daten **nicht normalverteilt** sind – vor allem bei kleinen Stichproben
* bei deutlichen **Ausreißern**
</div>
<div style="border: 2px solid #c05621; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem; background-color: #fffaf0;">
**Vor- und Nachteile**
 
* **+** robust gegenüber Ausreißern und schiefen Verteilungen
* **−** geringere Teststärke: Sind die Voraussetzungen für einen parametrischen Test erfüllt, findet dieser einen tatsächlichen Effekt eher.
</div>

<div style="border: 2px solid #2b6cb0; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Grafisch**
 
* **Histogramm:** Ist die Verteilung annähernd glockenförmig und symmetrisch?
* **Q-Q-Plot:** Liegen die Punkte nah an der Diagonalen? Systematische Abweichungen (z. B. Bögen oder Ausreißer an den Enden) sprechen gegen eine Normalverteilung.
</div>
<div style="border: 2px solid #805ad5; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**Statistisch: Shapiro-Wilk-Test**
 
* $H_0$: Die Daten sind normalverteilt.
* $p < .05$ → signifikante Abweichung von der Normalverteilung → nicht-parametrischen Test erwägen
* $p \geq .05$ → keine signifikante Abweichung → parametrischer Test möglich
*Beispiel Ausdauerleistung:* ohne Musik $W = 0.99$, $p = .998$; mit Musik $W = 0.97$, $p = .928$ → in beiden Gruppen keine Abweichung von der Normalverteilung.
 
</div>
<div style="border: 2px solid #2f855a; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem;">
**In JASP**
 
* *Descriptives → Descriptive Statistics:* unter *Statistics → Distribution* **Shapiro-Wilk test** aktivieren, unter *Plots* **Q-Q plots** und **Distribution plots**
* Alternativ direkt im t-Test oder in der ANOVA unter *Assumption Checks* → **Normality**
</div>
<div style="border: 2px solid #c05621; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem; background-color: #fffaf0;">
**Wichtig**
 
* Die Normalverteilung wird **getrennt für jede Gruppe** geprüft (bzw. für die Differenzen bei abhängigen Stichproben).
* Bei **kleinen** Stichproben erkennt der Shapiro-Wilk-Test Abweichungen kaum, bei **großen** wird er schon bei kleinen Abweichungen signifikant → immer zusätzlich die Grafiken betrachten.
* Ab etwa 30 Personen pro Gruppe sind t-Test und ANOVA relativ robust gegenüber Verletzungen der Normalverteilung.
</div>
 
 
### Unterschiedshypothesen
 
<!-- data-type="none" -->
| Situation                                  | Parametrischer Test             | Nicht-parametrische Alternative | Beispiel Ausdauerleistung                                                                 |
| :----------------------------------------- | :------------------------------ | :------------------------------ | :---------------------------------------------------------------------------------------- |
| 2 unabhängige Gruppen                      | t-Test für unabhängige Stichproben | Mann-Whitney-U-Test           | Gruppe ohne Musik vs. Gruppe mit Musik                                                    |
| 2 abhängige Messungen                      | t-Test für abhängige Stichproben   | Wilcoxon-Vorzeichen-Rang-Test | Dieselben Personen laufen einmal ohne und einmal mit Musik                                |
| > 2 unabhängige Gruppen                    | einfaktorielle ANOVA            | Kruskal-Wallis-Test             | Gruppen ohne Musik vs. langsame Musik vs. schnelle Musik                                  |
| > 2 abhängige Messungen                    | ANOVA mit Messwiederholung      | Friedman-Test                   | Dieselben Personen laufen ohne, mit langsamer und mit schneller Musik                     |
| 2 oder mehr unabhängige Variablen          | mehrfaktorielle ANOVA           | –                               | Musik (ohne / mit) × Geschlecht                                                           |
 
 
### Zusammenhangshypothesen
 
<!-- data-type="none" -->
| Situation                                   | Test                                | Beispiel Ausdauerleistung                                                   |
| :------------------------------------------ | :---------------------------------- | :-------------------------------------------------------------------------- |
| 2 metrische, normalverteilte Variablen      | Pearson-Korrelation ($r$)           | Musiktempo (BPM) und gelaufene Strecke                                      |
| ordinale oder nicht normalverteilte Daten   | Spearman-Rangkorrelation ($\rho$)   | Rangplatz im Lauf und Musiktempo                                            |
| Vorhersage einer AV durch eine/mehrere UV   | (multiple) lineare Regression       | Vorhersage der Strecke durch Musiktempo und wöchentlichen Trainingsumfang   |
| 2 nominale Variablen                        | Chi²-Test                           | Musik (ohne / mit) und Cooper-Test bestanden (ja / nein)                    |
 
 
### Und für unser Beispiel?
 
<div style="border: 2px solid #2f855a; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem; background-color: #f0fff4;">
**Unsere Studie im Überblick**
 
* **Fragestellung:** Unterschied (Laufen Personen mit Musik weiter?)
* **Stichproben:** zwei unabhängige Gruppen (verschiedene Personen)
* **AV:** Strecke in Metern → metrisch
→ Geeigneter Test: **t-Test für unabhängige Stichproben** (bzw. Mann-Whitney-U-Test, falls die Voraussetzungen nicht erfüllt sind)
 
</div>
<div style="border: 2px solid #c05621; border-radius: 8px; padding: 1rem 1.5rem; margin-bottom: 1rem; background-color: #fffaf0;">
**Ausblick**
 
Im nächsten Kapitel führen wir den t-Test für unabhängige Stichproben in JASP durch und prüfen vorher seine Voraussetzungen (Normalverteilung, Varianzhomogenität).
 
</div>
 
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
 
## Quiz
 
Testen Sie Ihr Wissen zu allen Themen dieses Kurses.
 
 
**Deskriptiv oder inferenziell?**
 
Welche Aussage gehört zur **deskriptiven** Statistik?
 
- [( )] Musik verbessert die Ausdauerleistung von Sportstudierenden signifikant (p < .05).
- [(X)] Die Standardabweichung der Gruppe ohne Musik beträgt 94,75 m.
- [( )] Der Unterschied zwischen den Gruppen lässt sich auf alle Sportstudierenden übertragen.
***********************************************************************
Die Standardabweichung beschreibt nur die Streuung **in der vorliegenden Stichprobe**. Aussagen über Signifikanz oder die Übertragbarkeit auf alle Sportstudierenden gehören zur inferenziellen Statistik.
***********************************************************************

**JASP-Ausgabe**
 
In welches Feld ziehen Sie in JASP die Variable **Gruppe**, um die Kennwerte getrennt nach Gruppen zu erhalten?
 
- [( )] Variables
- [(X)] Split
- [( )] Frequency tables
***********************************************************************
Über das Feld **Split** werden alle Kennwerte und Grafiken getrennt für jede Ausprägung der Gruppenvariable ausgegeben.
***********************************************************************
 
 
**Reliabilität und Skalenmittelwerte**
 
Die Reliabilitätsanalyse der Motivationsskala ergibt $\alpha = .82$. Wie ist dieser Wert einzuschätzen?
 
- [( )] nicht akzeptabel
- [( )] gerade noch akzeptabel
- [(X)] gut
***********************************************************************
Werte ab .80 gelten als gut. Die Items erfassen also weitgehend dasselbe Merkmal, und ein Skalenmittelwert kann gebildet werden.
***********************************************************************

 
Was passiert, wenn das invertierte Item **nicht** umgepolt wird?
 
- [(X)] Die Reliabilität sinkt, weil das Item den anderen Items entgegenläuft.
- [( )] Die Reliabilität steigt, weil die Items unterschiedlicher werden.
- [( )] Nichts, JASP polt invertierte Items automatisch um.
***********************************************************************
Ein nicht umgepoltes Item korreliert negativ mit den übrigen Items und senkt dadurch die interne Konsistenz. JASP erkennt invertierte Items nicht automatisch – sie müssen vorher umgepolt bzw. in der Analyse als *reverse-scaled items* angegeben werden.
***********************************************************************
 
 
**Testauswahl**
 
Alle 20 Personen laufen den Cooper-Test **einmal ohne und einmal mit Musik**. Welcher Test ist geeignet, wenn die Daten normalverteilt sind?
 
- [( )] t-Test für unabhängige Stichproben
- [(X)] t-Test für abhängige Stichproben
- [( )] einfaktorielle ANOVA
- [( )] Pearson-Korrelation
***********************************************************************
Da **dieselben Personen** zweimal gemessen werden, liegen abhängige Stichproben vor. Bei zwei Messzeitpunkten und normalverteilten Daten ist der t-Test für abhängige Stichproben geeignet.
***********************************************************************
 
Drei Gruppen laufen **ohne Musik, mit langsamer Musik und mit schneller Musik**. Die Daten sind **nicht** normalverteilt. Welcher Test ist geeignet?
 
- [( )] einfaktorielle ANOVA
- [( )] Friedman-Test
- [(X)] Kruskal-Wallis-Test
- [( )] Wilcoxon-Vorzeichen-Rang-Test
***********************************************************************
Es handelt sich um **mehr als zwei unabhängige Gruppen** mit nicht normalverteilten Daten. Die nicht-parametrische Alternative zur einfaktoriellen ANOVA ist der Kruskal-Wallis-Test.
***********************************************************************
 
Es soll untersucht werden, ob das **Musiktempo (BPM)** mit der **gelaufenen Strecke** zusammenhängt. Beide Variablen sind metrisch und normalverteilt. Welcher Test ist geeignet?
 
- [(X)] Pearson-Korrelation
- [( )] Chi²-Test
- [( )] t-Test für unabhängige Stichproben
***********************************************************************
Bei einem **Zusammenhang** zwischen zwei metrischen, normalverteilten Variablen ist die Pearson-Korrelation geeignet.
***********************************************************************
 
















