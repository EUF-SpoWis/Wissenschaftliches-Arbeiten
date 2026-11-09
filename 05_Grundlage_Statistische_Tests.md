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
| **Link auf GitHub:**     | https://github.com/EUF-SpoWis/Wissenschaftliches-Arbeiten/blob/main/06_Zusammenhaenge_analysieren.md |
| **Autoren:**             | Tim Heemsoth & Swantje Brandt |

> (c) Alle Rechte vorbehalten.

---


## Welcher Test passt?


<iframe
  src="https://github.com/EUF-SpoWis/Wissenschaftliches-Arbeiten/blob/main/HTML%20Tools/entscheidungsbaum-tests.html"
  width="100%"
  height="700px"
  style="border: none;">
</iframe>


<div id="tests-baum">
<style>
#tests-baum {
    background: #ffffff; color: #1f2933; border: 1px solid #dbe2eb; border-radius: 16px; padding: 16px; max-width: 900px; margin: 20px auto; font-family: system-ui, sans-serif;
    --bg: #ffffff; --fg: #1f2933; --muted: #64748b; --card: #f3f6fa; --line: #cbd5e1;
    --root: #2f6f57; --root-fg: #ffffff;
    --zus: #4e66bd; --zus-bg: #eef2fb;
    --unt: #2a9a50; --unt-bg: #eaf6ee;
    --par: #2f6f57; --par-bg: #e3efe9;
    --non: #e08a1e; --non-bg: #fdf3e7;
    --mus: #4e66bd;
  }#tests-baum, #tests-baum * { box-sizing: border-box; }#tests-baum { font-family: system-ui, -apple-system, "Segoe UI", sans-serif; background: var(--bg); color: var(--fg);
         margin: 0; padding: 16px; line-height: 1.45; }#tests-baum .wrap { max-width: 880px; margin: 0 auto; }#tests-baum .tools { display: flex; gap: 8px; flex-wrap: wrap; margin-bottom: 12px; }#tests-baum .tools button { border: 1px solid var(--line); background: var(--card); color: var(--fg); border-radius: 8px;
                  padding: 6px 12px; font: inherit; font-size: .9rem; cursor: pointer; }#tests-baum .tools button:hover { border-color: var(--root); }#tests-baum .legend { display: flex; gap: 10px; flex-wrap: wrap; font-size: .85rem; margin-bottom: 14px; }#tests-baum .chip { display: inline-block; padding: 1px 10px; border-radius: 99px; font-size: .78rem; font-weight: 600; border: 2px solid; }#tests-baum .chip.par { color: var(--par); background: var(--par-bg); border-color: var(--par); }#tests-baum .chip.non { color: var(--non); background: var(--non-bg); border-color: var(--non); }#tests-baum .root { display: inline-block; background: var(--root); color: var(--root-fg); padding: 10px 16px;
          border-radius: 12px; font-weight: 700; margin-bottom: 10px; }#tests-baum /* Baum */
  details { margin: 6px 0; }#tests-baum details > summary { list-style: none; cursor: pointer; display: flex; align-items: center; gap: 10px;
                      padding: 9px 14px; border-radius: 12px; border: 2px solid var(--line); background: var(--card);
                      font-weight: 600; user-select: none; }#tests-baum details > summary::-webkit-details-marker { display: none; }#tests-baum details > summary::before { content: "▶"; font-size: .7rem; transition: transform .15s; flex: none; }#tests-baum details[open] > summary::before { transform: rotate(90deg); }#tests-baum details > summary:hover { filter: brightness(0.97); }#tests-baum details > summary small { font-weight: 400; color: var(--muted); font-size: .8rem; margin-left: auto; text-align: right; }#tests-baum .kids { margin: 4px 0 4px 18px; padding-left: 16px; border-left: 3px solid var(--line); }#tests-baum .zus > summary { background: var(--zus-bg); border-color: var(--zus); }#tests-baum .unt > summary { background: var(--unt-bg); border-color: var(--unt); }#tests-baum .lvl > summary { background: var(--bg); }#tests-baum /* Blätter */
  .leaf { margin: 6px 0; padding: 10px 14px; border: 2px solid var(--line); border-radius: 12px; background: var(--card); }#tests-baum .leaf .row { display: flex; flex-wrap: wrap; gap: 8px; align-items: center; }#tests-baum .leaf .q { font-weight: 600; margin-right: 4px; }#tests-baum .tests { display: grid; grid-template-columns: repeat(auto-fit, minmax(210px, 1fr)); gap: 8px; margin-top: 8px; }#tests-baum .test { border: 2px solid; border-radius: 10px; padding: 8px 10px; }#tests-baum .test.par { background: var(--par-bg); border-color: var(--par); }#tests-baum .test.non { background: var(--non-bg); border-color: var(--non); }#tests-baum .test b { display: block; margin-top: 3px; }#tests-baum .ex { margin-top: 6px; font-size: .85rem; color: var(--fg); border-left: 4px solid var(--mus); padding-left: 8px; }#tests-baum .single { margin-top: 8px; }#tests-baum .single .test { background: var(--zus-bg); border-color: var(--zus); }#tests-baum .note { margin-top: 14px; font-size: .8rem; color: var(--muted); }
</style>
<div class="intro" style="color:#64748b; margin-bottom: 10px;">Klicke auf die Äste, um den Entscheidungsbaum Schritt für Schritt aufzuklappen.</div>
  <div class="tools">
    <button type="button" class="tb-open">Alle aufklappen</button>
    <button type="button" class="tb-close">Alle zuklappen</button>
  </div>
  <div class="legend">
    <span><span class="chip par">parametrisch</span> Voraussetzungen erfüllt</span>
    <span><span class="chip non">nichtparametrisch</span> ordinal oder Voraussetzungen verletzt</span>
  </div>
  <div class="root">Was soll getestet werden?</div>
  <div class="kids" style="margin-left: 14px;">
        <details class="zus">
      <summary>🔗 Zusammenhänge <small>Hängen zwei Merkmale zusammen?</small></summary>
      <div class="kids">
        <details class="lvl">
          <summary>🏷️ Nominal</summary>
          <div class="kids">
            <div class="single"><div class="test"><span class="chip par">Test</span><b>Chi-Quadrat-Test</b>
              <div class="ex">🏃🏾‍♀️ Hängt die Musikbedingung damit zusammen, ob jemand den Lauf ohne Gehpause schafft (ja/nein)?</div></div></div>
          </div>
        </details>
        <details class="lvl">
          <summary>📶 Ordinal</summary>
          <div class="kids">
            <div class="single"><div class="test"><span class="chip par">Test</span><b>Kendall-Tau oder Spearman-Korrelation</b>
              <div class="ex">📋 Hängt die Trainingshäufigkeit (Stufen 1 bis 5) mit dem Borg-Wert zusammen?</div></div></div>
          </div>
        </details>
        <details class="lvl">
          <summary>📏 Metrisch</summary>
          <div class="kids">
            <div class="single"><div class="test"><span class="chip par">Test</span><b>Pearson-Korrelation</b>
              <div class="ex">🏃🏾‍♀️ Hängt das Tempo der Musik (BPM) mit der gelaufenen Strecke zusammen?</div></div></div>
          </div>
        </details>
      </div>
    </details>
        <details class="unt">
      <summary>⚖️ Unterschiede <small>Unterscheiden sich Gruppen oder Messungen?</small></summary>
      <div class="kids">
        <details class="lvl">
          <summary>👥 Unabhängige Stichproben <small>verschiedene Personen</small></summary>
          <div class="kids">
            <details class="lvl">
              <summary>2 Gruppen</summary>
              <div class="kids">
                <div class="tests">
                  <div class="test par"><span class="chip par">parametrisch</span><b>t-Test für unabhängige Stichproben</b></div>
                  <div class="test non"><span class="chip non">nichtparametrisch</span><b>Mann-Whitney-U-Test</b></div>
                </div>
                <div class="ex">🏃🏾‍♀️ Strecke mit gegen ohne Musik (verschiedene Personen)<br>📋 Borg-Wert mit gegen ohne Musik (verschiedene Personen)</div>
              </div>
            </details>
            <details class="lvl">
              <summary>mehr als 2 Gruppen</summary>
              <div class="kids">
                <div class="tests">
                  <div class="test par"><span class="chip par">parametrisch</span><b>ANOVA</b></div>
                  <div class="test non"><span class="chip non">nichtparametrisch</span><b>Kruskal-Wallis-Test</b></div>
                </div>
                <div class="ex">🏃🏾‍♀️ Strecke bei ohne, langsamer und schneller Musik (verschiedene Personen)</div>
              </div>
            </details>
          </div>
        </details>
        <details class="lvl">
          <summary>🔁 Abhängige Stichproben <small>dieselben Personen</small></summary>
          <div class="kids">
            <details class="lvl">
              <summary>2 Messungen</summary>
              <div class="kids">
                <div class="tests">
                  <div class="test par"><span class="chip par">parametrisch</span><b>t-Test für verbundene Stichproben</b></div>
                  <div class="test non"><span class="chip non">nichtparametrisch</span><b>Wilcoxon-Test</b></div>
                </div>
                <div class="ex">🏃🏾‍♀️ Strecke derselben Personen mit und ohne Musik<br>📋 Borg-Wert derselben Personen mit und ohne Musik</div>
              </div>
            </details>
            <details class="lvl">
              <summary>mehr als 2 Messungen</summary>
              <div class="kids">
                <div class="tests">
                  <div class="test par"><span class="chip par">parametrisch</span><b>ANOVA mit Messwiederholung</b></div>
                  <div class="test non"><span class="chip non">nichtparametrisch</span><b>Friedman-Test</b></div>
                </div>
                <div class="ex">🏃🏾‍♀️ Strecke derselben Personen bei ohne, langsamer und schneller Musik</div>
              </div>
            </details>
          </div>
        </details>
      </div>
    </details>
  </div>
  <p class="note">Faustregel: Metrische, annähernd normalverteilte Daten ➜ parametrischer Test. Ordinale Daten oder verletzte Voraussetzungen ➜ nichtparametrischer Test.</p>
