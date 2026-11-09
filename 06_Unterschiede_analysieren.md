<!--
author: Swantje Brandt
email: swantje.brandt@uni-flensburg.de
version: 0.0.1
language: de
narrator: Deutsch Female

import:  https://raw.githubusercontent.com/EUF-SpoWis/M1_Einfuehrung_Sportwissenschaft/refs/heads/main/config.md
import: https://raw.githubusercontent.com/liaTemplates/PyScript/main/README.md

link:   https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css
        https://cdn.jsdelivr.net/gh/EUF-SpoWis/Wissenschaftliches-Arbeiten@main/Lia-Anpassungen/Ausblendungen.css

-->

## Unterschiede analysieren


[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/EUF-SpoWis/Wissenschaftliches-Arbeiten/main/05_Unterschiede_analysieren.md)


| Parameter                | Kursinformationen                                                                               |
| ------------------------ | ----------------------------------------------------------------------------------------------- |
| **Veranstaltung:**       | Wissenschaftliches Arbeiten                                                                                 |
| **Semester:**            |                                                                                 |
| **Hochschule:**          | `Europa-Universität Flensburg`                                                                  |
| **Inhalte:**             | `Sportwissenschaftliche Methoden mit Fokus auf der Analyse von Unterschieden `                  |
| **Link auf GitHub:**     | https://github.com/EUF-SpoWis/Wissenschaftliches-Arbeiten/blob/main/05_Unterschiede_analysieren.md      |
| **Autoren:**             | @author                                                                                      |

> (c) Alle Rechte vorbehalten. 


---

## Überblick: Unterschiede testen

--{{0}}--<div style="border-left: 6px solid #2e9e5b; background: rgba(46,158,91,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
💡 <b>Lehrbuch Hinweis:</b> In diesem Kurs lernst du, <b>welchen Test</b> du für Unterschiede brauchst, <b>wie du ihn in JASP durchführst</b> und <b>wie du das Ergebnis liest und berichtest</b>. Als Beispiel dient wie im Grundlagenkurs der 12-Minuten-Lauf mit und ohne Musik.
</div>

<div style="height: 15px;"></div>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #eef2fb; border: 2px solid #4e66bd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">👥</div>
<div style="text-align: center; font-size: 1.1em;"><b>Unabhängige Stichproben</b></div>
<div style="font-size: 0.9em;">Jede Person gehört nur zu <b>einer</b> Gruppe.</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #ffffff; border-left: 4px solid #4e66bd; border-radius: 0 8px 8px 0; font-size: 0.85em;">🏃🏾‍♀️ 20 Läufer:innen laufen <b>mit</b> Musik, 20 <b>andere</b> ohne Musik.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #eaf6ee; border: 2px solid #2a9a50; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔁</div>
<div style="text-align: center; font-size: 1.1em;"><b>Abhängige Stichproben</b></div>
<div style="font-size: 0.9em;">Dieselben Personen werden <b>mehrfach</b> gemessen.</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #ffffff; border-left: 4px solid #4e66bd; border-radius: 0 8px 8px 0; font-size: 0.85em;">🏃🏾‍♀️ Dieselben 20 Läufer:innen laufen <b>mit</b> und <b>ohne</b> Musik.</div>
</div>

</div>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 12px; padding: 10px; color: #1f2933;">
<table style="width: 100%; border-collapse: collapse; font-size: 0.9em;">
<tr><th style="text-align: left; padding: 8px;">Stichprobe</th><th style="padding: 8px; background: #2f6f57; color: #ffffff;">Parametrisch</th><th style="padding: 8px; background: #e08a1e; color: #ffffff;">Nichtparametrisch</th></tr>
<tr style="border-bottom: 1px solid #cbd5e1;"><td style="padding: 8px;"><b>Unabhängig</b><br><span style="font-size: 0.85em;">2 Gruppen</span></td><td style="padding: 8px; background: #e3efe9;">t-Test für unabhängige Stichproben</td><td style="padding: 8px; background: #fdf3e7;">Mann-Whitney-U-Test</td></tr>
<tr style="border-bottom: 1px solid #cbd5e1;"><td style="padding: 8px;"><b>Unabhängig</b><br><span style="font-size: 0.85em;">mehr als 2 Gruppen</span></td><td style="padding: 8px; background: #e3efe9;">ANOVA</td><td style="padding: 8px; background: #fdf3e7;">Kruskal-Wallis-Test</td></tr>
<tr style="border-bottom: 1px solid #cbd5e1;"><td style="padding: 8px;"><b>Abhängig</b><br><span style="font-size: 0.85em;">2 Messungen</span></td><td style="padding: 8px; background: #e3efe9;">t-Test für verbundene Stichproben</td><td style="padding: 8px; background: #fdf3e7;">Wilcoxon-Test</td></tr>
<tr style="border-bottom: 1px solid #cbd5e1;"><td style="padding: 8px;"><b>Abhängig</b><br><span style="font-size: 0.85em;">mehr als 2 Messungen</span></td><td style="padding: 8px; background: #e3efe9;">ANOVA mit Messwiederholung</td><td style="padding: 8px; background: #fdf3e7;">Friedman-Test</td></tr>
</table>
</div>

<div style="height: 10px;"></div>

<div style="border-left: 6px solid #e0a526; background: rgba(224,165,38,0.14); border-radius: 8px; padding: 0.7rem 1.2rem;">
📌 <b>Merke:</b> Die Zeile bestimmst du über das <b>Studiendesign</b> (dieselben oder verschiedene Personen, wie viele Bedingungen). Die Spalte bestimmst du über die <b>Voraussetzungen</b> deiner Daten (metrisch, normalverteilt, ähnliche Streuung).
</div>

<div style="height: 15px;"></div>

{{1}} <section>

<span style="font-size: 1.1em;"><b>Unser Datensatz aus dem Musikbeispiel:</b></span>

| Person | Bedingung | Strecke (m) | Borg-Wert |
| :-: | :-- | :-: | :-: |
| 1 | mit Musik | 2480 | 11 |
| 2 | mit Musik | 2650 | 13 |
| 3 | ohne Musik | 2350 | 13 |
| 4 | ohne Musik | 2480 | 15 |
| … | … | … | … |

<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
🏃🏾‍♀️ <span style="background: linear-gradient(transparent 55%, rgba(71, 69, 173, 0.55) 60%);"><b>Strecke (m)</b></span> 🏃🏾‍♀️<br>
Ausdauerleistung, <b>metrisch</b>. Das ist meist die abhängige Variable für parametrische Tests.
</div>

<div style="border: 2px solid #2a9a50; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
📋 <span style="background: linear-gradient(transparent 55%, rgba(66, 162, 61, 0.55) 60%);"><b>Borg-Wert (6 bis 20)</b></span> 📋<br>
Anstrengungsempfinden, streng genommen <b>ordinal</b>. Dafür passen eher nichtparametrische Tests.
</div>

</section>

{{2}} <section>

#### So gehst du in JASP grundsätzlich vor

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📂</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Daten laden</b></div>
<div style="font-size: 0.9em;">Datei (.csv oder .xlsx) über „Open“ öffnen. Jede Zeile ist eine Person bzw. Messung.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🏷️</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Skalenniveau prüfen</b></div>
<div style="font-size: 0.9em;">In der Spaltenüberschrift das Symbol anklicken und nominal, ordinal oder scale einstellen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔍</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Daten ansehen</b></div>
<div style="font-size: 0.9em;">Unter „Descriptives“ Kennwerte, Histogramme und Boxplots anfordern.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧪</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Test wählen</b></div>
<div style="font-size: 0.9em;">Passende Analyse im Menü wählen und Variablen in die Felder ziehen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Voraussetzungen prüfen</b></div>
<div style="font-size: 0.9em;">Unter „Assumption Checks“ Normalverteilung und Varianzhomogenität anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📖</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Ergebnis lesen</b></div>
<div style="font-size: 0.9em;">Teststatistik, <i>p</i>-Wert und Effektstärke ablesen und berichten.</div>
</div>

</div>

<!-- TODO: Screenshot JASP-Oberfläche (Datenansicht und Analysefenster) -->

<div style="border-left: 6px solid #e0a526; background: rgba(224,165,38,0.14); border-radius: 8px; padding: 0.7rem 1.2rem;">
📌 <b>Merke:</b> Ein Ergebnis gilt üblicherweise als <b>statistisch signifikant</b>, wenn <i>p</i> &lt; ,05. Der <i>p</i>-Wert sagt <b>nicht</b>, wie groß ein Effekt ist. Dafür brauchst du immer auch eine <b>Effektstärke</b>.
</div>

<div style="height: 15px;"></div>

</section>

---

## t-Test für unabhängige Stichproben