</div>
<script>
(() => {
  const root = document.getElementById("tests-baum");
  if (!root || root.dataset.initialized === "true") return;
  root.dataset.initialized = "true";
  root.querySelector(".tb-open").addEventListener("click", () => root.querySelectorAll("details").forEach(d => d.open = true));
  root.querySelector(".tb-close").addEventListener("click", () => root.querySelectorAll("details").forEach(d => d.open = false));
})();
</script>








---

### Grundlagen
<section>

<div style="height: 15px;"></div>

--{{0}}--<div style="border-left: 6px solid #2e9e5b; background: rgba(46,158,91,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
💡 <b>Lehrbuch Hinweis:</b> Du hast eine Forschungsfrage, eine Hypothese und Daten erhoben. Jetzt musst du entscheiden, mit welchem Test du deine Hypothese prüfst. Die Wahl hängt von <b>drei Fragen</b> ab.
</div>

<div style="height: 15px;"></div>

<!-- class="animate__animated animate__fadeInUp" -->
<span style="background: #641a85; color: white; border-radius: 999px; padding: 0.1rem 0.7rem; font-weight: bold;">1. Zusammenhang oder Unterschied:</span> <span style="font-size: 1.1em;">Möchte ich wissen, <i>ob zwei Merkmale zusammenhängen</i>, oder <i>ob sich Gruppen bzw. Messzeitpunkte unterscheiden</i>?</span>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<span style="background: #9507a8; color: white; border-radius: 999px; padding: 0.1rem 0.7rem; font-weight: bold;">2. Skalenniveau und Stichprobe:</span> <span style="font-size: 1.1em;">Welches Skalenniveau haben meine Variablen, und wie viele Gruppen gibt es? Sind es <i>dieselben</i> oder <i>verschiedene</i> Personen?</span>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<span style="background: #420cc0; color: white; border-radius: 999px; padding: 0.1rem 0.7rem; font-weight: bold;">3. Parametrisch oder nicht:</span> <span style="font-size: 1.1em;">Sind die Voraussetzungen für einen parametrischen Test erfüllt (z. B. Normalverteilung)? Wenn nicht, gibt es nichtparametrische Alternativen.</span>

</section>

{{1}} <section>

<span style="font-size: 1.1em;"><b>Der Entscheidungsbaum im Überblick:</b></span>

<div style="display: flex; flex-wrap: wrap; gap: 12px; align-items: stretch; margin: 15px 0;">

<div style="flex: 1 1 140px; display: flex; align-items: center; justify-content: center; text-align: center; padding: 14px; border: 2px solid #2f6f57; border-radius: 10px; background: #2f6f57; color: #ffffff;"><b>Was soll getestet werden?</b></div>

<div style="flex: 3 1 360px; display: grid; gap: 12px;">

<div style="padding: 12px; border: 2px solid #4e66bd; border-radius: 10px; background: #eef2fb; color: #1f2933;"><b>🔗 Zusammenhänge</b><br><span style="font-size: 0.9em;">nominal ➜ Chi-Quadrat-Test · ordinal ➜ Kendall / Spearman · metrisch ➜ Pearson</span></div>

<div style="padding: 12px; border: 2px solid #2a9a50; border-radius: 10px; background: #eaf6ee; color: #1f2933;"><b>⚖️ Unterschiede</b><br><span style="font-size: 0.9em;">unabhängige oder abhängige Stichproben ➜ 2 oder mehr Gruppen ➜ parametrisch oder nichtparametrisch</span></div>

</div>

</div>

<div style="border-left: 6px solid #e0a526; background: rgba(224,165,38,0.14); border-radius: 8px; padding: 0.7rem 1.2rem;">
📌 <b>Merke:</b> Der Test hängt davon ab, <b>was</b> du wissen willst (Zusammenhang oder Unterschied), <b>was für Daten</b> du hast (Skalenniveau) und <b>wie</b> die Daten zustande kamen (dieselben oder verschiedene Personen).
</div>

<div style="height: 15px;"></div>

</section>

{{2}} <section>

<span style="font-size: 1.1em;"><b>Unser Datensatz aus dem Musikbeispiel:</b></span>

Alle Beispiele auf den folgenden Folien beziehen sich auf den 12-Minuten-Lauf mit und ohne Musik. So sieht ein Datensatz aus, den du später in JASP öffnest (jede Zeile ist eine Person bzw. eine Messung):

| Person | Bedingung | Strecke (m) | Borg-Wert |
| :-: | :-- | :-: | :-: |
| 1 | mit Musik | 2480 | 11 |
| 2 | mit Musik | 2650 | 13 |
| 3 | ohne Musik | 2350 | 13 |
| 4 | ohne Musik | 2480 | 15 |
| … | … | … | … |

<div style="display: flex; gap: 1.5rem; align-items: stretch; flex-wrap: wrap;">

<div style="flex: 1; min-width: 220px;">
<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem; height: 100%; box-sizing: border-box;">
🏃🏾‍♀️ <b>Strecke (m)</b> 🏃🏾‍♀️<br>
Ausdauerleistung, <b>metrisch</b> (Verhältnisskala).
</div>
</div>

<div style="flex: 1; min-width: 220px;">
<div style="border: 2px solid #2a9a50; border-radius: 12px; padding: 0.8rem 1.3rem; height: 100%; box-sizing: border-box;">
📋 <b>Borg-Wert (6 bis 20)</b> 📋<br>
Anstrengungsempfinden, streng genommen <b>ordinal</b>.
</div>
</div>

</div>

<div style="height: 15px;"></div>

</section>

---

### Zusammenhänge testen
<section>


--{{0}}--<div style="border-left: 6px solid #2e9e5b; background: rgba(46,158,91,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
💡 Bei Zusammenhängen bestimmt das <b>Skalenniveau</b> den Test.
</div>