<span style="font-size: 1.1em;"><b>Wann passt der Test?</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🎯</div>
<div style="text-align: center; font-size: 1.1em;"><b>Fragestellung</b></div>
<div style="font-size: 0.9em;">Unterscheiden sich <b>zwei Gruppen</b> im Mittelwert?</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📏</div>
<div style="text-align: center; font-size: 1.1em;"><b>Daten</b></div>
<div style="font-size: 0.9em;">Abhängige Variable <b>metrisch</b>, Gruppenvariable nominal mit 2 Stufen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">👥</div>
<div style="text-align: center; font-size: 1.1em;"><b>Stichprobe</b></div>
<div style="font-size: 0.9em;"><b>Verschiedene</b> Personen in den Gruppen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>Voraussetzungen</b></div>
<div style="font-size: 0.9em;">Normalverteilung in beiden Gruppen, ähnliche Streuung, unabhängige Messungen.</div>
</div>

</div>

<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
🏃🏾‍♀️ <span style="background: linear-gradient(transparent 55%, rgba(71, 69, 173, 0.55) 60%);"><b>Wirkung auf die Ausdauerleistung</b></span> 🏃🏾‍♀️<br>
Laufen Personen <b>mit Musik</b> im 12-Minuten-Lauf weiter als <b>andere</b> Personen <b>ohne Musik</b>? Verglichen werden die mittleren Strecken in Metern.
</div>

<span style="font-size: 1.1em;"><b>Hypothesen</b></span>

| Hypothese | Formulierung im Musikbeispiel |
| :-- | :-- |
| **H0** | Die mittlere Strecke ist mit und ohne Musik gleich (μ<sub>mit</sub> = μ<sub>ohne</sub>). |
| **H1 (ungerichtet)** | Die mittlere Strecke unterscheidet sich (μ<sub>mit</sub> ≠ μ<sub>ohne</sub>). |
| **H1 (gerichtet)** | Mit Musik ist die mittlere Strecke größer (μ<sub>mit</sub> &gt; μ<sub>ohne</sub>). |

{{1}} <section>

<span style="font-size: 1.1em;"><b>Durchführung in JASP</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🏷️</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Variablen einstellen</b></div>
<div style="font-size: 0.9em;">Bedingung als nominal, Strecke als scale.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧪</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Analyse öffnen</b></div>
<div style="font-size: 0.9em;">T-Tests ➜ Classical ➜ Independent Samples T-Test.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔗</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Variablen zuweisen</b></div>
<div style="font-size: 0.9em;">Strecke in „Dependent Variables“, Bedingung in „Grouping Variable“.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">☑️</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Test wählen</b></div>
<div style="font-size: 0.9em;">Unter „Tests“ <b>Student</b> anhaken (Welch bei ungleichen Streuungen).</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">➕</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Zusatzangaben</b></div>
<div style="font-size: 0.9em;">„Mean difference“, „Effect size“ (Cohen’s d) und „Descriptives“ anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Voraussetzungen</b></div>
<div style="font-size: 0.9em;">Unter „Assumption Checks“ Normality und Equality of variances anhaken.</div>
</div>

</div>

<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> T-Tests ➜ Classical ➜ Independent Samples T-Test</div>
<div style="height: 10px;"></div>

<!-- TODO: Screenshot JASP: t-Test für unabhängige Stichproben -->

</section>

{{2}} <section>

<span style="font-size: 1.1em;"><b>Ergebnis lesen</b></span>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Independent Samples T-Test</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;"></th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">t</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">df</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">p</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Mean Difference</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">SE Difference</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Cohen’s d</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Strecke</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2,26</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">38</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,029</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">136,50</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">60,29</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">0,72</td></tr>
</table>
</div>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Descriptives</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Gruppe</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">N</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Mean</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">SD</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">mit Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">20</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2585,50</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">195,33</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">ohne Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">20</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2449,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">185,87</td></tr>
</table>
</div>

<div style="font-size: 0.8em; opacity: 0.7; margin-bottom: 10px;">Fiktive Daten, nachgebaut im Stil der JASP-Ausgabe.</div>

<ul style="font-size: 0.95em;">
<li><b><i>p</i>-Wert:</b> <i>p</i> = ,029 ist kleiner als ,05. Die H0 wird verworfen, der Unterschied ist statistisch signifikant.</li>
<li><b>Richtung:</b> Der Mittelwert mit Musik ist 136,5 m größer als ohne Musik.</li>
<li><b>Cohen’s d:</b> 0,72 entspricht einem mittleren bis großen Effekt.</li>
<li><b>Gleiche Streuung:</b> Levene-Test <i>p</i> = ,756, die Streuungen sind ähnlich (Student-Test passt).</li>
</ul>

<span style="font-size: 1.1em;"><b>Effektstärke einordnen</b></span>

Cohen’s <i>d</i>: ab 0,2 klein, ab 0,5 mittel, ab 0,8 groß (Cohen, 1988). Der Wert zeigt, wie viele Standardabweichungen die Gruppen auseinanderliegen.

</section>

{{3}} <section>

<span style="font-size: 1.1em;"><b>So berichtest du das Ergebnis</b></span>

<div style="border-left: 6px solid #a74ebd; background: #f6f1fa; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
✍️ <b>Musterbericht (APA):</b><br>
<i>Personen mit Musik liefen im Mittel weiter (M = 2585,50 m, SD = 195,33) als Personen ohne Musik (M = 2449,00 m, SD = 185,87), t(38) = 2,26, p = ,029, d = 0,72.</i>
</div>

<details>
<summary><b>👉 Voraussetzungen prüfen und was du bei Verletzung tust</b></summary>

| Voraussetzung | Prüfung in JASP | Ergebnis im Beispiel | Bei Verletzung |
| :-- | :-- | :-- | :-- |
| Normalverteilung | Shapiro-Wilk, Q-Q-Plot | <i>p</i> = ,948 bzw. ,967 ➜ erfüllt | Mann-Whitney-U-Test |
| Gleiche Streuung | Levene-Test | <i>p</i> = ,756 ➜ erfüllt | Welch-Test anhaken |
| Unabhängigkeit | Studiendesign | verschiedene Personen ➜ erfüllt | anderer Test (verbunden) |

</details>

**Frage 1:** Im Levene-Test ist p = ,03. Was tust du?

- [( )] Student-Test beibehalten
- [(X)] Welch-Test anhaken
- [( )] Chi-Quadrat-Test wählen
- [( )] Nichts, der Test ist ungültig

<details>
<summary><b>👉 Erklärung</b></summary>

Ein signifikanter Levene-Test zeigt ungleiche Streuungen. Der Welch-Test ist dafür robust.

</details>

<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Cohen (1988); Döring & Bortz (2016); JASP Team (2024)
</div>

</section>

---

## Mann-Whitney-U-Test

<span style="font-size: 1.1em;"><b>Wann passt der Test?</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🎯</div>
<div style="text-align: center; font-size: 1.1em;"><b>Fragestellung</b></div>
<div style="font-size: 0.9em;">Unterscheiden sich <b>zwei Gruppen</b> in der zentralen Tendenz (Rangplätze)?</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📏</div>
<div style="text-align: center; font-size: 1.1em;"><b>Daten</b></div>
<div style="font-size: 0.9em;">Abhängige Variable <b>ordinal</b> (oder metrisch, aber nicht normalverteilt).</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">👥</div>
<div style="text-align: center; font-size: 1.1em;"><b>Stichprobe</b></div>
<div style="font-size: 0.9em;"><b>Verschiedene</b> Personen in den Gruppen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>Voraussetzungen</b></div>
<div style="font-size: 0.9em;">Unabhängige Messungen, mindestens ordinale Daten, ähnlich geformte Verteilungen.</div>
</div>

</div>

<div style="border: 2px solid #2a9a50; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
📋 <span style="background: linear-gradient(transparent 55%, rgba(66, 162, 61, 0.55) 60%);"><b>Wirkung auf das Anstrengungsempfinden</b></span> 📋<br>
Geben Personen <b>mit Musik</b> niedrigere Borg-Werte an als <b>andere</b> Personen <b>ohne Musik</b>?
</div>

<span style="font-size: 1.1em;"><b>Hypothesen</b></span>

| Hypothese | Formulierung im Musikbeispiel |
| :-- | :-- |
| **H0** | Die Verteilung der Borg-Werte ist in beiden Gruppen gleich. |
| **H1 (ungerichtet)** | Die Borg-Werte unterscheiden sich zwischen den Gruppen. |
| **H1 (gerichtet)** | Mit Musik sind die Borg-Werte niedriger. |

{{1}} <section>

<span style="font-size: 1.1em;"><b>Durchführung in JASP</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🏷️</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Variablen einstellen</b></div>
<div style="font-size: 0.9em;">Bedingung nominal, Borg-Wert ordinal.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧪</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Analyse öffnen</b></div>
<div style="font-size: 0.9em;">T-Tests ➜ Classical ➜ Independent Samples T-Test.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔗</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Variablen zuweisen</b></div>
<div style="font-size: 0.9em;">Borg-Wert in „Dependent Variables“, Bedingung in „Grouping Variable“.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">☑️</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Test wählen</b></div>
<div style="font-size: 0.9em;">Unter „Tests“ <b>Mann-Whitney</b> anhaken, Student abwählen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">➕</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Zusatzangaben</b></div>
<div style="font-size: 0.9em;">„Location parameter“ (Hodges-Lehmann) und „Effect size“ (rank-biserial) anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔍</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Gruppen vergleichen</b></div>
<div style="font-size: 0.9em;">„Descriptives“ und „Descriptives plots“ anhaken, um die Mediane zu sehen.</div>
</div>