<div style="height: 15px;"></div>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #eef2fb; border: 2px solid #4e66bd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🏷️</div>
<div style="text-align: center; font-size: 1.1em;"><b>Nominal</b></div>
<div style="text-align: center; font-style: italic; color: #4a5568; margin: 6px 0 8px 0;">„Hängen zwei Kategorien zusammen?“</div>
<div style="font-size: 0.9em;"><b>Chi-Quadrat-Test</b><br>Vergleicht, ob die Häufigkeiten in den Kategorien so verteilt sind, wie es ohne Zusammenhang zu erwarten wäre.</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #ffffff; border-left: 4px solid #4e66bd; border-radius: 0 8px 8px 0; font-size: 0.85em;">🏃🏾‍♀️ Hängt die Bedingung (mit/ohne Musik) damit zusammen, ob jemand den Lauf <b>ohne Gehpause</b> schafft (ja/nein)?</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> Frequencies ➜ Contingency Tables</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #eef2fb; border: 2px solid #4e66bd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📶</div>
<div style="text-align: center; font-size: 1.1em;"><b>Ordinal</b></div>
<div style="text-align: center; font-style: italic; color: #4a5568; margin: 6px 0 8px 0;">„Steigt der eine Rang, wenn der andere steigt?“</div>
<div style="font-size: 0.9em;"><b>Kendall-Tau oder Spearman-Korrelation</b><br>Zusammenhang zwischen Rangfolgen.</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #ffffff; border-left: 4px solid #2a9a50; border-radius: 0 8px 8px 0; font-size: 0.85em;">📋 Hängt der <b>Borg-Wert</b> mit der Rangplatzierung im Lauf zusammen?</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> Regression ➜ Classical ➜ Correlation (Spearman bzw. Kendall’s tau-b anhaken)</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #eef2fb; border: 2px solid #4e66bd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📏</div>
<div style="text-align: center; font-size: 1.1em;"><b>Metrisch</b></div>
<div style="text-align: center; font-style: italic; color: #4a5568; margin: 6px 0 8px 0;">„Wie stark hängen zwei Messwerte zusammen?“</div>
<div style="font-size: 0.9em;"><b>Pearson-Korrelation (<i>r</i>)</b><br>Linearer Zusammenhang zwischen zwei metrischen Variablen.</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #ffffff; border-left: 4px solid #4e66bd; border-radius: 0 8px 8px 0; font-size: 0.85em;">🏃🏾‍♀️ Hängt die <b>Strecke</b> mit dem <b>Tempo (BPM) der Musik</b> zusammen?</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> Regression ➜ Classical ➜ Correlation (Pearson)</div>
</div>

</div>

<div style="border-left: 6px solid #e0a526; background: rgba(224,165,38,0.14); border-radius: 8px; padding: 0.7rem 1.2rem;">
📌 <b>Merke:</b> Ein Zusammenhang sagt nichts über <b>Ursache und Wirkung</b>. Dafür braucht es ein Experiment (siehe Kapitel Design).
</div>

<div style="height: 15px;"></div>

</section>

---

### Unterschiede testen
<section>

--{{0}}--<div style="border-left: 6px solid #2e9e5b; background: rgba(46,158,91,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
💡 Hier brauchst du zwei Entscheidungen: <b>Sind die Stichproben unabhängig oder abhängig?</b> und <b>Wie viele Gruppen bzw. Messzeitpunkte gibt es?</b>
</div>

<div style="height: 15px;"></div>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #eef2fb; border: 2px solid #4e66bd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">👥</div>
<div style="text-align: center; font-size: 1.1em;"><b>Unabhängige Stichproben</b></div>
<div style="text-align: center; font-style: italic; color: #4a5568; margin: 6px 0 8px 0;">„Sind es verschiedene Personen?“</div>
<div style="font-size: 0.9em;">Jede Person gehört nur zu <b>einer</b> Gruppe.</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #ffffff; border-left: 4px solid #4e66bd; border-radius: 0 8px 8px 0; font-size: 0.85em;">🏃🏾‍♀️ 20 Läufer:innen laufen <b>mit</b> Musik, 20 <b>andere</b> laufen <b>ohne</b> Musik.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #eaf6ee; border: 2px solid #2a9a50; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔁</div>
<div style="text-align: center; font-size: 1.1em;"><b>Abhängige Stichproben</b></div>
<div style="text-align: center; font-style: italic; color: #4a5568; margin: 6px 0 8px 0;">„Sind es dieselben Personen?“</div>
<div style="font-size: 0.9em;">Dieselben Personen werden <b>mehrfach</b> gemessen (oder sind gepaart).</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #ffffff; border-left: 4px solid #4e66bd; border-radius: 0 8px 8px 0; font-size: 0.85em;">🏃🏾‍♀️ Dieselben 20 Läufer:innen laufen einmal <b>mit</b> und einmal <b>ohne</b> Musik.</div>
</div>

</div>

</section>

{{1}} <section>

<span style="font-size: 1.1em;"><b>Welche Tests gibt es? (Im Beispiel: Wie viele Bedingungen vergleiche ich?)</b></span>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 12px; padding: 10px; color: #1f2933;">
<table style="width: 100%; border-collapse: collapse; font-size: 0.9em;">
<tr><th style="text-align: left; padding: 8px;">Stichprobe</th><th style="padding: 8px; background: #2f6f57; color: #ffffff;">Parametrisch</th><th style="padding: 8px; background: #e08a1e; color: #ffffff;">Nichtparametrisch</th><th style="text-align: left; padding: 8px;">Musikbeispiel</th></tr>
<tr style="border-bottom: 1px solid #cbd5e1;"><td style="padding: 8px;"><b>Unabhängig</b><br><span style="font-size: 0.85em;">2 Gruppen</span></td><td style="padding: 8px; background: #e3efe9;">t-Test für unabhängige Stichproben</td><td style="padding: 8px; background: #fdf3e7;">Mann-Whitney-U-Test</td><td style="padding: 8px; font-size: 0.85em;">🏃🏾‍♀️ Strecke: mit Musik gegen ohne Musik (verschiedene Personen)<br>📋 Borg-Wert: dito</td></tr>
<tr style="border-bottom: 1px solid #cbd5e1;"><td style="padding: 8px;"><b>Unabhängig</b><br><span style="font-size: 0.85em;">mehr als 2 Gruppen</span></td><td style="padding: 8px; background: #e3efe9;">ANOVA</td><td style="padding: 8px; background: #fdf3e7;">Kruskal-Wallis-Test</td><td style="padding: 8px; font-size: 0.85em;">🏃🏾‍♀️ Strecke bei ohne / langsamer / schneller Musik (verschiedene Personen)</td></tr>
<tr style="border-bottom: 1px solid #cbd5e1;"><td style="padding: 8px;"><b>Abhängig</b><br><span style="font-size: 0.85em;">2 Messungen</span></td><td style="padding: 8px; background: #e3efe9;">t-Test für verbundene Stichproben</td><td style="padding: 8px; background: #fdf3e7;">Wilcoxon-Test</td><td style="padding: 8px; font-size: 0.85em;">🏃🏾‍♀️ Strecke derselben Personen mit und ohne Musik<br>📋 Borg-Wert: dito</td></tr>
<tr style="border-bottom: 1px solid #cbd5e1;"><td style="padding: 8px;"><b>Abhängig</b><br><span style="font-size: 0.85em;">mehr als 2 Messungen</span></td><td style="padding: 8px; background: #e3efe9;">ANOVA mit Messwiederholung</td><td style="padding: 8px; background: #fdf3e7;">Friedman-Test</td><td style="padding: 8px; font-size: 0.85em;">🏃🏾‍♀️ Strecke derselben Personen bei ohne / langsamer / schneller Musik</td></tr>
</table>
</div>

<div style="height: 10px;"></div>