</div>

<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> T-Tests ➜ Classical ➜ Independent Samples T-Test ➜ Tests: Mann-Whitney</div>
<div style="height: 10px;"></div>

<!-- TODO: Screenshot JASP: Mann-Whitney-U-Test -->

</section>

{{2}} <section>

<span style="font-size: 1.1em;"><b>Ergebnis lesen</b></span>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Independent Samples T-Test</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;"></th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Test</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">W</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">df</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">p</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Rank-Biserial Correlation</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Borg-Wert</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Mann-Whitney</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">66,5</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;"></td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">&lt; ,001</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">−,67</td></tr>
</table>
</div>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Descriptives</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Gruppe</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">N</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Median</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">mit Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">20</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">12</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">ohne Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">20</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">14</td></tr>
</table>
</div>

<div style="font-size: 0.8em; opacity: 0.7; margin-bottom: 10px;">Fiktive Daten, nachgebaut im Stil der JASP-Ausgabe.</div>

<ul style="font-size: 0.95em;">
<li><b><i>p</i>-Wert:</b> <i>p</i> < ,001 ➜ die Verteilungen unterscheiden sich signifikant.</li>
<li><b>W:</b> JASP nennt die Teststatistik W. Sie entspricht dem U-Wert der ersten Gruppe, bei anderer Gruppenreihenfolge kann sie abweichen (n<sub>1</sub>·n<sub>2</sub> − U).</li>
<li><b>Richtung:</b> Der Median mit Musik (12) liegt unter dem Median ohne Musik (14).</li>
<li><b>Rank-biserial:</b> −,67 ➜ mit Musik tendenziell niedrigere Werte, großer Effekt.</li>
</ul>

<span style="font-size: 1.1em;"><b>Effektstärke einordnen</b></span>

Die rank-biserial Korrelation wird wie <i>r</i> eingeordnet: ab ,1 klein, ab ,3 mittel, ab ,5 groß (Cohen, 1988). Das Vorzeichen zeigt die Richtung, die Größe die Stärke.

</section>

{{3}} <section>

<span style="font-size: 1.1em;"><b>So berichtest du das Ergebnis</b></span>

<div style="border-left: 6px solid #a74ebd; background: #f6f1fa; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
✍️ <b>Musterbericht (APA):</b><br>
<i>Personen mit Musik gaben niedrigere Borg-Werte an (Mdn = 12) als Personen ohne Musik (Mdn = 14), U = 66,5, p < ,001, r<sub>rb</sub> = −,67.</i>
</div>

<details>
<summary><b>👉 Voraussetzungen prüfen und was du bei Verletzung tust</b></summary>

| Voraussetzung | Hinweis |
| :-- | :-- |
| Skalenniveau | mindestens ordinal, der Borg-Wert erfüllt das |
| Unabhängigkeit | verschiedene Personen in den Gruppen |
| Form der Verteilungen | für die Deutung als Mediandifferenz sollten die Verteilungen ähnlich geformt sein |
| Gebundene Ränge (Ties) | viele gleiche Werte (z. B. mehrere Personen mit 13) sind bei Borg normal; JASP rechnet mit einer Korrektur |

</details>

**Frage 1:** Warum eignet sich der Mann-Whitney-U-Test für Borg-Werte?

- [( )] Weil Borg-Werte nominal sind
- [(X)] Weil er keine metrischen Daten und keine Normalverteilung voraussetzt
- [( )] Weil er für mehr als zwei Gruppen gilt
- [( )] Weil er Zusammenhänge prüft

<details>
<summary><b>👉 Erklärung</b></summary>

Der Test arbeitet mit Rangplätzen und braucht nur ordinale Daten.

</details>

<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Döring & Bortz (2016); Eid, Gollwitzer & Schmitt (2017); JASP Team (2024)
</div>

</section>

---

## t-Test für verbundene Stichproben

<span style="font-size: 1.1em;"><b>Wann passt der Test?</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🎯</div>
<div style="text-align: center; font-size: 1.1em;"><b>Fragestellung</b></div>
<div style="font-size: 0.9em;">Unterscheiden sich <b>zwei Messungen derselben Personen</b> im Mittelwert?</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📏</div>
<div style="text-align: center; font-size: 1.1em;"><b>Daten</b></div>
<div style="font-size: 0.9em;">Abhängige Variable <b>metrisch</b>, zwei Messungen pro Person.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">👥</div>
<div style="text-align: center; font-size: 1.1em;"><b>Stichprobe</b></div>
<div style="font-size: 0.9em;"><b>Dieselben</b> Personen unter beiden Bedingungen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>Voraussetzungen</b></div>
<div style="font-size: 0.9em;">Die <b>Differenzen</b> sind ungefähr normalverteilt.</div>
</div>

</div>

<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
🏃🏾‍♀️ <span style="background: linear-gradient(transparent 55%, rgba(71, 69, 173, 0.55) 60%);"><b>Wirkung auf die Ausdauerleistung</b></span> 🏃🏾‍♀️<br>
Dieselben 20 Personen laufen einmal <b>mit</b> und einmal <b>ohne</b> Musik (Reihenfolge ausgeglichen). Verglichen werden die Strecken pro Person.
</div>

<div style="font-size: 0.8em; opacity: 0.7;">Die Daten sind fiktiv. Im Datensatz stehen beide Messungen in zwei Spalten: <b>Strecke_mit</b> und <b>Strecke_ohne</b>.</div>

<span style="font-size: 1.1em;"><b>Hypothesen</b></span>

| Hypothese | Formulierung im Musikbeispiel |
| :-- | :-- |
| **H0** | Die mittlere Differenz der Strecken ist null (μ<sub>D</sub> = 0). |
| **H1 (ungerichtet)** | Die mittlere Differenz ist nicht null (μ<sub>D</sub> ≠ 0). |
| **H1 (gerichtet)** | Mit Musik ist die Strecke im Mittel größer (μ<sub>D</sub> &gt; 0). |

{{1}} <section>

<span style="font-size: 1.1em;"><b>Durchführung in JASP</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📋</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Datenformat</b></div>
<div style="font-size: 0.9em;">Beide Messungen stehen <b>in je einer Spalte</b> (Wide-Format), eine Zeile pro Person.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧪</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Analyse öffnen</b></div>
<div style="font-size: 0.9em;">T-Tests ➜ Classical ➜ Paired Samples T-Test.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔗</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Variablen zuweisen</b></div>
<div style="font-size: 0.9em;">Strecke_mit und Strecke_ohne als Paar in „Variable Pairs“.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">☑️</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Test wählen</b></div>
<div style="font-size: 0.9em;">Unter „Tests“ <b>Student</b> anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">➕</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Zusatzangaben</b></div>
<div style="font-size: 0.9em;">„Mean difference“, „Effect size“ und „Descriptives“ anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Voraussetzungen</b></div>
<div style="font-size: 0.9em;">„Assumption Checks“ ➜ Normality prüft die Differenzen.</div>
</div>

</div>

<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> T-Tests ➜ Classical ➜ Paired Samples T-Test</div>
<div style="height: 10px;"></div>

<!-- TODO: Screenshot JASP: t-Test für verbundene Stichproben -->

</section>

{{2}} <section>

<span style="font-size: 1.1em;"><b>Ergebnis lesen</b></span>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Paired Samples T-Test</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Messung 1</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Messung 2</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">t</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">df</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">p</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Mean Difference</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">SE Difference</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Cohen’s d</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Strecke_mit</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Strecke_ohne</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">9,48</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">19</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">&lt; ,001</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">115,05</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">12,13</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2,12</td></tr>
</table>
</div>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Descriptives</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Messung</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">N</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Mean</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">SD</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Strecke_mit</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">20</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2599,05</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">228,99</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Strecke_ohne</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">20</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2484,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">223,65</td></tr>
</table>
</div>

<div style="font-size: 0.8em; opacity: 0.7; margin-bottom: 10px;">Fiktive Daten, nachgebaut im Stil der JASP-Ausgabe.</div>

<ul style="font-size: 0.95em;">
<li><b><i>p</i>-Wert:</b> <i>p</i> < ,001 ➜ die Differenz ist signifikant.</li>
<li><b>Richtung:</b> Mit Musik wurde im Mittel 115,0 m weiter gelaufen.</li>
<li><b>Cohen’s d:</b> 2,12 (bei verbundenen Stichproben bezogen auf die Standardabweichung der Differenzen), ein sehr großer Effekt.</li>
<li><b>Konfidenzintervall:</b> 95 %-KI der Differenz [89,7; 140,4] m, es enthält die Null nicht.</li>
</ul>