<div style="border-left: 6px solid #e0a526; background: rgba(224,165,38,0.14); border-radius: 8px; padding: 0.7rem 1.2rem;">
📌 <b>Merke:</b> Die Zeilen bestimmst du über das <b>Studiendesign</b> (dieselben oder verschiedene Personen, wie viele Bedingungen), die Spalten über die <b>Voraussetzungen</b> deiner Daten (nächste Folie).
</div>

<div style="height: 15px;"></div>

</section>

---

### Parametrisch oder nichtparametrisch?
<section>


--{{0}}--<div style="border-left: 6px solid #2e9e5b; background: rgba(46,158,91,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
💡 Parametrische Tests liefern bei erfüllten Voraussetzungen die höchste Aussagekraft. Sind die Voraussetzungen verletzt, weichst du auf einen nichtparametrischen Test aus.
</div>

<div style="height: 15px;"></div>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📏</div>
<div style="text-align: center; font-size: 1.1em;"><b>Metrisches Skalenniveau</b></div>
<div style="text-align: center; font-style: italic; color: #4a5568; margin: 6px 0 8px 0;">„Kann ich einen Mittelwert sinnvoll berechnen?“</div>
<div style="font-size: 0.9em;">Parametrische Tests rechnen mit Mittelwerten und Standardabweichungen.</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #ffffff; border-left: 4px solid #4e66bd; border-radius: 0 8px 8px 0; font-size: 0.85em;">🏃🏾‍♀️ Strecke in Metern: <b>ja</b>.</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #ffffff; border-left: 4px solid #2a9a50; border-radius: 0 8px 8px 0; font-size: 0.85em;">📋 Borg-Wert: streng genommen ordinal, daher eher <b>nichtparametrisch</b> (oder begründet als metrisch behandeln).</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔔</div>
<div style="text-align: center; font-size: 1.1em;"><b>Normalverteilung</b></div>
<div style="text-align: center; font-style: italic; color: #4a5568; margin: 6px 0 8px 0;">„Ist die Verteilung ungefähr glockenförmig?“</div>
<div style="font-size: 0.9em;">Prüfen mit Histogramm, Q-Q-Plot oder Shapiro-Wilk-Test. Bei großen Stichproben sind die Tests weniger empfindlich gegen Abweichungen.</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> Assumption Checks ➜ Normality (Q-Q plot, Shapiro-Wilk)</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">⚖️</div>
<div style="text-align: center; font-size: 1.1em;"><b>Gleiche Streuung</b></div>
<div style="text-align: center; font-style: italic; color: #4a5568; margin: 6px 0 8px 0;">„Streuen die Gruppen ähnlich stark?“</div>
<div style="font-size: 0.9em;">Varianzhomogenität bei unabhängigen Gruppen, prüfbar mit dem Levene-Test.</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> Assumption Checks ➜ Equality of variances (Levene)</div>
</div>

</div>

</section>

{{1}} <section>

<div style="border: 2px solid #a74ebd; border-radius: 12px; padding: 0.8rem 1.3rem; background: #f6f1fa; color: #1f2933;">
<b>Faustregel:</b> Voraussetzungen erfüllt ➜ <span style="background: #e3efe9; padding: 0 6px; border-radius: 6px;">parametrischer Test</span> · Voraussetzungen verletzt oder ordinale Daten ➜ <span style="background: #fdf3e7; padding: 0 6px; border-radius: 6px;">nichtparametrischer Test</span>
</div>

<div style="height: 15px;"></div>

<div style="display: flex; gap: 1.5rem; align-items: stretch; flex-wrap: wrap;">

<div style="flex: 1; min-width: 220px;">
<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem; height: 100%; box-sizing: border-box;">
🏃🏾‍♀️ <b>Strecke mit/ohne Musik</b> 🏃🏾‍♀️<br>
Wenn die Strecken ungefähr normalverteilt sind: <b>t-Test</b>. Gibt es starke Ausreißer: <b>Mann-Whitney-U-Test</b>.
</div>
</div>

<div style="flex: 1; min-width: 220px;">
<div style="border: 2px solid #2a9a50; border-radius: 12px; padding: 0.8rem 1.3rem; height: 100%; box-sizing: border-box;">
📋 <b>Borg-Wert mit/ohne Musik</b> 📋<br>
Ordinale Skala: <b>Mann-Whitney-U-Test</b> (bei denselben Personen: <b>Wilcoxon-Test</b>).
</div>
</div>

</div>

<div style="height: 15px;"></div>

</section>

---

### So gehst du in JASP vor
<section>


--{{0}}--<div style="border-left: 6px solid #2e9e5b; background: rgba(46,158,91,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
💡 JASP ist ein kostenloses Statistikprogramm mit grafischer Oberfläche. Die Ergebnisse aktualisieren sich automatisch, sobald du Einstellungen änderst.
</div>

<div style="height: 15px;"></div>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📂</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Daten laden</b></div>
<div style="font-size: 0.9em;">Datei (.csv oder .xlsx) per „Open“ öffnen. Jede Zeile ist eine Person bzw. Messung, jede Spalte eine Variable.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🏷️</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Skalenniveau prüfen</b></div>
<div style="font-size: 0.9em;">Oben in der Datenspalte das Symbol anklicken und das Skalenniveau einstellen (nominal, ordinal, scale). Falsche Einstellung ➜ falsche Analysen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔍</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Daten ansehen</b></div>
<div style="font-size: 0.9em;">Unter „Descriptives“ Kennwerte, Histogramme und Boxplots anfordern, um Ausreißer und Verteilung zu erkennen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧪</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Test auswählen</b></div>
<div style="font-size: 0.9em;">In der oberen Menüleiste die passende Analyse wählen und die Variablen in die Felder ziehen (z. B. Strecke ➜ „Dependent Variables“, Bedingung ➜ „Grouping Variable“).</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Voraussetzungen prüfen</b></div>
<div style="font-size: 0.9em;">Unter „Assumption Checks“ Normalverteilung und Varianzhomogenität anhaken und ablesen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📖</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Ergebnis lesen</b></div>
<div style="font-size: 0.9em;">Teststatistik, <i>p</i>-Wert und Effektstärke ablesen und in einem Satz berichten.</div>
</div>

</div>