<span style="font-size: 1.1em;"><b>Effektstärke einordnen</b></span>

Cohen’s <i>d</i> wird wie beim t-Test für unabhängige Stichproben eingeordnet (0,2 klein, 0,5 mittel, 0,8 groß). Da die Differenzen im Beispiel kaum streuen, fällt der Wert hier sehr hoch aus.

</section>

{{3}} <section>

<span style="font-size: 1.1em;"><b>So berichtest du das Ergebnis</b></span>

<div style="border-left: 6px solid #a74ebd; background: #f6f1fa; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
✍️ <b>Musterbericht (APA):</b><br>
<i>Dieselben Personen liefen mit Musik (M = 2599,05 m, SD = 228,99) weiter als ohne Musik (M = 2484,00 m, SD = 223,65), t(19) = 9,48, p < ,001, d = 2,12.</i>
</div>

<details>
<summary><b>👉 Voraussetzungen prüfen und was du bei Verletzung tust</b></summary>

| Voraussetzung | Prüfung in JASP | Ergebnis im Beispiel | Bei Verletzung |
| :-- | :-- | :-- | :-- |
| Differenzen normalverteilt | Shapiro-Wilk, Q-Q-Plot der Differenzen | <i>p</i> = ,790 ➜ erfüllt | Wilcoxon-Test |
| Abhängige Paare | Studiendesign | dieselben Personen ➜ erfüllt | anderer Test (unabhängig) |

</details>

**Frage 1:** Worauf bezieht sich die Normalverteilungsannahme beim t-Test für verbundene Stichproben?

- [( )] Auf beide Messungen einzeln
- [(X)] Auf die Differenzen der Messpaare
- [( )] Auf die Gruppenvariable
- [( )] Auf die Anzahl der Personen

<details>
<summary><b>👉 Erklärung</b></summary>

Beim verbundenen t-Test werden die Differenzen pro Person analysiert.

</details>

<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Cohen (1988); Döring &a Bortz (2016); JASP Team (2024)
</div>

</section>

---

## Wilcoxon-Test

<span style="font-size: 1.1em;"><b>Wann passt der Test?</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🎯</div>
<div style="text-align: center; font-size: 1.1em;"><b>Fragestellung</b></div>
<div style="font-size: 0.9em;">Unterscheiden sich <b>zwei Messungen derselben Personen</b> (Rangplätze der Differenzen)?</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📏</div>
<div style="text-align: center; font-size: 1.1em;"><b>Daten</b></div>
<div style="font-size: 0.9em;">Abhängige Variable <b>ordinal</b> (oder metrisch, aber nicht normalverteilt).</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">👥</div>
<div style="text-align: center; font-size: 1.1em;"><b>Stichprobe</b></div>
<div style="font-size: 0.9em;"><b>Dieselben</b> Personen unter beiden Bedingungen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>Voraussetzungen</b></div>
<div style="font-size: 0.9em;">Mindestens ordinale Daten, Differenzen symmetrisch verteilt.</div>
</div>

</div>

<div style="border: 2px solid #2a9a50; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
📋 <span style="background: linear-gradient(transparent 55%, rgba(66, 162, 61, 0.55) 60%);"><b>Wirkung auf das Anstrengungsempfinden</b></span> 📋<br>
Dieselben 20 Personen geben nach dem Lauf <b>mit</b> und <b>ohne</b> Musik ihren Borg-Wert an. Verglichen werden die Werte pro Person.
</div>

<span style="font-size: 1.1em;"><b>Hypothesen</b></span>

| Hypothese | Formulierung im Musikbeispiel |
| :-- | :-- |
| **H0** | Es gibt keinen Unterschied zwischen den Borg-Werten mit und ohne Musik. |
| **H1 (ungerichtet)** | Die Borg-Werte unterscheiden sich. |
| **H1 (gerichtet)** | Mit Musik sind die Borg-Werte niedriger. |

{{1}} <section>

<span style="font-size: 1.1em;"><b>Durchführung in JASP</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📋</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Datenformat</b></div>
<div style="font-size: 0.9em;">Borg_mit und Borg_ohne in zwei Spalten, eine Zeile pro Person.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧪</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Analyse öffnen</b></div>
<div style="font-size: 0.9em;">T-Tests ➜ Classical ➜ Paired Samples T-Test.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔗</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Variablen zuweisen</b></div>
<div style="font-size: 0.9em;">Borg_mit und Borg_ohne als Paar in „Variable Pairs“.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">☑️</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Test wählen</b></div>
<div style="font-size: 0.9em;">Unter „Tests“ <b>Wilcoxon signed-rank</b> anhaken, Student abwählen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">➕</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Zusatzangaben</b></div>
<div style="font-size: 0.9em;">„Effect size“ (rank-biserial) und „Descriptives“ anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔍</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Bindungen beachten</b></div>
<div style="font-size: 0.9em;">Personen mit gleichem Wert in beiden Bedingungen (Differenz 0) gehen nicht in den Test ein.</div>
</div>

</div>

<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> T-Tests ➜ Classical ➜ Paired Samples T-Test ➜ Tests: Wilcoxon signed-rank</div>
<div style="height: 10px;"></div>

<!-- TODO: Screenshot JASP: Wilcoxon-Test -->

</section>

{{2}} <section>

<span style="font-size: 1.1em;"><b>Ergebnis lesen</b></span>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Paired Samples T-Test</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Messung 1</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Messung 2</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Test</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">W</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">z</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">p</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Rank-Biserial Correlation</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Borg_mit</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Borg_ohne</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Wilcoxon</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">20,0</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">−3,02</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,002</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">−,79</td></tr>
</table>
</div>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Descriptives</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Messung</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">N</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Median</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Borg_mit</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">20</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">12</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Borg_ohne</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">20</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">14</td></tr>
</table>
</div>

<div style="font-size: 0.8em; opacity: 0.7; margin-bottom: 10px;">Fiktive Daten, nachgebaut im Stil der JASP-Ausgabe.</div>

<ul style="font-size: 0.95em;">
<li><b><i>p</i>-Wert:</b> <i>p</i> = ,002 ➜ signifikant.</li>
<li><b>W:</b> 20,0 ist die Summe der Ränge der positiven Differenzen. Hier gibt es nur wenige positive Differenzen, also sinken die Werte mit Musik bei den meisten Personen.</li>
<li><b>Richtung:</b> Median mit Musik 12, ohne Musik 14.</li>
<li><b>Rank-biserial:</b> −,79 ➜ großer Effekt, bei den meisten Personen sind die Werte mit Musik niedriger.</li>
<li><b>Bindung:</b> 1 Person mit Differenz 0 ging nicht in den Test ein, ausgewertet wurden 19 Paare.</li>
</ul>

<span style="font-size: 1.1em;"><b>Effektstärke einordnen</b></span>

Wie beim Mann-Whitney-Test: rank-biserial Korrelation ab ,1 klein, ab ,3 mittel, ab ,5 groß.

</section>

{{3}} <section>

<span style="font-size: 1.1em;"><b>So berichtest du das Ergebnis</b></span>

<div style="border-left: 6px solid #a74ebd; background: #f6f1fa; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
✍️ <b>Musterbericht (APA):</b><br>
<i>Mit Musik fiel das Anstrengungsempfinden niedriger aus (Mdn = 12) als ohne Musik (Mdn = 14), W = 20,0, z = −3,02, p = ,002, r<sub>rb</sub> = −,79.</i>
</div>

<details>
<summary><b>👉 Voraussetzungen prüfen und was du bei Verletzung tust</b></summary>

| Voraussetzung | Hinweis |
| :-- | :-- |
| Skalenniveau | mindestens ordinal |
| Abhängige Paare | dieselben Personen in beiden Bedingungen |
| Symmetrie der Differenzen | die Verteilung der Differenzen sollte ungefähr symmetrisch sein |
| Differenz 0 | Paare mit gleichem Wert werden ausgeschlossen |

</details>

**Frage 1:** Welcher parametrische Test ist die Entsprechung zum Wilcoxon-Test?

- [( )] t-Test für unabhängige Stichproben
- [(X)] t-Test für verbundene Stichproben
- [( )] ANOVA
- [( )] Pearson-Korrelation

<details>
<summary><b>👉 Erklärung</b></summary>

Beide Tests vergleichen zwei Messungen derselben Personen.

</details>

<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Döring & Bortz (2016); Eid, Gollwitzer &a Schmitt (2017); JASP Team (2024)
</div>

</section>

---

## ANOVA (einfaktoriell)

<span style="font-size: 1.1em;"><b>Wann passt der Test?</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🎯</div>
<div style="text-align: center; font-size: 1.1em;"><b>Fragestellung</b></div>
<div style="font-size: 0.9em;">Unterscheiden sich <b>mehr als zwei Gruppen</b> im Mittelwert?</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📏</div>
<div style="text-align: center; font-size: 1.1em;"><b>Daten</b></div>
<div style="font-size: 0.9em;">Abhängige Variable <b>metrisch</b>, Gruppenvariable nominal mit 3 oder mehr Stufen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">👥</div>
<div style="text-align: center; font-size: 1.1em;"><b>Stichprobe</b></div>
<div style="font-size: 0.9em;"><b>Verschiedene</b> Personen in den Gruppen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>Voraussetzungen</b></div>
<div style="font-size: 0.9em;">Normalverteilung in jeder Gruppe, gleiche Streuung, unabhängige Messungen.</div>
</div>

</div>

<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
🏃🏾‍♀️ <span style="background: linear-gradient(transparent 55%, rgba(71, 69, 173, 0.55) 60%);"><b>Wirkung auf die Ausdauerleistung</b></span> 🏃🏾‍♀️<br>
Drei Gruppen mit je 15 verschiedenen Personen laufen <b>ohne Musik</b>, mit <b>langsamer Musik</b> oder mit <b>schneller Musik</b>. Verglichen werden die mittleren Strecken.
</div>

<span style="font-size: 1.1em;"><b>Hypothesen</b></span>

| Hypothese | Formulierung im Musikbeispiel |
| :-- | :-- |
| **H0** | Alle drei Gruppen haben dieselbe mittlere Strecke (μ<sub>ohne</sub> = μ<sub>langsam</sub> = μ<sub>schnell</sub>). |
| **H1 (ungerichtet)** | Mindestens zwei Gruppen unterscheiden sich in der mittleren Strecke. |

{{1}} <section>

<span style="font-size: 1.1em;"><b>Durchführung in JASP</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🏷️</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Variablen einstellen</b></div>
<div style="font-size: 0.9em;">Musikbedingung nominal, Strecke scale.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧪</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Analyse öffnen</b></div>
<div style="font-size: 0.9em;">ANOVA ➜ Classical ➜ ANOVA.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔗</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Variablen zuweisen</b></div>
<div style="font-size: 0.9em;">Strecke in „Dependent Variable“, Musikbedingung in „Fixed Factors“.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">➕</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Effektstärke</b></div>
<div style="font-size: 0.9em;">Unter „Display“ „Effect size“ (η²) anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔍</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Post-hoc-Tests</b></div>
<div style="font-size: 0.9em;">Unter „Post Hoc Tests“ den Faktor ins rechte Feld ziehen, „Tukey“ anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Voraussetzungen</b></div>
<div style="font-size: 0.9em;">„Assumption Checks“ ➜ Homogeneity tests und Q-Q plot anhaken.</div>
</div>

</div>

<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> ANOVA ➜ Classical ➜ ANOVA</div>
<div style="height: 10px;"></div>

<!-- TODO: Screenshot JASP: ANOVA (einfaktoriell) -->

</section>

{{2}} <section>

<span style="font-size: 1.1em;"><b>Ergebnis lesen</b></span>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">ANOVA – Strecke</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Cases</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Sum of Squares</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">df</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Mean Square</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">F</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">p</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">η²</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Musikbedingung</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">645447</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">322723</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">16,92</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">&lt; ,001</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,45</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Residuals</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">801191</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">42</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">19076</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;"></td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;"></td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;"></td></tr>
</table>
</div>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Post Hoc Tests – Tukey</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Vergleich</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Mean Difference</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">p<sub>tukey</sub></th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">ohne – langsam</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">−136,6</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,026</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">ohne – schnell</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">−293,1</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">&lt; ,001</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">langsam – schnell</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">−156,5</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,009</td></tr>
</table>
</div>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Descriptives</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Gruppe</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">N</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Mean</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">SD</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">ohne Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">15</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2399,53</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">156,38</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">langsame Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">15</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2536,13</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">107,91</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">schnelle Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">15</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2692,67</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">145,36</td></tr>
</table>
</div>

<div style="font-size: 0.8em; opacity: 0.7; margin-bottom: 10px;">Fiktive Daten, nachgebaut im Stil der JASP-Ausgabe.</div>

<ul style="font-size: 0.95em;">
<li><b>Omnibustest:</b> F(2, 42) = 16,92, <i>p</i> < ,001. Mindestens zwei Gruppen unterscheiden sich, aber noch nicht, <i>welche</i>.</li>
<li><b>Post-hoc-Tests:</b> Erst dann schaust du in die Tukey-Tabelle. Hier unterscheiden sich alle drei Paare signifikant (kleinstes <i>p</i> = ,026).</li>
<li><b>η²:</b> ,45 ➜ rund 45 % der Streuung der Strecken lassen sich durch die Musikbedingung erklären (großer Effekt).</li>
<li><b>Warum nicht mehrere t-Tests?</b> Jeder zusätzliche Test erhöht das Risiko, einen Unterschied fälschlich als signifikant zu werten (α-Fehler-Kumulierung). Die ANOVA prüft alle Gruppen gemeinsam.</li>
</ul>

<span style="font-size: 1.1em;"><b>Effektstärke einordnen</b></span>

η²: ab ,01 klein, ab ,06 mittel, ab ,14 groß (Cohen, 1988).

</section>

{{3}} <section>

<span style="font-size: 1.1em;"><b>So berichtest du das Ergebnis</b></span>

<div style="border-left: 6px solid #a74ebd; background: #f6f1fa; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
✍️ <b>Musterbericht (APA):</b><br>
<i>Die Strecke unterschied sich zwischen den drei Bedingungen, F(2, 42) = 16,92, p < ,001, η² = ,45. Tukey-Post-hoc-Tests zeigten, dass mit schneller Musik (M = 2692,67 m, SD = 145,36) weiter gelaufen wurde als mit langsamer Musik (M = 2536,13 m, SD = 107,91; p = ,009) und ohne Musik (M = 2399,53 m, SD = 156,38; p < ,001).</i>
</div>

<details>
<summary><b>👉 Voraussetzungen prüfen und was du bei Verletzung tust</b></summary>

| Voraussetzung | Prüfung in JASP | Ergebnis im Beispiel | Bei Verletzung |
| :-- | :-- | :-- | :-- |
| Normalverteilung | Q-Q-Plot der Residuen, Shapiro-Wilk je Gruppe | <i>p</i> = ,231; ,818; ,188 ➜ erfüllt | Kruskal-Wallis-Test |
| Gleiche Streuung | Levene-Test | <i>p</i> = ,448 ➜ erfüllt | Welch-Korrektur („Homogeneity corrections“) |
| Unabhängigkeit | Studiendesign | verschiedene Personen ➜ erfüllt | ANOVA mit Messwiederholung |

</details>

**Frage 1:** Die ANOVA ist signifikant (p < ,001). Was sagt dir das?

- [( )] Alle Gruppen unterscheiden sich voneinander
- [(X)] Mindestens zwei Gruppen unterscheiden sich
- [( )] Es gibt keinen Unterschied
- [( )] Die Daten sind normalverteilt

<details>
<summary><b>👉 Erklärung</b></summary>

Die ANOVA zeigt nur, dass es irgendeinen Unterschied gibt. Welche Gruppen sich unterscheiden, zeigen die Post-hoc-Tests.

</details>

<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Cohen (1988); Döring & Bortz (2016); Eid, Gollwitzer & Schmitt (2017); JASP Team (2024)
</div>

</section>

---

## Kruskal-Wallis-Test

<span style="font-size: 1.1em;"><b>Wann passt der Test?</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🎯</div>
<div style="text-align: center; font-size: 1.1em;"><b>Fragestellung</b></div>
<div style="font-size: 0.9em;">Unterscheiden sich <b>mehr als zwei Gruppen</b> in der zentralen Tendenz?</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📏</div>
<div style="text-align: center; font-size: 1.1em;"><b>Daten</b></div>
<div style="font-size: 0.9em;">Abhängige Variable <b>ordinal</b> (oder metrisch, aber nicht normalverteilt).</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">👥</div>
<div style="text-align: center; font-size: 1.1em;"><b>Stichprobe</b></div>
<div style="font-size: 0.9em;"><b>Verschiedene</b> Personen in den Gruppen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>Voraussetzungen</b></div>
<div style="font-size: 0.9em;">Unabhängige Messungen, mindestens ordinale Daten, ähnlich geformte Verteilungen.</div>
</div>

</div>

<div style="border: 2px solid #2a9a50; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
📋 <span style="background: linear-gradient(transparent 55%, rgba(66, 162, 61, 0.55) 60%);"><b>Wirkung auf das Anstrengungsempfinden</b></span> 📋<br>
Drei Gruppen mit je 15 verschiedenen Personen laufen <b>ohne Musik</b>, mit <b>langsamer</b> oder mit <b>schneller Musik</b>. Verglichen werden die Borg-Werte.
</div>

<span style="font-size: 1.1em;"><b>Hypothesen</b></span>

| Hypothese | Formulierung im Musikbeispiel |
| :-- | :-- |
| **H0** | Die Verteilung der Borg-Werte ist in allen drei Gruppen gleich. |
| **H1 (ungerichtet)** | Mindestens eine Gruppe unterscheidet sich in der Verteilung der Borg-Werte. |