!?[Allgemeine Einführung in JASP](https://youtu.be/DFmlkq6a8gc)

</section>

{{1}} <section>

<details>
<summary><b>👉 Klicke hier, um zu sehen wo du welchen Test in JASP findest.</b></summary>

<span style="font-size: 1.1em;"><b>Wo finde ich welchen Test in JASP?</b></span>

| Test | Pfad in JASP |
| :--- | :----------- |
| Chi-Quadrat-Test | Frequencies ➜ Classical ➜ Contingency Tables |
| Pearson, Spearman, Kendall | Regression ➜ Classical ➜ Correlation |
| t-Test für unabhängige Stichproben (und Mann-Whitney-U) | T-Tests ➜ Classical ➜ Independent Samples T-Test (unter „Tests“ Student, Welch oder Mann-Whitney wählen) |
| t-Test für verbundene Stichproben (und Wilcoxon) | T-Tests ➜ Classical ➜ Paired Samples T-Test (unter „Tests“ Student oder Wilcoxon wählen) |
| ANOVA (und Kruskal-Wallis) | ANOVA ➜ Classical ➜ ANOVA (Kruskal-Wallis im Bereich „Nonparametrics“) |
| ANOVA mit Messwiederholung (und Friedman) | ANOVA ➜ Classical ➜ Repeated Measures ANOVA (Friedman im Bereich „Nonparametrics“) |

<div style="font-size: 0.85em; opacity: 0.8;">Die Menüführung kann sich je nach JASP-Version leicht unterscheiden.</div>

</details>

!?[Allgemeine Einführung in JASP](https://youtu.be/36LUe7ZsV08)

</section>

---

### Beispiele aus dem Musikprojekt

<details>
<summary><b>👉 Beispiel 1: Zwei verschiedene Gruppen</b></summary>

<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
🏃🏾‍♀️ <b>Strecke, mit gegen ohne Musik</b><br>
<b>Frage:</b> Laufen Personen mit Musik weiter als Personen ohne Musik?<br>
<b>Daten:</b> Bedingung (nominal, 2 Gruppen, verschiedene Personen), Strecke (metrisch)<br>
<b>Test:</b> t-Test für unabhängige Stichproben (bei verletzten Voraussetzungen: Mann-Whitney-U-Test)<br>
<b>H0:</b> Es gibt keinen Unterschied in der mittleren Strecke.
</div>

<div style="border: 2px solid #2a9a50; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
📋 <b>Borg-Wert, mit gegen ohne Musik</b><br>
<b>Frage:</b> Empfinden Personen mit Musik den Lauf als weniger anstrengend?<br>
<b>Daten:</b> Bedingung (nominal, 2 Gruppen), Borg-Wert (ordinal)<br>
<b>Test:</b> Mann-Whitney-U-Test<br>
<b>H0:</b> Es gibt keinen Unterschied im Anstrengungsempfinden.
</div>

<!-- TODO: JASP-Screenshot Independent Samples T-Test mit Strecke -->

</details>

<details>
<summary><b>👉 Beispiel 2: Dieselben Personen zweimal</b></summary>

<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
🏃🏾‍♀️ <b>Strecke, mit gegen ohne Musik</b><br>
<b>Frage:</b> Laufen dieselben Personen mit Musik weiter als ohne Musik?<br>
<b>Daten:</b> zwei Messungen pro Person (Strecke, metrisch)<br>
<b>Test:</b> t-Test für verbundene Stichproben (bei verletzten Voraussetzungen: Wilcoxon-Test)<br>
<b>H0:</b> Es gibt keinen Unterschied zwischen den beiden Messungen.
</div>

<div style="border: 2px solid #2a9a50; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
📋 <b>Borg-Wert, mit gegen ohne Musik</b><br>
<b>Frage:</b> Empfinden dieselben Personen den Lauf mit Musik als weniger anstrengend?<br>
<b>Daten:</b> zwei Messungen pro Person (Borg-Wert, ordinal)<br>
<b>Test:</b> Wilcoxon-Test<br>
<b>H0:</b> Es gibt keinen Unterschied zwischen den beiden Messungen.
</div>

<!-- TODO: JASP-Screenshot Paired Samples T-Test -->

</details>

<details>
<summary><b>👉 Beispiel 3: Drei Musikbedingungen</b></summary>

<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
🏃🏾‍♀️ <b>Strecke bei ohne / langsamer / schneller Musik</b><br>
<b>Frage:</b> Unterscheidet sich die Strecke je nach Musiktempo?<br>
<b>Daten:</b> Bedingung (nominal, 3 Gruppen), Strecke (metrisch)<br>
<b>Test:</b> ANOVA (verschiedene Personen) bzw. ANOVA mit Messwiederholung (dieselben Personen). Alternativen: Kruskal-Wallis bzw. Friedman.<br>
<b>H0:</b> Alle drei Bedingungen haben dieselbe mittlere Strecke.
</div>

<!-- TODO: JASP-Screenshot ANOVA mit Post-hoc-Tests -->

</details>

<details>
<summary><b>👉 Beispiel 4: Zusammenhang</b></summary>

<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
🏃🏾‍♀️ <b>Strecke und Tempo der Musik</b><br>
<b>Frage:</b> Laufen Personen weiter, je schneller die Musik ist?<br>
<b>Daten:</b> Tempo (BPM, metrisch), Strecke (metrisch)<br>
<b>Test:</b> Pearson-Korrelation (bei ordinalen Daten: Spearman oder Kendall)<br>
<b>H0:</b> Es gibt keinen Zusammenhang zwischen Tempo und Strecke.
</div>

</details>

<div style="border-left: 6px solid #4e66bd; background: #f2f6fb; border-radius: 0 12px 12px 0; padding: 1rem 1.4rem; margin: 1rem 0; color: #1f2933;">
📋 Überlege dir für deine eigene Studie: Wie viele <b>Gruppen oder Messungen</b> hast du, sind es <b>dieselben oder verschiedene Personen</b>, und welches <b>Skalenniveau</b> hat deine abhängige Variable? Welcher Test folgt daraus? Mache dir Notizen.
</div>

<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Zum Nachlesen: Döring & Bortz (2016); Eid, Gollwitzer & Schmitt (2017); JASP Team (2024)
</div>

---

### Check-Up: Testwahl

<!-- class="animate__animated animate__fadeIn" -->
<div style="border-left: 6px solid #a74ebd; background: rgba(185, 145, 215, 0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
<span style="font-size: 1.3em;"><i>Welcher Test passt zu welcher Fragestellung? Teste dein Wissen.</i></span>
</div>

<div style="height: 15px;"></div>

Beantworte die Fragen. Bei einigen Fragen hilft dir ein Hinweis, und nach dem Beantworten bekommst du eine kurze Erklärung.

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

Zwei abhängige Messungen mit ordinalen Daten ➜ Wilcoxon-Test (nichtparametrische Alternative zum t-Test für verbundene Stichproben).

</details>

**Frage 3:** Du vergleichst die Strecke bei drei Bedingungen (ohne, langsame, schnelle Musik) mit drei verschiedenen Gruppen. Die Voraussetzungen sind erfüllt. Welcher Test passt?

- [( )] t-Test für unabhängige Stichproben
- [(X)] ANOVA
- [( )] Friedman-Test
- [( )] Spearman-Korrelation

[[?]] Mehr als zwei unabhängige Gruppen.

<details>
<summary><b>👉 Erklärung</b></summary>

Mehr als zwei unabhängige Gruppen mit metrischer Messung ➜ ANOVA. Der Friedman-Test wäre die Variante für dieselben Personen mit nichtparametrischen Daten.

</details>

**Frage 4:** Du willst prüfen, ob die Strecke mit dem Tempo der Musik (BPM) zusammenhängt. Beide Variablen sind metrisch. Welcher Test passt?

- [( )] Chi-Quadrat-Test
- [(X)] Pearson-Korrelation
- [( )] Kruskal-Wallis-Test
- [( )] Mann-Whitney-U-Test

<details>
<summary><b>👉 Erklärung</b></summary>

Zusammenhang zwischen zwei metrischen Variablen ➜ Pearson-Korrelation.

</details>

**Frage 5:** Du willst prüfen, ob Bedingung (mit/ohne Musik) und Gehpause (ja/nein) zusammenhängen. Beide Variablen sind nominal. Welcher Test passt?

- [( )] Pearson-Korrelation
- [( )] t-Test
- [(X)] Chi-Quadrat-Test
- [( )] ANOVA

[[?]] Beide Variablen sind Kategorien.

<details>
<summary><b>👉 Erklärung</b></summary>

Zwei nominale Variablen ➜ Chi-Quadrat-Test.

</details>

---

### Literatur

* Döring, N. &a Bortz, J. (2016). <i>Forschungsmethoden und Evaluation in den Sozial- und Humanwissenschaften</i> (5. Aufl.). Springer.
* Eid, M., Gollwitzer, M. &a Schmitt, M. (2017). <i>Statistik und Forschungsmethoden</i> (5. Aufl.). Beltz.
* JASP Team (2024). <i>JASP</i> (Version 0.19) [Computer software]. https://jasp-stats.org/


## Deskriptive Statistik, Reliabilität und Skalenmittelwerte in JASP


--{{0}}--<div style="border-left: 6px solid #2e9e5b; background: rgba(46,158,91,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
💡 <b>Lehrbuch Hinweis:</b> Bevor du Tests rechnest, lernst du deine Daten kennen: Du berechnest <b>Kennwerte</b>, prüfst bei Fragebögen, ob die Items <b>zuverlässig</b> messen, und bildest <b>Skalenmittelwerte</b>. Alle drei Schritte machst du in JASP.
</div>

<div style="height: 15px;"></div>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📊</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Deskriptive Statistik</b></div>
<div style="font-size: 0.9em;">Kennwerte und Grafiken je Gruppe.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔍</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Reliabilitätsanalyse</b></div>
<div style="font-size: 0.9em;">Messen die Items einer Skala dasselbe? (Cronbachs α)</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧮</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Skalenmittelwerte</b></div>
<div style="font-size: 0.9em;">Ein Wert pro Person aus mehreren Items.</div>
</div>

</div>

---

### Deskriptive Statistik in JASP


<span style="font-size: 1.1em;"><b>Wann brauche ich das?</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔎</div>
<div style="text-align: center; font-size: 1.1em;"><b>Daten kennenlernen</b></div>
<div style="font-size: 0.9em;">Wie groß sind Mittelwert und Streuung? Wie sehen die Verteilungen aus?</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🚨</div>
<div style="text-align: center; font-size: 1.1em;"><b>Fehler finden</b></div>
<div style="font-size: 0.9em;">Tippfehler, Ausreißer und unplausible Werte fallen sofort auf.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>Voraussetzungen prüfen</b></div>
<div style="font-size: 0.9em;">Histogramm und Q-Q-Plot zeigen, ob eine Normalverteilung plausibel ist.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✍️</div>
<div style="text-align: center; font-size: 1.1em;"><b>Berichten</b></div>
<div style="font-size: 0.9em;"><i>M</i>, <i>SD</i> und <i>Mdn</i> je Gruppe gehören in jeden Ergebnisteil.</div>
</div>

</div>

<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
🏃🏾‍♀️ <b>Wirkung auf die Ausdauerleistung</b>🏃🏾‍♀️<br>
Du beschreibst die <b>Strecke</b> (metrisch) je Gruppe mit Mittelwert und Standardabweichung.
</div>

<div style="border: 2px solid #2a9a50; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
📋 <b>Wirkung auf das Anstrengungsempfinden</b> 📋<br>
Du beschreibst den <b>Borg-Wert</b> (ordinal) je Gruppe vor allem mit Median, Minimum und Maximum.
</div>

{{1}} <section>

<span style="font-size: 1.1em;"><b>Durchführung in JASP</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🏷️</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Skalenniveau prüfen</b></div>
<div style="font-size: 0.9em;">Strecke als scale, Borg-Wert als ordinal, Bedingung als nominal.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧪</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Analyse öffnen</b></div>
<div style="font-size: 0.9em;">Descriptives ➜ Descriptive Statistics.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔗</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Variablen zuweisen</b></div>
<div style="font-size: 0.9em;">Strecke und Borg-Wert in „Variables“, Bedingung in „Split“.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">☑️</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Kennwerte wählen</b></div>
<div style="font-size: 0.9em;">Unter „Statistics“ Mean, Median, Mode, Std. deviation, Minimum, Maximum und Range anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📈</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Grafiken</b></div>
<div style="font-size: 0.9em;">Unter „Plots“ Distribution plots, Boxplots und Q-Q plots anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📋</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Tabelle übernehmen</b></div>
<div style="font-size: 0.9em;">Rechtsklick auf die Tabelle ➜ „Copy“ und in dein Dokument einfügen.</div>
</div>

</div>

<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> Descriptives ➜ Descriptive Statistics</div>
<div style="height: 10px;"></div>


</section>

{{2}} <section>

<span style="font-size: 1.1em;"><b>Ergebnis lesen</b></span>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Descriptive Statistics – Strecke (m)</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;"></th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">mit Musik</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">ohne Musik</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Valid</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">20</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">20</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Mode</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2260<sup>a</sup></td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2130<sup>a</sup></td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Median</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2580,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2440,00</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Mean</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2585,50</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2449,00</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Std. Deviation</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">195,33</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">185,87</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Variance</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">38152,37</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">34546,32</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Range</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">690,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">680,00</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Minimum</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2260,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2130,00</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Maximum</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2950,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2810,00</td></tr>
</table>
</div>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Descriptive Statistics – Borg-Wert</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;"></th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">mit Musik</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">ohne Musik</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Valid</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">20</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">20</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Mode</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">12</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">14</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Median</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">12,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">14,00</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Mean</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">12,40</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">14,40</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Std. Deviation</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">1,43</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">1,43</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Range</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">5,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">5,00</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Minimum</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">10,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">12,00</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Maximum</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">15,00</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">17,00</td></tr>
</table>
</div>

<div style="font-size: 0.8em; opacity: 0.7;"><sup>a</sup> Es gibt mehrere Modi, angezeigt wird der kleinste.</div>

<div style="font-size: 0.8em; opacity: 0.7; margin-bottom: 10px;">Fiktive Daten, nachgebaut im Stil der JASP-Ausgabe.</div>

<ul style="font-size: 0.95em;">
<li><b>Valid:</b> Anzahl gültiger Werte je Gruppe (hier 20). „Missing“ zeigt fehlende Werte.</li>
<li><b>Mean und Median:</b> Liegen sie nah beieinander (Strecke: 2585,5 und 2580,0 m), ist die Verteilung ungefähr symmetrisch.</li>
<li><b>Std. Deviation:</b> Die Strecken streuen mit Musik um etwa 195 m um den Mittelwert.</li>
<li><b>Range, Minimum, Maximum:</b> Prüfe auf Plausibilität. Der Borg-Wert muss zwischen 6 und 20 liegen, die Strecke darf nicht negativ sein.</li>
<li><b>Boxplot:</b> Punkte außerhalb der „Whiskers“ sind mögliche Ausreißer. Prüfe sie, entferne sie aber nie ohne Begründung.</li>
</ul>

</section>

{{3}} <section>

<span style="font-size: 1.1em;"><b>So berichtest du das Ergebnis</b></span>

<div style="border-left: 6px solid #a74ebd; background: #f6f1fa; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
✍️ <b>Musterbericht (APA):</b><br>
<i>Mit Musik wurde im Mittel weiter gelaufen (M = 2585,50 m, SD = 195,33, Mdn = 2580) als ohne Musik (M = 2449,00 m, SD = 185,87, Mdn = 2440). Der Borg-Wert lag mit Musik bei Mdn = 12 (Spannweite 10–15) und ohne Musik bei Mdn = 14 (Spannweite 12–17).</i>
</div>

<details>
<summary><b>👉 Was kann bei den Daten schiefgehen?</b></summary>

| Problem | Woran du es erkennst | Lösung |
| :-- | :-- | :-- |
| Falsches Skalenniveau | „Mean“ fehlt oder wird nicht angezeigt | Spaltensymbol anklicken, auf „scale“ umstellen |
| Tippfehler | Maximum oder Minimum unplausibel (z. B. Borg-Wert 22) | Rohdaten prüfen und korrigieren |
| Fehlende Werte | „Missing“ größer als 0 | Ursache klären, Codes wie 999 als fehlend definieren |
| Ausreißer | Punkte im Boxplot | Prüfen, ob echt oder Fehler; Analyse mit und ohne berichten |

</details>

!?[Allgemeine Einführung in JASP](https://youtu.be/2lGMEnK6f2A)

<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Döring & Bortz (2016); Eid, Gollwitzer & Schmitt (2017); JASP Team (2024)
</div>

</section>

---

### Reliabilitätsanalyse in JASP

<span style="font-size: 1.1em;"><b>Wann brauche ich das?</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧩</div>
<div style="text-align: center; font-size: 1.1em;"><b>Mehrere Items</b></div>
<div style="font-size: 0.9em;">Du misst ein Merkmal mit mehreren Aussagen (Items) und willst wissen, ob sie zusammenpassen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📏</div>
<div style="text-align: center; font-size: 1.1em;"><b>Interne Konsistenz</b></div>
<div style="font-size: 0.9em;">Cronbachs α und McDonalds ω zeigen, wie stark die Items zusammenhängen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">↩️</div>
<div style="text-align: center; font-size: 1.1em;"><b>Umpolen nötig</b></div>
<div style="font-size: 0.9em;">Negativ gepolte Items müssen vorher umgepolt werden, sonst ist α falsch.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🚫</div>
<div style="text-align: center; font-size: 1.1em;"><b>Nicht für Einzelitems</b></div>
<div style="font-size: 0.9em;">Bei einem einzelnen Wert (z. B. Borg-Skala) gibt es kein α.</div>
</div>

</div>

<div style="border: 2px solid #2a9a50; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
📋 <b>Wirkung auf das Anstrengungsempfinden</b> 📋<br>
Die Skala <b>Anstrengungsempfinden</b> besteht aus 4 Items (1 = trifft gar nicht zu bis 5 = trifft völlig zu):<br>1 „Der 12-Minuten-Lauf war körperlich anstrengend.“<br>2 „Ich musste mich beim Laufen überwinden.“<br>3 „Nach dem Lauf fühlte ich mich erschöpft.“<br>4 „Der Lauf ist mir leicht gefallen.“ <b>(negativ gepolt)</b>
</div>

<div style="font-size: 0.8em; opacity: 0.7;">Fiktive Daten von 30 Personen (15 mit, 15 ohne Musik).</div>

{{1}} <section>

<span style="font-size: 1.1em;"><b>Durchführung in JASP</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🏷️</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Skalenniveau</b></div>
<div style="font-size: 0.9em;">Alle Items als ordinal oder scale einstellen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧪</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Analyse öffnen</b></div>
<div style="font-size: 0.9em;">Reliability ➜ Single-Test Reliability Analysis (in älteren Versionen: Factor ➜ Reliability Analysis).</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔗</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Items zuweisen</b></div>
<div style="font-size: 0.9em;">Alle vier Items in „Variables“ ziehen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">↩️</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Umpolen</b></div>
<div style="font-size: 0.9em;">Item 4 in das Feld „Reverse-scaled items“ ziehen (das Umpolen übernimmt JASP).</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">☑️</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Kennwerte</b></div>
<div style="font-size: 0.9em;">Cronbach’s α und McDonald’s ω anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔍</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Itemstatistik</b></div>
<div style="font-size: 0.9em;">Unter „Individual item statistics“ „α if item dropped“ und „Item-rest correlation“ anhaken.</div>
</div>

</div>

<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> Reliability ➜ Single-Test Reliability Analysis</div>
<div style="height: 10px;"></div>


</section>

{{2}} <section>

<span style="font-size: 1.1em;"><b>Ergebnis lesen</b></span>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Scale Reliability Statistics</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;"></th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Estimate</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Cronbach’s α</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,86</td></tr>
</table>
</div>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Individual Item Reliability Statistics</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Item</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Cronbach’s α (if item dropped)</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Item-rest correlation</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Item 1</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,82</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,73</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Item 2</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,79</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,80</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Item 3</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,82</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,72</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Item 4 (umgepolt)</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,87</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,60</td></tr>
</table>
</div>

<div style="font-size: 0.8em; opacity: 0.7; margin-bottom: 10px;">Fiktive Daten, nachgebaut im Stil der JASP-Ausgabe.</div>

<ul style="font-size: 0.95em;">
<li><b>Cronbachs α:</b> ,86 ➜ gute interne Konsistenz. Als Faustregel gelten ab ,70 akzeptable, ab ,80 gute und ab ,90 sehr gute Werte.</li>
<li><b>Item-rest correlation (Trennschärfe):</b> Sie zeigt, wie gut ein Item zur restlichen Skala passt. Alle vier Items liegen zwischen ,60 und ,80, also über ,30.</li>
<li><b>α if item dropped:</b> Würde α deutlich steigen, wenn du ein Item weglässt, passt dieses Item schlecht. Hier sinkt α beim Weglassen von Item 1 bis 3 (auf ,82, ,79 und ,82), bei Item 4 steigt es nur minimal auf ,87. Weil die Trennschärfe von Item 4 mit ,60 noch gut ist, bleibt es in der Skala.</li>
<li><b>McDonald’s ω:</b> JASP zeigt es zusätzlich an. Es ist eine Alternative zu α, die weniger strenge Annahmen braucht, und wird oft ähnlich interpretiert.</li>
<li><b>Vergleich ohne Umpolen:</b> Ließest du Item 4 unverändert, wäre α nur ,32 und die Trennschärfe von Item 4 negativ (−,60).</li>
</ul>

</section>

{{3}} <section>

<span style="font-size: 1.1em;"><b>So berichtest du das Ergebnis</b></span>

<div style="border-left: 6px solid #a74ebd; background: #f6f1fa; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
✍️ <b>Musterbericht (APA):</b><br>
<i>Die Skala Anstrengungsempfinden (4 Items, Antwortskala 1–5, ein Item umgepolt) wies eine gute interne Konsistenz auf (Cronbachs α = ,86).</i>
</div>

<details>
<summary><b>👉 Wie berichte ich es und was tue ich bei niedrigem α?</b></summary>

| Situation | Was tun? |
| :-- | :-- |
| α unter ,70 | Trennschärfen prüfen, negativ gepolte Items kontrollieren, ggf. Items streichen oder die Skala nicht verwenden |
| Item-rest correlation negativ | Item vermutlich nicht umgepolt oder inhaltlich falsch gepolt |
| α über ,95 | Items sind vermutlich inhaltlich sehr ähnlich (Redundanz) |
| Skala mit wenigen Items | α fällt bei wenigen Items niedriger aus, mit zwei Items besser die Korrelation angeben |
| Mehrere Dimensionen | α pro Dimension berechnen, nicht über alle Items zusammen |

</details>

!?[Allgemeine Einführung in JASP](https://youtu.be/golKIhL8eDk)

<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Cronbach (1951); Hayes & Coutts (2020); Moosbrugger & Kelava (2020); Nunnally (1978); JASP Team (2024)
</div>

</section>

---

### Skalenmittelwerte in JASP

<span style="font-size: 1.1em;"><b>Wann brauche ich das?</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">1️⃣</div>
<div style="text-align: center; font-size: 1.1em;"><b>Ein Wert pro Person</b></div>
<div style="font-size: 0.9em;">Aus vier Items wird ein einziger Wert für das Anstrengungsempfinden.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">↩️</div>
<div style="text-align: center; font-size: 1.1em;"><b>Erst umpolen</b></div>
<div style="font-size: 0.9em;">Negativ gepolte Items werden vor der Berechnung umgepolt (6 minus Antwort bei 5 Stufen).</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">➗</div>
<div style="text-align: center; font-size: 1.1em;"><b>Mittelwert oder Summe</b></div>
<div style="font-size: 0.9em;">Der Mittelwert bleibt auf der Antwortskala (1 bis 5) und ist leichter zu deuten.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📊</div>
<div style="text-align: center; font-size: 1.1em;"><b>Weiterrechnen</b></div>
<div style="font-size: 0.9em;">Der Skalenmittelwert wird wie eine metrische Variable weiterverwendet (z. B. t-Test).</div>
</div>

</div>

<div style="border: 2px solid #2a9a50; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
📋 <b>Wirkung auf das Anstrengungsempfinden</b> 📋<br>
Aus den vier Items der Skala <b>Anstrengungsempfinden</b> wird pro Person ein Skalenmittelwert gebildet (1 = geringe, 5 = starke Anstrengung). Danach kannst du ihn zwischen Musik und keiner Musik vergleichen.
</div>

{{1}} <section>

<span style="font-size: 1.1em;"><b>Durchführung in JASP</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📂</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Daten ansehen</b></div>
<div style="font-size: 0.9em;">Datenansicht in JASP öffnen, jede Zeile ist eine Person.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">➕</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Neue Spalte</b></div>
<div style="font-size: 0.9em;">Auf das „+“ rechts neben der letzten Spalte klicken, Namen vergeben (z. B. Item4_umgepolt), „Computed Column“ wählen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">↩️</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Umpolen</b></div>
<div style="font-size: 0.9em;">Formel: <code>6 - Item4</code> (bei einer Skala von 1 bis 5).</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧮</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Mittelwert bilden</b></div>
<div style="font-size: 0.9em;">Weitere neue Spalte „Anstrengung_Skala“ mit der Formel <code>(Item1 + Item2 + Item3 + Item4_umgepolt) / 4</code>.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🏷️</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Skalenniveau</b></div>
<div style="font-size: 0.9em;">Die neue Spalte als „scale“ einstellen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔍</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Prüfen</b></div>
<div style="font-size: 0.9em;">Mit Descriptives kontrollieren: Minimum und Maximum müssen zwischen 1 und 5 liegen.</div>
</div>

</div>

<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> Datenansicht ➜ „+“ ➜ Computed Column (Formel eingeben)</div>
<div style="height: 10px;"></div>

<!-- TODO: Screenshot JASP: Skalenmittelwerte in JASP -->

</section>

{{2}} <section>

<span style="font-size: 1.1em;"><b>Ergebnis lesen</b></span>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Datenansicht (die ersten 4 Personen)</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Person</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Item 1</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Item 2</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Item 3</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Item 4</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Item 4 umgepolt</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Skalenmittelwert</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">1</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">3</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">4</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2,25</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">3</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">3</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">3</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2,50</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">3</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">4</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2,00</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">4</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">1</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">1</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">3</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">3</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">1,75</td></tr>
</table>
</div>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Descriptive Statistics – Skalenmittelwert Anstrengung</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;"></th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">mit Musik</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">ohne Musik</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Valid</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">15</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">15</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Mean</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">2,37</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">3,12</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Std. Deviation</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">0,57</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">0,69</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Minimum</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">1,75</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">1,75</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Maximum</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">3,75</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">4,00</td></tr>
</table>
</div>

<div style="font-size: 0.8em; opacity: 0.7; margin-bottom: 10px;">Fiktive Daten, nachgebaut im Stil der JASP-Ausgabe.</div>

<ul style="font-size: 0.95em;">
<li><b>Kontrollrechnung für Person 1:</b> (2 + 3 + 2 + 2) : 4 = 2,25. Das Ergebnis muss mit der JASP-Spalte übereinstimmen.</li>
<li><b>Gruppenvergleich:</b> Mit Musik liegt der Skalenmittelwert bei 2,37, ohne Musik bei 3,12. Das Anstrengungsempfinden ist mit Musik also niedriger.</li>
<li><b>Wertebereich prüfen:</b> Minimum und Maximum müssen im Bereich der Antwortskala (1 bis 5) liegen. Andernfalls wurde falsch umgepolt oder falsch berechnet.</li>
<li><b>Fehlende Werte:</b> Fehlt bei einer Person ein Item, ergibt die Formel keinen Wert. Lege vorher fest, wie du damit umgehst (z. B. nur Personen mit allen Items oder Mittelwert der vorhandenen Items).</li>
</ul>

</section>

{{3}} <section>

<span style="font-size: 1.1em;"><b>So berichtest du das Ergebnis</b></span>

<div style="border-left: 6px solid #a74ebd; background: #f6f1fa; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
✍️ <b>Musterbericht (APA):</b><br>
<i>Das Anstrengungsempfinden wurde über vier Items (Antwortskala 1–5, ein Item umgepolt; Cronbachs α = ,86) erfasst. Höhere Werte bedeuten stärkeres Anstrengungsempfinden. Mit Musik lag der Skalenmittelwert bei M = 2,37 (SD = 0,57), ohne Musik bei M = 3,12 (SD = 0,69).</i>
</div>

<details>
<summary><b>👉 Wie berichte ich es und worauf muss ich achten?</b></summary>

| Frage | Antwort |
| :-- | :-- |
| Mittelwert oder Summe? | Mittelwert, wenn alle Items dieselbe Skala haben. Der Wert bleibt auf der Antwortskala und ist leichter zu deuten. |
| Darf ich Mittelwerte aus Likert-Items bilden? | Bei mehreren Items und einer geprüften Reliabilität ist das üblich. Einzelne Likert-Items sind streng genommen ordinal. |
| Muss ich α vorher prüfen? | Ja. Erst wenn die Items zuverlässig zusammenpassen, ist ein Skalenmittelwert sinnvoll. |
| Wie polt man bei anderen Skalen um? | (Skalenmaximum + 1) minus Antwort, z. B. bei 1 bis 7: 8 minus Antwort. |

</details>

!?[Allgemeine Einführung in JASP](https://youtu.be/Xa5Hdfb9NBc)

<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Moosbrugger & Kelava (2020); Döring & Bortz (2016); JASP Team (2024)
</div>

</section>

---

### Check-Up: Deskriptive Statistik, Reliabilität und Skalenmittelwerte


<div style="height: 15px;"></div>

**Frage 1:** Wo findest du in JASP die Mittelwerte und Standardabweichungen je Gruppe?

- [(X)] Descriptives ➜ Descriptive Statistics (Variable „Split“)
- [( )] T-Tests ➜ Paired Samples T-Test
- [( )] Frequencies ➜ Contingency Tables
- [( )] Regression ➜ Correlation

<details>
<summary><b>👉 Erklärung</b></summary>

Mit „Split“ trennst du die Kennwerte nach der Gruppenvariable.

</details>

**Frage 2:** Welcher Kennwert passt am besten zur Beschreibung des ordinalen Borg-Werts?

- [( )] Mittelwert
- [(X)] Median
- [( )] Varianz
- [( )] Summe

<details>
<summary><b>👉 Erklärung</b></summary>

Bei ordinalen Daten passt der Median immer.

</details>

**Frage 3:** Was zeigt Cronbachs α?

- [( )] Ob zwei Gruppen sich unterscheiden
- [(X)] Wie stark die Items einer Skala zusammenhängen (interne Konsistenz)
- [( )] Wie groß ein Effekt ist
- [( )] Ob die Daten normalverteilt sind

<details>
<summary><b>👉 Erklärung</b></summary>

α ist ein Maß für die interne Konsistenz einer Skala.

</details>


**Frage 4:** Bei einer Skala von 1 bis 7 hat Item 3 (negativ gepolt) den Wert 2. Welcher umgepolte Wert geht in den Mittelwert ein?

- [( )] 2
- [( )] 5
- [(X)] 6
- [( )] 7

<details>
<summary><b>👉 Erklärung</b></summary>

Umpolen: 8 minus Antwort, also 8 − 2 = 6.

</details>

**Frage 5:** Welche Werte muss der Skalenmittelwert bei einer Skala von 1 bis 5 annehmen können?

- [( )] Nur ganze Zahlen
- [(X)] Werte zwischen 1 und 5
- [( )] Werte zwischen 0 und 1
- [( )] Beliebige Werte

<details>
<summary><b>👉 Erklärung</b></summary>

Der Mittelwert bleibt im Bereich der Antwortskala, Zwischenwerte sind möglich.

</details>

---

### Literatur

* Cronbach, L. J. (1951). Coefficient alpha and the internal structure of tests. <i>Psychometrika, 16</i>(3), 297–334.
* Döring, N. &amp; Bortz, J. (2016). <i>Forschungsmethoden und Evaluation in den Sozial- und Humanwissenschaften</i> (5. Aufl.). Springer.
* Eid, M., Gollwitzer, M. &amp; Schmitt, M. (2017). <i>Statistik und Forschungsmethoden</i> (5. Aufl.). Beltz.
* Hayes, A. F. &amp; Coutts, J. J. (2020). Use omega rather than Cronbach’s alpha for estimating reliability. But… <i>Communication Methods and Measures, 14</i>(1), 1–24.
* JASP Team (2024). <i>JASP</i> (Version 0.19) [Computer software]. https://jasp-stats.org/
* Moosbrugger, H. &amp; Kelava, A. (Hrsg.). (2020). <i>Testtheorie und Fragebogenkonstruktion</i> (3. Aufl.). Springer.
* Nunnally, J. C. (1978). <i>Psychometric theory</i> (2nd ed.). McGraw-Hill.