{{1}} <section>

<span style="font-size: 1.1em;"><b>Durchführung in JASP</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🏷️</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Variablen einstellen</b></div>
<div style="font-size: 0.9em;">Musikbedingung nominal, Borg-Wert ordinal.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧪</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Analyse öffnen</b></div>
<div style="font-size: 0.9em;">ANOVA ➜ Classical ➜ ANOVA.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔗</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Variablen zuweisen</b></div>
<div style="font-size: 0.9em;">Borg-Wert in „Dependent Variable“, Musikbedingung in „Fixed Factors“.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">☑️</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Kruskal-Wallis</b></div>
<div style="font-size: 0.9em;">Den Bereich „Nonparametrics“ öffnen, den Faktor ins rechte Feld ziehen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔍</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Post-hoc-Tests</b></div>
<div style="font-size: 0.9em;">In „Nonparametrics“ „Dunn’s post hoc test“ anhaken (mit Bonferroni-Korrektur).</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📊</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Kennwerte</b></div>
<div style="font-size: 0.9em;">„Descriptives“ anhaken, um Mediane je Gruppe zu sehen.</div>
</div>

</div>

<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> ANOVA ➜ Classical ➜ ANOVA ➜ Nonparametrics (Kruskal-Wallis)</div>
<div style="height: 10px;"></div>

<!-- TODO: Screenshot JASP: Kruskal-Wallis-Test -->

</section>

{{2}} <section>

<span style="font-size: 1.1em;"><b>Ergebnis lesen</b></span>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Kruskal-Wallis Test</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Faktor</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Statistic</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">df</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">p</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Musikbedingung</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">22,68</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">&lt; ,001</td></tr>
</table>
</div>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Dunn’s Post Hoc Test</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Vergleich</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">z</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">p<sub>bonf</sub></th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">ohne – langsam</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">3,85</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">&lt; ,001</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">ohne – schnell</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">4,35</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">&lt; ,001</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">langsam – schnell</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">0,51</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">1,000</td></tr>
</table>
</div>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Descriptives</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Gruppe</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">N</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Median</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">ohne Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">15</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">14</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">langsame Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">15</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">12</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">schnelle Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">15</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">12</td></tr>
</table>
</div>

<div style="font-size: 0.8em; opacity: 0.7; margin-bottom: 10px;">Fiktive Daten, nachgebaut im Stil der JASP-Ausgabe.</div>

<ul style="font-size: 0.95em;">
<li><b>Omnibustest:</b> H(2) = 22,68, <i>p</i> < ,001 ➜ mindestens eine Gruppe unterscheidet sich.</li>
<li><b>Post-hoc-Tests:</b> Ohne Musik gegen langsame und gegen schnelle Musik ist signifikant, langsame gegen schnelle Musik nicht (p<sub>bonf</sub> = 1,000).</li>
<li><b>Effektstärke ε²:</b> ,52 ➜ großer Effekt (JASP gibt sie nicht direkt aus, du berechnest ε² = H·(N+1) / (N²−1) von Hand).</li>
<li><b>Hinweis:</b> Die Post-hoc-Tests nutzen eine Korrektur für mehrfaches Testen (Bonferroni), deshalb steht p<sub>bonf</sub> in der Tabelle.</li>
</ul>

<span style="font-size: 1.1em;"><b>Effektstärke einordnen</b></span>

ε²: ab ,01 klein, ab ,08 mittel, ab ,26 groß (Tomczak & Tomczak, 2014). Die Faustwerte sind weniger einheitlich als bei d oder η², berichte deshalb immer auch die Mediane.

</section>

{{3}} <section>

<span style="font-size: 1.1em;"><b>So berichtest du das Ergebnis</b></span>

<div style="border-left: 6px solid #a74ebd; background: #f6f1fa; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
✍️ <b>Musterbericht (APA):</b><br>
<i>Der Borg-Wert unterschied sich zwischen den Bedingungen, H(2) = 22,68, p < ,001, ε² = ,52. Dunn-Post-hoc-Tests (Bonferroni-korrigiert) zeigten niedrigere Werte mit langsamer (Mdn = 12) und schneller Musik (Mdn = 12) als ohne Musik (Mdn = 14); langsame und schnelle Musik unterschieden sich nicht (p = 1,000).</i>
</div>

<details>
<summary><b>👉 Voraussetzungen prüfen und was du bei Verletzung tust</b></summary>

| Voraussetzung | Hinweis |
| :-- | :-- |
| Skalenniveau | mindestens ordinal |
| Unabhängigkeit | verschiedene Personen in den Gruppen |
| Verteilungsform | für die Deutung als Medianvergleich sollten die Verteilungen ähnlich geformt sein |
| Gruppengröße | kleine Gruppen (unter 5) liefern unsichere Ergebnisse |

</details>

**Frage 1:** Wofür brauchst du nach einem signifikanten Kruskal-Wallis-Test Post-hoc-Tests?

- [( )] Um die Normalverteilung zu prüfen
- [(X)] Um herauszufinden, welche Gruppen sich unterscheiden
- [( )] Um die Effektstärke zu berechnen
- [( )] Um Ausreißer zu entfernen

<details>
<summary><b>👉 Erklärung</b></summary>

Der Omnibustest zeigt nur, dass sich irgendeine Gruppe unterscheidet. Die Paarvergleiche zeigen, welche.

</details>

<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Döring & Bortz (2016); Eid, Gollwitzer & Schmitt (2017); Tomczak & Tomczak (2014); JASP Team (2024)
</div>

</section>

---

## ANOVA mit Messwiederholung

<span style="font-size: 1.1em;"><b>Wann passt der Test?</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🎯</div>
<div style="text-align: center; font-size: 1.1em;"><b>Fragestellung</b></div>
<div style="font-size: 0.9em;">Unterscheiden sich <b>mehr als zwei Messungen derselben Personen</b> im Mittelwert?</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📏</div>
<div style="text-align: center; font-size: 1.1em;"><b>Daten</b></div>
<div style="font-size: 0.9em;">Abhängige Variable <b>metrisch</b>, mindestens drei Messungen pro Person.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">👥</div>
<div style="text-align: center; font-size: 1.1em;"><b>Stichprobe</b></div>
<div style="font-size: 0.9em;"><b>Dieselben</b> Personen unter allen Bedingungen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>Voraussetzungen</b></div>
<div style="font-size: 0.9em;">Normalverteilung, Sphärizität (gleiche Varianz der Differenzen).</div>
</div>

</div>

<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
🏃🏾‍♀️ <span style="background: linear-gradient(transparent 55%, rgba(71, 69, 173, 0.55) 60%);"><b>Wirkung auf die Ausdauerleistung</b></span> 🏃🏾‍♀️<br>
Dieselben 15 Personen laufen <b>ohne Musik</b>, mit <b>langsamer</b> und mit <b>schneller Musik</b> (Reihenfolge ausgeglichen). Verglichen werden die Strecken.
</div>

<span style="font-size: 1.1em;"><b>Hypothesen</b></span>

| Hypothese | Formulierung im Musikbeispiel |
| :-- | :-- |
| **H0** | Die mittlere Strecke ist unter allen drei Bedingungen gleich. |
| **H1 (ungerichtet)** | Mindestens zwei Bedingungen unterscheiden sich in der mittleren Strecke. |

{{1}} <section>

<span style="font-size: 1.1em;"><b>Durchführung in JASP</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📋</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Datenformat</b></div>
<div style="font-size: 0.9em;">Drei Spalten: Strecke_ohne, Strecke_langsam, Strecke_schnell. Eine Zeile pro Person.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧪</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Analyse öffnen</b></div>
<div style="font-size: 0.9em;">ANOVA ➜ Classical ➜ Repeated Measures ANOVA.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔗</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Faktor anlegen</b></div>
<div style="font-size: 0.9em;">Faktor „Musik“ mit den Stufen ohne, langsam, schnell definieren und die Spalten den Stufen zuordnen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">➕</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Effektstärke</b></div>
<div style="font-size: 0.9em;">„Effect size“ (η²p) anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔍</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Post-hoc-Tests</b></div>
<div style="font-size: 0.9em;">„Post Hoc Tests“ ➜ Faktor „Musik“ ➜ Bonferroni anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Sphärizität</b></div>
<div style="font-size: 0.9em;">„Assumption Checks“ ➜ Sphericity tests anhaken, bei Verletzung Greenhouse-Geisser wählen.</div>
</div>

</div>

<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> ANOVA ➜ Classical ➜ Repeated Measures ANOVA</div>
<div style="height: 10px;"></div>

<!-- TODO: Screenshot JASP: ANOVA mit Messwiederholung -->

</section>

{{2}} <section>

<span style="font-size: 1.1em;"><b>Ergebnis lesen</b></span>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Test of Sphericity</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;"></th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Mauchly’s W</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">p</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Greenhouse-Geisser ε</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">0,67</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,073</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">0,75</td></tr>
</table>
</div>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Within Subjects Effects</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Cases</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Sphericity Correction</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">df</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">F</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">p</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">η²p</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">None</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2; 28</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">51,66</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">&lt; ,001</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,79</td></tr>
</table>
</div>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Post Hoc Tests – Bonferroni</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Vergleich</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">t</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">p<sub>bonf</sub></th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">ohne – langsam</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">−8,40</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">&lt; ,001</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">ohne – schnell</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">−8,11</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">&lt; ,001</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">langsam – schnell</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">−4,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,004</td></tr>
</table>
</div>

<div style="font-size: 0.8em; opacity: 0.7; margin-bottom: 10px;">Fiktive Daten, nachgebaut im Stil der JASP-Ausgabe.</div>

<ul style="font-size: 0.95em;">
<li><b>Sphärizität zuerst:</b> Mauchly-Test <i>p</i> = ,073 ➜ nicht signifikant, die Annahme gilt (Zeile „None“ lesen). Wäre er signifikant, nimmst du die Zeile „Greenhouse-Geisser“.</li>
<li><b>Haupteffekt:</b> F(2, 28) = 51,66, <i>p</i> < ,001 ➜ mindestens zwei Bedingungen unterscheiden sich.</li>
<li><b>Post-hoc-Tests:</b> Alle drei Paarvergleiche sind nach Bonferroni-Korrektur signifikant.</li>
<li><b>η²p:</b> ,79 ➜ großer Effekt.</li>
</ul>

<span style="font-size: 1.1em;"><b>Effektstärke einordnen</b></span>

η²p: ab ,01 klein, ab ,06 mittel, ab ,14 groß (Cohen, 1988).

</section>

{{3}} <section>

<span style="font-size: 1.1em;"><b>So berichtest du das Ergebnis</b></span>

<div style="border-left: 6px solid #a74ebd; background: #f6f1fa; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
✍️ <b>Musterbericht (APA):</b><br>
<i>Die Strecke unterschied sich zwischen den Bedingungen, F(2, 28) = 51,66, p < ,001, η²p = ,79. Bonferroni-korrigierte Vergleiche zeigten, dass die Strecke ohne Musik (M = 2447,93 m, SD = 151,50) kürzer war als mit langsamer (M = 2557,07 m, SD = 145,98) und mit schneller Musik (M = 2623,27 m, SD = 118,95); auch langsame und schnelle Musik unterschieden sich (p = ,004).</i>
</div>

<details>
<summary><b>👉 Voraussetzungen prüfen und was du bei Verletzung tust</b></summary>

| Voraussetzung | Prüfung in JASP | Ergebnis im Beispiel | Bei Verletzung |
| :-- | :-- | :-- | :-- |
| Sphärizität | Mauchly-Test | <i>p</i> = ,073 ➜ erfüllt | Greenhouse-Geisser-Korrektur |
| Normalverteilung | Q-Q-Plot | annähernd erfüllt | Friedman-Test |
| Abhängige Messungen | Studiendesign | dieselben Personen ➜ erfüllt | ANOVA (unabhängig) |

</details>

**Frage 1:** Der Mauchly-Test ist signifikant (p = ,01). Was tust du?

- [( )] Nichts, die Annahme gilt
- [(X)] Die Greenhouse-Geisser-Korrektur verwenden
- [( )] Einen t-Test für unabhängige Stichproben rechnen
- [( )] Die Messwiederholung ignorieren

<details>
<summary><b>👉 Erklärung</b></summary>

Ein signifikanter Mauchly-Test bedeutet, dass die Sphärizität verletzt ist. Die Korrektur passt die Freiheitsgrade an.

</details>

<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Cohen (1988); Döring & Bortz (2016); Eid, Gollwitzer & Schmitt (2017); JASP Team (2024)
</div>

</section>

---

## Friedman-Test

<span style="font-size: 1.1em;"><b>Wann passt der Test?</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🎯</div>
<div style="text-align: center; font-size: 1.1em;"><b>Fragestellung</b></div>
<div style="font-size: 0.9em;">Unterscheiden sich <b>mehr als zwei Messungen derselben Personen</b> in der zentralen Tendenz?</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📏</div>
<div style="text-align: center; font-size: 1.1em;"><b>Daten</b></div>
<div style="font-size: 0.9em;">Abhängige Variable <b>ordinal</b> (oder metrisch, aber nicht normalverteilt).</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">👥</div>
<div style="text-align: center; font-size: 1.1em;"><b>Stichprobe</b></div>
<div style="font-size: 0.9em;"><b>Dieselben</b> Personen unter allen Bedingungen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>Voraussetzungen</b></div>
<div style="font-size: 0.9em;">Mindestens ordinale Daten, abhängige Messungen.</div>
</div>

</div>

<div style="border: 2px solid #2a9a50; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
📋 <span style="background: linear-gradient(transparent 55%, rgba(66, 162, 61, 0.55) 60%);"><b>Wirkung auf das Anstrengungsempfinden</b></span> 📋<br>
Dieselben 15 Personen geben nach dem Lauf <b>ohne Musik</b>, mit <b>langsamer</b> und mit <b>schneller Musik</b> ihren Borg-Wert an.
</div>

<span style="font-size: 1.1em;"><b>Hypothesen</b></span>

| Hypothese | Formulierung im Musikbeispiel |
| :-- | :-- |
| **H0** | Die Borg-Werte unterscheiden sich unter den drei Bedingungen nicht. |
| **H1 (ungerichtet)** | Mindestens eine Bedingung unterscheidet sich. |

{{1}} <section>

<span style="font-size: 1.1em;"><b>Durchführung in JASP</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📋</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Datenformat</b></div>
<div style="font-size: 0.9em;">Drei Spalten: Borg_ohne, Borg_langsam, Borg_schnell, eine Zeile pro Person.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧪</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Analyse öffnen</b></div>
<div style="font-size: 0.9em;">ANOVA ➜ Classical ➜ Repeated Measures ANOVA.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔗</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Faktor anlegen</b></div>
<div style="font-size: 0.9em;">Faktor „Musik“ mit drei Stufen definieren, Spalten zuordnen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">☑️</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Friedman</b></div>
<div style="font-size: 0.9em;">Den Bereich „Nonparametrics“ öffnen, den Faktor ins rechte Feld ziehen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔍</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Post-hoc-Tests</b></div>
<div style="font-size: 0.9em;">„Conover’s post hoc tests“ anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📊</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Kennwerte</b></div>
<div style="font-size: 0.9em;">„Descriptives“ anhaken, um Mediane zu sehen.</div>
</div>

</div>

<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> ANOVA ➜ Classical ➜ Repeated Measures ANOVA ➜ Nonparametrics (Friedman)</div>
<div style="height: 10px;"></div>

<!-- TODO: Screenshot JASP: Friedman-Test -->

</section>

{{2}} <section>

<span style="font-size: 1.1em;"><b>Ergebnis lesen</b></span>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Friedman Test</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Faktor</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">χ²</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">df</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">p</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Kendall’s W</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">13,78</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,001</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,46</td></tr>
</table>
</div>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Descriptives</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Bedingung</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">N</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Median</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Mean Rank</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">ohne Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">15</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">14</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2,73</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">langsame Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">15</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">13</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">1,73</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">schnelle Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">15</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">12</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">1,53</td></tr>
</table>
</div>

<div style="font-size: 0.8em; opacity: 0.7; margin-bottom: 10px;">Fiktive Daten, nachgebaut im Stil der JASP-Ausgabe.</div>

<ul style="font-size: 0.95em;">
<li><b>Teststatistik:</b> χ²(2) = 13,78, <i>p</i> = ,001 ➜ mindestens eine Bedingung unterscheidet sich.</li>
<li><b>Mittlere Ränge:</b> ohne Musik 2,73, langsam 1,73, schnell 1,53 ➜ je schneller die Musik, desto niedriger die Borg-Werte.</li>
<li><b>Kendall’s W:</b> ,46 ➜ starke Übereinstimmung der Rangfolge über die Personen hinweg (großer Effekt).</li>
<li><b>Post-hoc-Tests:</b> Die Paarvergleiche (Conover) liest du wie beim Kruskal-Wallis-Test: signifikant, wenn p<sub>bonf</sub> &lt; ,05.</li>
</ul>

<span style="font-size: 1.1em;"><b>Effektstärke einordnen</b></span>

Kendall’s W: ab ,1 klein, ab ,3 mittel, ab ,5 groß (Cohen, 1988). W = ,46 liegt an der Grenze zwischen mittel und groß.

</section>

{{3}} <section>

<span style="font-size: 1.1em;"><b>So berichtest du das Ergebnis</b></span>

<div style="border-left: 6px solid #a74ebd; background: #f6f1fa; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
✍️ <b>Musterbericht (APA):</b><br>
<i>Der Borg-Wert unterschied sich zwischen den drei Bedingungen, χ²(2) = 13,78, p = ,001, W = ,46. Die Mediane lagen ohne Musik bei 14, mit langsamer Musik bei 13 und mit schneller Musik bei 12.</i>
</div>

<details>
<summary><b>👉 Voraussetzungen prüfen und was du bei Verletzung tust</b></summary>

| Voraussetzung | Hinweis |
| :-- | :-- |
| Skalenniveau | mindestens ordinal |
| Abhängige Messungen | dieselben Personen unter allen Bedingungen |
| Vollständige Daten | Personen mit fehlenden Werten werden ausgeschlossen |
| Gebundene Ränge | gleiche Werte innerhalb einer Person werden mit mittleren Rängen berücksichtigt |

</details>

**Frage 1:** Welcher Test ist die nichtparametrische Alternative zur ANOVA mit Messwiederholung?

- [( )] Kruskal-Wallis-Test
- [(X)] Friedman-Test
- [( )] Mann-Whitney-U-Test
- [( )] Chi-Quadrat-Test

<details>
<summary><b>👉 Erklärung</b></summary>

Der Friedman-Test arbeitet mit Rängen innerhalb jeder Person und eignet sich für mehr als zwei Messungen.

</details>

<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Cohen (1988); Döring & Bortz (2016); JASP Team (2024)
</div>

</section>

---

## Check-Up: Unterschiede testen

<!-- class="animate__animated animate__fadeIn" -->
<div style="border-left: 6px solid #a74ebd; background: rgba(185, 145, 215, 0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
<span style="font-size: 1.3em;"><i>Welcher Test passt zu welcher Situation? Teste dein Wissen.</i></span>
</div>

<div style="height: 15px;"></div>

Beantworte die Fragen. Nach dem Beantworten bekommst du eine kurze Erklärung.

**Frage 1:** 40 verschiedene Personen laufen 12 Minuten, 20 mit und 20 ohne Musik. Du vergleichst die Strecken (metrisch, annähernd normalverteilt). Welcher Test passt?

- [(X)] t-Test für unabhängige Stichproben
- [( )] t-Test für verbundene Stichproben
- [( )] Chi-Quadrat-Test
- [( )] Friedman-Test

[[?]] Verschiedene Personen bedeutet unabhängige Stichproben.

<details>
<summary><b>👉 Erklärung</b></summary>

Zwei Gruppen aus verschiedenen Personen mit metrischer Messung ➜ t-Test für unabhängige Stichproben.

</details>

**Frage 2:** Dieselben 20 Personen laufen einmal mit und einmal ohne Musik. Du vergleichst die Borg-Werte (ordinal). Welcher Test passt?

- [( )] Mann-Whitney-U-Test
- [(X)] Wilcoxon-Test
- [( )] ANOVA
- [( )] Pearson-Korrelation

[[?]] Dieselben Personen und ordinale Daten.

<details>
<summary><b>👉 Erklärung</b></summary>

Zwei abhängige Messungen mit ordinalen Daten ➜ Wilcoxon-Test.

</details>

**Frage 3:** Du vergleichst die Strecke bei drei Bedingungen mit drei verschiedenen Gruppen. Die Voraussetzungen sind erfüllt. Welcher Test passt?

- [( )] t-Test für unabhängige Stichproben
- [(X)] ANOVA
- [( )] Friedman-Test
- [( )] Wilcoxon-Test

<details>
<summary><b>👉 Erklärung</b></summary>

Mehr als zwei unabhängige Gruppen mit metrischen Daten ➜ ANOVA.

</details>

**Frage 4:** Dieselben Personen geben ihren Borg-Wert unter drei Bedingungen an. Welcher Test passt?

- [( )] Kruskal-Wallis-Test
- [(X)] Friedman-Test
- [( )] Mann-Whitney-U-Test
- [( )] t-Test für unabhängige Stichproben

<details>
<summary><b>👉 Erklärung</b></summary>

Mehr als zwei abhängige Messungen mit ordinalen Daten ➜ Friedman-Test.

</details>

**Frage 5:** Ein signifikanter ANOVA-Test sagt dir, dass …

- [( )] alle Gruppen sich unterscheiden
- [(X)] sich mindestens zwei Gruppen unterscheiden
- [( )] die Daten normalverteilt sind
- [( )] die Effektstärke groß ist

<details>
<summary><b>👉 Erklärung</b></summary>

Welche Gruppen sich unterscheiden, zeigen erst die Post-hoc-Tests.

</details>

**Frage 6:** Welche Angabe gehört <b>nicht</b> in den Bericht eines t-Tests?

- [( )] Mittelwerte und Standardabweichungen
- [( )] Teststatistik mit Freiheitsgraden
- [( )] Effektstärke
- [(X)] Der Dateiname des JASP-Projekts

<details>
<summary><b>👉 Erklärung</b></summary>

Berichtet werden Kennwerte, Teststatistik mit df, p-Wert und Effektstärke.

</details>

---

## Literatur

* Cohen, J. (1988). <i>Statistical power analysis for the behavioral sciences</i> (2nd ed.). Lawrence Erlbaum.
* Döring, N. & Bortz, J. (2016). <i>Forschungsmethoden und Evaluation in den Sozial- und Humanwissenschaften</i> (5. Aufl.). Springer.
* Eid, M., Gollwitzer, M. & Schmitt, M. (2017). <i>Statistik und Forschungsmethoden</i> (5. Aufl.). Beltz.
* JASP Team (2024). <i>JASP</i> (Version 0.19) [Computer software]. https://jasp-stats.org/
* Tomczak, M. & Tomczak, E. (2014). The need to report effect size estimates revisited. <i>Trends in Sport Sciences, 21</i>(1), 19–25.






##### Trainingsinnovation

**Ausgangslage**

Eine Sportwissenschaftlerin hat eine neue Krafttrainingsmethode "Wonder-Power" erfunden. Sie vermutet, dass *Wonder-Power* die Sprungkraft von Sportler*innen stärker fördert, als ein Standardtraining. Ihre Annahmen lassen sich wie folgt in Hypothesen überführen:  

**Operationalisierte Hypothesen** 

- H0: Sportler\*innen, die nach "Wonder-Power" trainiert haben und Sportler\*innen, die nach einem Standardtraining trainiert haben, unterscheiden sich nicht hinsichtlich der Verbesserung ihrer Sprunghöhe beim Jump and Reach. 
- H1: Sportler\*innen, die nach "Wonder-Power" trainiert haben und Sportler\*innen, die nach einem Standardtraining  trainiert haben, unterscheiden sich hinsichtlich der Verbesserung ihrer Sprunghöhe beim Jump and Reach. 

**Statistische Hypothesen**

- H0: M("Wonder-Power") = M("Standardtraining") 
- H1: M("Wonder-Power") ≠ M("Standardtraining") 

**Statistischer Hintergrund**

Wenn wir Personen in zwei Gruppen aufteilen und bei diesen Merkmale messen (z. B. Verbesserung der Sprunghöhe beim Jum and Reach), dann ist davon auszugehen, dass sich die Gruppen im Mittelwert unterscheiden, hier also nicht exakt die gleichen Ergebnisse vorliegen. In unserem Fall könnte es sein, dass M("Wonder-Power") = 10 cm und M("Standardtraining") = 7 cm. Aber ist der Unterschied von 3 cm ein bedeutsamer Unterschied oder eher zufällig? Um dies bewerten zu können, reichen die Informationen allein über den Mittelwert nicht aus, was an folgenden Beispielen aufgezeigt werden soll (s. Abbildungen).

![Streudiagramm 1](img/Stat_Streudiagramm1.jpg "Streudiagramm 1")
![Streudiagramm 2](img/Stat_Streudiagramm2.jpg "Streudiagramm 2")
![Streudiagramm 3](img/Stat_Streudiagramm3.jpg "Streudiagramm 3")

Text Text Text

![t_Berechnung](img/t_Berechnung.jpg)
Text

Wir brauchen also weitere Informationen 

- Wie viele Personen haben an der Studie teilgenommen?
- Wie groß ist die Streuung der Ergebnisse um den Mittelwert innerhalb der Gruppen?

Mit diesen Informationen können wir einen "standardisierten Mittelwertunterschied" berechnen wie folgt: 


**Empirisches Vorgehen**
@
## Entscheidung über den T-Wert


<div style="width:100%; max-width:960px; margin: 0 100px 0 0;">
  <iframe
    scrolling="no"
    title="T-Verteilung"
    src="https://www.geogebra.org/material/iframe/id/nvgjbxj7/width/950/height=558/border/888888/sfsb=true/smb=false/stb=false/stbh=false/ai=false/asb=false/sri=false/rc=false/ld=false/sdz=true/ctl=false"
    width="950"
    height="558"
    style="border:0px;"
    allowfullscreen
    allow="fullscreen">
  </iframe>
</div>

<p><a href="https://www.geogebra.org/m/nvgjbxj7" target="_blank" style="font-weight:bold;"> GeoGebra im Vollbild öffnen</a></p>
