 <!--
author: Melina Burmeister
version: 0.0.1
language: de
narrator: Deutsch Female

import:  https://raw.githubusercontent.com/EUF-SpoWis/Wissenschaftliches-Arbeiten/refs/heads/main/config.md

import: https://raw.githubusercontent.com/LiaTemplates/citations/refs/heads/main/README.md

link: https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css

-->

# Style-Book 🎨 

[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/EUF-SpoWis/Wissenschaftliches-Arbeiten/refs/heads/main/Style-Book.md)

| Parameter              | Kursinformationen                                                                                              |
| ---------------------- | -------------------------------------------------------------------------------------------------------------- |
| **Veranstaltung:**     |                                                                                               |
| **Semester:**          |                                                                                             |
| **Hochschule:**        | `Europa-Universität Flensburg`                                                                                 |
| **Inhalte:**           | `Style-Book`                                                                             |
| **Link auf GitHub:**   | https://github.com/EUF-SpoWis/Wissenschaftliches-Arbeiten/blob/main/Style-Book.md     |
| **Autoren:**           | Melina Burmeister                                                                                              |

<section>
## Für Folien mit dem gewissen Etwas

### Hier findest du **Gestaltungselemente zum Kopieren**: Boxen, Tabellen, Aufklappbares, Abbildungen und viels mehr. Damit werden aus langen Stichpunktlisten Folien, durch die man sich gern klickt.

### So ist jeder Beitrag aufgebaut

<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem;">
(0. **Name und Einsatzzweck:** wann lohnt sich das Element?) 
1. **Vorschau:** so sieht es aus.
2. **Code zum Kopieren:** kopieren, einfügen, Text austauschen, fertig.
3. **Anpassen:** an welchen Stellschrauben du drehen kannst (Farbe, Rundung, Abstand).
</div>
</section>

---
## Hervorheben

### Umrandete Box
<section>

#### Beispielsweise für Einleitungen und Kernaussagen, wenn die Folie nur wenig Text hat.

<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem;">
Methoden sind <b>wissenschaftliche Werkzeuge</b> 🛠️.
</div>

**Code zum Kopieren:**

```html
<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem;">
Hier dein Text.
</div>
```

**Anpassen:** Farbe über `#4e66bd`, Rundung über `border-radius`.

#### Mehrere Umrandete Boxen könnten so auch für Aufzählungen genutzt werden: 
<div style="border: 2px solid #278f25; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 0.8rem 0;">
  <b style="color: #278f25;">Qualitative Forschung:</b> Beschreibung
</div>

<div style="border: 2px solid #1a9f8d; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 0.8rem 0;">
  <b style="color: #1a9f8d;">Qunatitative Forschung</b> Beschreibung
</div>

<div style="border: 2px solid #643d8d; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 0.8rem 0;">
  <b style="color: #643d8d;">Mixed-Methodes:</b> Beschreibung
</div>
</section>

### Hinweisbox
<section>

#### Tipp, Achtung, Merke

<div style="border-left: 6px solid #2e9e5b; background: rgba(46,158,91,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
💡 <b>Tipp:</b> Hier dein Text.
</div>

<div style="border-left: 6px solid #e08a1e; background: rgba(224,138,30,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
⚠️ <b>Achtung:</b> Hier dein Text.
</div>

<div style="border-left: 6px solid #4e66bd; background: rgba(78,102,189,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
📌 <b>Merke:</b> Hier dein Text.
</div>

**Code zum Kopieren:**

```html
<div style="border-left: 6px solid #2e9e5b; background: rgba(46,158,91,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
💡 <b>Tipp:</b> Hier dein Text.
</div>
```

```html
<div style="border-left: 6px solid #e08a1e; background: rgba(224,138,30,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
⚠️ <b>Achtung:</b> Hier dein Text.
</div>
```

```html
<div style="border-left: 6px solid #4e66bd; background: rgba(78,102,189,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
📌 <b>Merke:</b> Hier dein Text.
</div>
```

**Anpassen:** Farbe der Box jeweils über `#2e9e5b`, `#e08a1e`, `4e66bd`. Farbe der Seitenleiste jeweils über `rgba(46,158,91,0.12)`, `rgba(224,138,30,0.12)`, `rgba(78,102,189,0.12)` 
</section>

### Merksatz mit Seitenstrich
<section>

#### Schlichter als eine Box, gut für Definitionen

<div style="border-left: 6px solid #4e66bd; background: #f2f6fb; border-radius: 0 12px 12px 0; padding: 1rem 1.4rem; margin: 1rem 0;">
Der zentrale Forschungsauftrag der qualitativen Forschung ist die <b>Rekonstruktion von Sinn, subjektiven Sichtweisen, Alltagstheorien und Bedeutungskonstruktionen</b> <small>(Helfferich, 2011)</small>.
</div>

**Code zum Kopieren:**

```html
<div style="border-left: 6px solid #4e66bd; background: #f2f6fb; border-radius: 0 12px 12px 0; padding: 1rem 1.4rem; margin: 1rem 0;">
Hier dein Text</b> <small>(hier ggf. deine Quelle)</small>.
</div>
```

**Anpassen:** Fabe des Seitenstrichs über `#4e66bd` und Hintergrundfarbe über `#f2f6fb`.
</section>

### Zitatkasten
<section>

#### Beispielsweise für Aussagen aus Studien, einschlägiger Literatur etc. 

<div style="border-left: 4px solid #4e66bd; padding: 0.3rem 1.2rem; font-style: italic;">
„Hier steht das Zitat."
<div style="font-style: normal; font-size: 0.85em; opacity: 0.7; margin-top: 0.4rem;">
– Quelle, Jahr
</div>
</div>

**Code zum Kopieren:**

```html
<div style="border-left: 4px solid #4e66bd; padding: 0.3rem 1.2rem; font-style: italic;">
„Hier steht das Zitat."
<div style="font-style: normal; font-size: 0.85em; opacity: 0.7; margin-top: 0.4rem;">
– Quelle, Jahr
</div>
</div>
```

**Anpassen:** Farbe des Stirchs an der Seite über `#4e66bd`. Die Quellenzeile kann einfach gelöscht werden, falls sie nicht benötigt wird. 
</section>

### Marker-Effekt
<section>

#### Das ist ein Inline-Element, also mitten im Satz einsetzbar.
Methoden sind <span style="background: linear-gradient(transparent 55%, rgba(255,215,0,0.55) 100%);">wissenschaftliche Werkzeuge</span>.
Methoden sind <span style="background: linear-gradient(transparent 55%, rgba(13, 255, 0, 0.55) 60%);">wissenschaftliche Werkzeuge</span>.
Methoden sind <span style="background: linear-gradient(transparent 55%, rgba(255, 81, 0, 0.55) 5%);">wissenschaftliche Werkzeuge</span>.

**Code zum Kopieren:**

```html
Unmarkierter Textabschnitt <span style="background: linear-gradient(transparent 55%, rgba(255,215,0,0.55) 100%);">Textabschnitt der markiert werden soll</span>. Hier kann es mit einem unmarkierten Teil weitergehen.
```

**Anpassen:** Die Farbe steckt in `rgba(255,215,0,0.55)` (Gelb). Die Zahl `100%` bestimmt, wie hoch der Marker reicht. Kleiner heißt höher, größer heißt schmaler Streifen unten. Ein einfacheres Gelb bekommst du auch mit `<mark>`Text`</mark>`, das ist aber im dunklen Theme oft zu grell.
</section>

### Badge / Label
<section>

#### Das ist ein Inline-Element, also mitten im Satz einsetzbar. Nützlich beispielsweise als kleine Etiketten wie „Neu“, „Wichtig“, „Wiederholung“. 
<span style="background: #4e66bd; color: white; border-radius: 999px; padding: 0.1rem 0.7rem; font-size: 0.8em; font-weight: bold;">Neu</span> Etwas Neues. 
<span style="background: #bd4e4e; color: white; border-radius: 999px; padding: 0.1rem 0.7rem; font-size: 0.8em; font-weight: bold;">Wichtig</span> Etwas Wichtiges.
<span style="background: #4ebd68; color: white; border-radius: 999px; padding: 0.1rem 0.7rem; font-size: 0.8em; font-weight: bold;">Wiederholung</span> Etwas Wiederholendes.

**Code zum Kopieren**: 
```html
<span style="background: #4e66bd; color: white; border-radius: 999px; padding: 0.1rem 0.7rem; font-size: 0.8em; font-weight: bold;">Neu</span> Etwas Neues.
```
```html
<span style="background: #bd4e4e; color: white; border-radius: 999px; padding: 0.1rem 0.7rem; font-size: 0.8em; font-weight: bold;">Wichtig</span> Etwas Wichtiges.
```
```html
<span style="background: #4ebd68; color: white; border-radius: 999px; padding: 0.1rem 0.7rem; font-size: 0.8em; font-weight: bold;">Wiederholung</span> Etwas Wiederholendes.
```

**Anpassen:** Farbe jeweils über `#4e66bd`, `#bd4e4e`, `#4ebd68`. Mit `border-radius: 6px` statt `999px` wird es eckiger statt pillenförmig.
</section>

## Anordnen

### Trennlinien

Abschnitt 1 

<hr style="border: none; border-top: 2px solid #4e66bd; margin: 1.5rem 0;">

Abschnitt 2

<hr style="border: none; height: 2px; background: linear-gradient(to right, transparent, #4e66bd, transparent); margin: 1.5rem 0;">

Abschnitt 3

**Code zum Kopieren**:

```html
Abschnitt 1 

<hr style="border: none; border-top: 2px solid #4e66bd; margin: 1.5rem 0;">

Abschnitt 2

<hr style="border: none; height: 2px; background: linear-gradient(to right, transparent, #4e66bd, transparent); margin: 1.5rem 0;">

Abschnitt 3
```

### Zwei Spalten Links-Rechts

<div style="display: flex; gap: 1.5rem; align-items: center; flex-wrap: wrap;">

<div style="flex: 1; min-width: 220px;">
Hier dein Text links.
</div>

<div style="flex: 1; min-width: 220px;">
<img src="img\Interviewsituation.jpg" style="max-width: 100%; border-radius: 8px;">
</div>

</div>

**Code zum Kopieren**:

```html
<div style="display: flex; gap: 1.5rem; align-items: center; flex-wrap: wrap;">

<div style="flex: 1; min-width: 220px;">
Hier dein Text links.
</div>

<div style="flex: 1; min-width: 220px;">
<img src="Hier Video/Bild/Medie einfügen" style="max-width: 100%; border-radius: 8px;">
</div>

</div>
```

### Kacheln/Karten
<section>

#### Nach Wunsch, können die jeweiligen Zeilen (Emoji, Überschrift, Text) gelöscht oder vertauscht werden.

**Varainte 1: Ohne Animation**

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0; text-align: center;">

  <div style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">🧑</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>

  <div style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">📝</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>

  <div style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">🔍</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>

  <div style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">🏡</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>

  <div style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">🧩</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>
</div>

**Code zum Kopieren**:

```html
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0; text-align: center;">

  <div style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">🧑</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>

  <div style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">📝</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>

  <div style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">🔍</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>

  <div style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">🏡</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>

  <div style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">🧩</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>
</div>
```

**Variante 2: Mit Animation**

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0; text-align: center;">

  <div class="animate__animated animate__fadeInUp" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">🧑</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>

  <div class="animate__animated animate__fadeInUp animate__delay-1s" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">📝</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>

  <div class="animate__animated animate__fadeInUp animate__delay-2s" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">🔍</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>

  <div class="animate__animated animate__fadeInUp animate__delay-3s" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">🏡</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>

  <div class="animate__animated animate__fadeInUp animate__delay-4s" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">🧩</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>
</div>

**Code zum Kopieren**:

```html
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0; text-align: center;">

  <div class="animate__animated animate__fadeInUp" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">🧑</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>

  <div class="animate__animated animate__fadeInUp animate__delay-1s" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">📝</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>

  <div class="animate__animated animate__fadeInUp animate__delay-2s" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">🔍</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>

  <div class="animate__animated animate__fadeInUp animate__delay-3s" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">🏡</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>

  <div class="animate__animated animate__fadeInUp animate__delay-4s" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <div style="font-size: 1.5em; margin-bottom: 5px;">🧩</div>
    <strong style="display: block; margin-bottom: 5px;">Überschrift</strong>
    <span style="font-size: 0.85em; color: #4a5568;">Dein Text.</span>
  </div>
</div>
```
</section>

### Aufklappbare Details
**Eignet sich beispielsweise für Check-Listen, Zusatzinfos, Beispiele etc.**

<details>
<summary>🔍 Klick hier, um ein Beispiel zu sehen</summary>

- Deine "versteckten" Infos

</details>

**Code zum Kopieren**:

```html
<details>
<summary>🔍 Klick hier, um ein Beispiel zu sehen</summary>

- Deine "versteckten" Infos

</details>
```

<b>Frage:</b> Hier steht die Frage.

<details>
<summary>👉 Lösung anzeigen</summary>

Hier steht die Antwort.

</details>

**Code zum Kopieren**:

```html
<b>Frage:</b> Hier steht die Frage.

<details>
<summary>👉 Lösung anzeigen</summary>

Hier steht die Antwort.

</details>
```

### Zeitleiste/Ablaufpfeile

<div style="display: flex; align-items: center; gap: 0.6rem; flex-wrap: wrap;">
<div style="border: 2px solid #8b4ebd; border-radius: 12px; padding: 0.5rem 1rem;">Schritt 1</div>
<span style="font-size: 1.5em;">➜</span>
<div style="border: 2px solid #544ebd; border-radius: 12px; padding: 0.5rem 1rem;">Schritt 2</div>
<span style="font-size: 1.5em;">➜</span>
<div style="border: 2px solid #4eb2bd; border-radius: 12px; padding: 0.5rem 1rem;">Schritt 3</div>
</div>

**Code zum Kopieren**: 

```html
<div style="display: flex; align-items: center; gap: 0.6rem; flex-wrap: wrap;">
<div style="border: 2px solid #8b4ebd; border-radius: 12px; padding: 0.5rem 1rem;">Schritt 1</div>
<span style="font-size: 1.5em;">➜</span>
<div style="border: 2px solid #544ebd; border-radius: 12px; padding: 0.5rem 1rem;">Schritt 2</div>
<span style="font-size: 1.5em;">➜</span>
<div style="border: 2px solid #4eb2bd; border-radius: 12px; padding: 0.5rem 1rem;">Schritt 3</div>
</div>
```

<div style="border-left: 3px solid #4e66bd; padding-left: 1.2rem; margin-left: 0.5rem;">

<div style="margin-bottom: 1rem;">
<b>1. Phase: Titel</b><br>
Hier eine kurze Beschreibung.
</div>

<div style="margin-bottom: 1rem;">
<b>2. Phase: Titel</b><br>
Hier eine kurze Beschreibung.
</div>

<div>
<b>3. Phase: Titel</b><br>
Hier eine kurze Beschreibung.
</div>

</div>

**Code zum Kopieren**: 

```html
<div style="border-left: 3px solid #4e66bd; padding-left: 1.2rem; margin-left: 0.5rem;">

<div style="margin-bottom: 1rem;">
<b>1. Phase: Titel</b><br>
Hier eine kurze Beschreibung.
</div>

<div style="margin-bottom: 1rem;">
<b>2. Phase: Titel</b><br>
Hier eine kurze Beschreibung.
</div>

<div>
<b>3. Phase: Titel</b><br>
Hier eine kurze Beschreibung.
</div>

</div>
```

## Präsentationsübergänge
<div style="border-left: 6px solid #4e66bd; background: #f2f6fb; border-radius: 0 12px 12px 0; padding: 1rem 1.4rem; margin: 1rem 0;">
Um den Elementen in deinen Folien etwas Bewegung zu geben, gibt es verschiedene Animationen zum Ein- und Ausblenden. 
</div>

### Per Klick einblenden
<section>

#### Wie auch im gängigen Powerpointformat, hast du die Möglichkeit, jedes Element per Klick einblenden zu lassen. 

Mit Pfeil rechts bzw. „Weiter" erscheint jeweils der nächste Kasten.

{{1}}
- Schritt 1

{{2}}
- Schritt 2

{{3}}
- Schritt 3

**Code zum Kopieren**: 
```html
{{1}}
- Schritt 1

{{2}}
- Schritt 2

{{3}}
- Schritt 3
```
</section>

### Animation beim Erscheinen der Folie

<div style="background-color:#f0f4f8; border-left: 4px solid #b94655; padding: 12px 16px; border-radius: 4px; margin: 16px 0;">
<span style="background: #bd4e4e; color: white; border-radius: 999px; padding: 0.1rem 0.7rem; font-size: 0.8em; font-weight: bold;">Wichtig</span> Bei den folgenden Animationen handelt es sich um CSS-Datein (animate.css), welche für die Gestaltung von HTML-Seiten gentutz werden. Damit diese in LiaScript reibungslos funktionieren, müssen sie über einen Link im Header verknüft werden. Füge dafür folgende Zeile in deinem Header ein: 
```html
 link: https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css
 ```
</div>

#### Einfaches Einblenden

<!-- class="animate__animated animate__fadeIn" -->
- So lässt du einfach Markdown Elemente erscheinen

<div class="animate__animated animate__fadeIn" style="border-left: 6px solid #4e66bd; background: #f2f6fb; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 0.8rem 0;">
Aber auch html Elemente können eingeblendet werden. 
</div>

**Code zum Kopieren**:
```html
<!-- class="animate__animated animate__fadeIn" -->
- So lässt du einfach Markdown Elemente erscheinen

<div class="animate__animated animate__fadeIn" style="border-left: 6px solid #4e66bd; background: #f2f6fb; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 0.8rem 0;">
Aber auch html Elemente können eingeblendet werden. 
</div>
```

<div style="background-color:#f0f4f8; border-left: 4px solid #b94655; padding: 12px 16px; border-radius: 4px; margin: 16px 0;">
<span style="background: #bd4e4e; color: white; border-radius: 999px; padding: 0.1rem 0.7rem; font-size: 0.8em; font-weight: bold;">Hinweis</span> **Der kleine, aber feine Unterschied für die Animation der Markdown-Elemente und den HTML-Elementen liegt in der Einbindung im Code. Bei Ersterem muss der Animationscode lediglich vor das gewünschte Element gesetzt werden. Für HTML-Elemente wird die Zeile direkt mit in den Code eingebunden (meistens direkt vor den Style-Block).** 
</div>

#### Einblenden von Oben/Unten

<!-- class="animate__animated animate__fadeInUp" -->
> Das hier kommt von oben!

<!-- class="animate__animated animate__fadeInDown" -->
> Das hier kommt von unten!

**Code zum Kopieren**:

```html
<!-- class="animate__animated animate__fadeInUp" -->
> Das hier kommt von oben!

<!-- class="animate__animated animate__fadeInDown" -->
> Das hier kommt von unten!
```

#### Einblenden von Links/Rechts

<!-- class="animate__animated animate__slideInLeft" -->
<div style="border: 2px solid #278f25; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 0.8rem 0;">
  <b style="color: #278f25;">Das hier kommt von Links</b> 
</div>

<!-- class="animate__animated animate__lightSpeedInLeft" -->
<div style="border: 2px solid #278f25; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 0.8rem 0;">
  <b style="color: #278f25;">Das hier kommt von Links, aber etwas schneller</b> 
</div>

<!-- class="animate__animated animate__slideInRight" -->
<div style="border: 2px solid #1a9f8d; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 0.8rem 0;">
  <b style="color: #1a9f8d;">Das hier kommt von Rechts</b> 
</div>

<!-- class="animate__animated animate__lightSpeedInRight" -->
<div style="border: 2px solid #1a9f8d; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 0.8rem 0;">
  <b style="color: #1a9f8d;">Das hier kommt von Rechts, aber etwas schneller</b> 
</div>

**Code zum Kopieren**:

```html
<!-- class="animate__animated animate__slideInLeft" -->
<div style="border: 2px solid #278f25; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 0.8rem 0;">
  <b style="color: #278f25;">Das hier kommt von Links</b> 
</div>

<!-- class="animate__animated animate__lightSpeedInLeft" -->
<div style="border: 2px solid #278f25; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 0.8rem 0;">
  <b style="color: #278f25;">Das hier kommt von Links, aber etwas schneller</b> 
</div>

<!-- class="animate__animated animate__slideInRight" -->
<div style="border: 2px solid #1a9f8d; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 0.8rem 0;">
  <b style="color: #1a9f8d;">Das hier kommt von Rechts</b> 
</div>

<!-- class="animate__animated animate__lightSpeedInRight" -->
<div style="border: 2px solid #1a9f8d; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 0.8rem 0;">
  <b style="color: #1a9f8d;">Das hier kommt von Rechts, aber etwas schneller</b> 
</div>
```

#### Nacheinander einblenden 

<div class="animate__animated animate__fadeIn" style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.7rem 1.2rem; margin: 0.5rem 0;">
Das erscheint sofort.
</div>

<div class="animate__animated animate__fadeIn animate__delay-1s" style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.7rem 1.2rem; margin: 0.5rem 0;">
Das nach 1 Sekunde
</div>

<div class="animate__animated animate__fadeIn animate__delay-2s" style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.7rem 1.2rem; margin: 0.5rem 0;">
Und das dann nach 2 Sekunden
</div>

**Code zum Kopieren**:

```html
<div class="animate__animated animate__fadeIn" style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.7rem 1.2rem; margin: 0.5rem 0;">
Das erscheint sofort.
</div>

<div class="animate__animated animate__fadeIn animate__delay-1s" style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.7rem 1.2rem; margin: 0.5rem 0;">
Das nach 1 Sekunde
</div>

<div class="animate__animated animate__fadeIn animate__delay-2s" style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.7rem 1.2rem; margin: 0.5rem 0;">
Und das dann nach 2 Sekunden
</div>
```

#### Bouncing 

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0; text-align: center;">

  <div class="animate__animated animate__bounceIn" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <strong style="display: block; margin-bottom: 5px;">Diese Karte erscheint mit einem Bounce</strong>
  </div>

</div>

**Code zum Kopieren**:

```html
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0; text-align: center;">

  <div class="animate__animated animate__bounceIn" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <strong style="display: block; margin-bottom: 5px;">Diese Karte erscheint mit einem Bounce</strong>
  </div>

</div>
```

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0; text-align: center;">

  <div class="animate__animated animate__bounceInLeft" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <strong style="display: block; margin-bottom: 5px;">Diese Karte kommt von links mit Schwung</strong>
  </div>

  <div class="animate__animated animate__bounceInRight" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <strong style="display: block; margin-bottom: 5px;">Diese Karte kommt von rechts mit Schwung</strong>
  </div>

</div>

**Code zum Kopieren**:

```html
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0; text-align: center;">

  <div class="animate__animated animate__bounceInLeft" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <strong style="display: block; margin-bottom: 5px;">Diese Karte kommt von links mit Schwung</strong>
  </div>

  <div class="animate__animated animate__bounceInRight" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <strong style="display: block; margin-bottom: 5px;">Diese Karte kommt von rechts mit Schwung</strong>
  </div>

</div>
```

>**Weitere Varianten**: animate__bounceInUp; animate__bounceInDown

#### Zoom

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0; text-align: center;">

  <div class="animate__animated animate__zoomIn" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <strong style="display: block; margin-bottom: 5px;">Diese Karte erscheint mit einem Bounce</strong>
  </div>

</div>

**Code zum Kopieren**:

```html
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0; text-align: center;">

  <div class="animate__animated animate__zoomIn" style="background: #f8fafc; border: 1px solid #e2e8f0; padding: 15px; border-radius: 8px;">
    <strong style="display: block; margin-bottom: 5px;">Diese Karte erscheint mit einem Bounce</strong>
  </div>

</div>
```

#### Flipping

<!-- class="animate__animated animate__flipInX" -->
>Dieses Element erscheint durch ein Aufklappen

<!-- class="animate__animated animate__flipInY" -->
>Dieses Element erscheint mit viel Schwung

**Code zum Kopieren**:

```html
<!-- class="animate__animated animate__flipInX" -->
>Dieses Element erscheint durch ein Aufklappen

<!-- class="animate__animated animate__flipInY" -->
>Dieses Element erscheint mit viel Schwung
```

#### Reinrotieren

<!-- class="animate__animated animate__rollIn" -->
>Wir rotieren aus zwei verschiedenen Richtungen rein

<!-- class="animate__animated animate__rotateIn" -->
>Wir rotieren aus zwei verschiedenen Richtungen rein

**Code zum Kopieren**:

```html
<!-- class="animate__animated animate__rollIn" -->
>Wir rotieren aus zwei verschiedenen Richtungen rein

<!-- class="animate__animated animate__rotateIn" -->
>Wir rotieren aus zwei verschiedenen Richtungen rein
```

<!-- class="animate__animated animate__jackInTheBox"-->
>Hier eine weitere Variante

**Code zum Kopieren**:

```html
<!-- class="animate__animated animate__jackInTheBox"-->
>Hier eine weitere Variante
```

### Zur Betonung von Elementen 

#### Wackeln
<!-- class="animate__animated animate__wobble"-->
>Einfaches Wackeln

<!-- class="animate__animated animate__jello"-->
>Starkes Wackeln

<!-- class="animate__animated animate__swing"-->
>Mittleres Wackeln

<!-- class="animate__animated animate__headShake"-->
>Kleines Wackeln

**Codes zum Kopieren**:
```html
<!-- class="animate__animated animate__wobble"-->
>Einfaches Wackeln
```
```html
<!-- class="animate__animated animate__jello"-->
>Starkes Wackeln
```
```html
<!-- class="animate__animated animate__swing"-->
>Mittleres Wackeln
```
```html
<!-- class="animate__animated animate__headShake"-->
>Kleines Wackeln
```

#### Pulsieren
<!-- class="animate__animated animate__heartBeat"-->
>Einfaches Pulsieren

<!-- class="animate__animated animate__flash"-->
>Aufleuchten

**Codes zum Kopieren**:

```html
<!-- class="animate__animated animate__heartBeat"-->
>Einfaches Pulsieren
```
```html
<!-- class="animate__animated animate__flash"-->
>Aufleuchten
```

## Besondere Abbildungen

### Analyseebenen 

<div style="max-width:720px;margin:1em auto;padding:16px 20px;border:3px solid #1f3a5f;border-radius:10px;background:#e8eef7;color:#1a1a1a;text-align:center;font-family:sans-serif;">

<div style="font-size:1.3em;"><b>MAKROEBENE</b></div>

<div>Gesellschaftliche Teilsysteme</div>

<div style="margin:8px 0 14px 0;"><i>Sport als Teilsystem der Gesellschaft<br>Beziehungen zu Politik, Wirtschaft, Medien u. a.</i></div>

<div style="padding:14px 18px;border:3px solid #2f6b4f;border-radius:10px;background:#e6f2ea;color:#1a1a1a;">

<div style="font-size:1.2em;"><b>MESOEBENE</b></div>

<div>Komplexere soziale Ordnungsmuster</div>

<div style="margin:8px 0 14px 0;"><i>Sportvereine und Verbände<br>Schulen und Hochschulen<br>Teams, Fanszenen, Subkulturen</i></div>

<div style="padding:12px 16px;border:3px solid #9a5b13;border-radius:10px;background:#fbefdc;color:#1a1a1a;">

<div style="font-size:1.1em;"><b>MIKROEBENE</b></div>

<div>Interaktionen in kleineren sozialen Gebilden</div>

<div style="margin-top:8px;"><i>Trainer:in und Athlet:in<br>Lehrkraft und Klasse<br>Mitglieder innerhalb einer formellen/informellen Gruppe</i></div>

</div>

</div>

</div>

**Code zum Kopieren:**

```html
<div style="max-width:720px;margin:1em auto;padding:16px 20px;border:3px solid #1f3a5f;border-radius:10px;background:#e8eef7;color:#1a1a1a;text-align:center;font-family:sans-serif;">

<div style="font-size:1.3em;"><b>MAKROEBENE</b></div>

<div>Gesellschaftliche Teilsysteme</div>

<div style="margin:8px 0 14px 0;"><i>Sport als Teilsystem der Gesellschaft<br>Beziehungen zu Politik, Wirtschaft, Medien u. a.</i></div>

<div style="padding:14px 18px;border:3px solid #2f6b4f;border-radius:10px;background:#e6f2ea;color:#1a1a1a;">

<div style="font-size:1.2em;"><b>MESOEBENE</b></div>

<div>Komplexere soziale Ordnungsmuster</div>

<div style="margin:8px 0 14px 0;"><i>Sportvereine und Verbände<br>Schulen und Hochschulen<br>Teams, Fanszenen, Subkulturen</i></div>

<div style="padding:12px 16px;border:3px solid #9a5b13;border-radius:10px;background:#fbefdc;color:#1a1a1a;">

<div style="font-size:1.1em;"><b>MIKROEBENE</b></div>

<div>Interaktionen in kleineren sozialen Gebilden</div>

<div style="margin-top:8px;"><i>Trainer:in und Athlet:in<br>Lehrkraft und Klasse<br>Mitglieder innerhalb einer formellen/informellen Gruppe</i></div>

</div>

</div>

</div>
```

**Anpassen:** Die Farben der einzelnen Ebenen können jeweils über `#1f3a5f`, `#2f6b4f`, `#9a5b13` geändert werden. Natürlich kann auch der Text innerhalb der Abbildung geändert werden, sodass inhaltlich Spielraum für verschiedene Ebenen-Darstellungen ist.  

### Phasendiagramm

(Hier am Beispiel des methodischen Spektrums)

**Variante 1: Ohne Animation**

<div style="position: relative; margin: 30px 0 60px 0;">

  <div style="display: flex; gap: 15px; justify-content: space-between; align-items: center; flex-wrap: wrap;">

    <div style="flex: 1; min-width: 200px; background: #f0f4f8; border-left: 5px solid #2b6cb0; padding: 15px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.05);">
      <strong style="color: #2b6cb0; font-size: 1.1em; display: block; margin-bottom: 5px;">1. Datenerhebung</strong>
      <span style="font-size: 0.9em; color: #4a5568;">z. B. Leitfadeninterviews, teilnehmende/nicht-teilnehmende Beobachtungen</span>
    </div>

    <div style="font-size: 1.5em; color: #a0aec0; font-weight: bold;">➔</div>

    <div style="flex: 1; min-width: 200px; background: #f0f4f8; border-left: 5px solid #2b6cb0; padding: 15px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.05);">
      <strong style="color: #2b6cb0; font-size: 1.1em; display: block; margin-bottom: 5px;">2. Datenaufbereitung</strong>
      <span style="font-size: 0.9em; color: #4a5568;">z. B. Transkription, Anonymisierung, Erstellung des Feldporträts</span>
    </div>

    <div style="font-size: 1.5em; color: #a0aec0; font-weight: bold;">➔</div>

    <div style="flex: 1; min-width: 200px; background: #f0f4f8; border-left: 5px solid #2b6cb0; padding: 15px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.05);">
      <strong style="color: #2b6cb0; font-size: 1.1em; display: block; margin-bottom: 5px;">3. Analyse & Interpretation</strong>
      <span style="font-size: 0.9em; color: #4a5568;">z. B. Kodierung, Typenbildung</span>
    </div>

  </div>

  <div style="position: absolute; right: 5%; left: 5%; bottom: -35px; height: 30px;">
    <svg width="100%" height="100%" viewBox="0 0 500 40" fill="none" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none">
      <path d="M 480 5 C 480 35, 20 35, 20 12" stroke="#2b6cb0" stroke-width="2" stroke-dasharray="4 3" fill="none" />
      <polygon points="15,14 20,4 25,14" fill="#2b6cb0" />
    </svg>
    <span style="position: absolute; bottom: -14px; left: 50%; transform: translateX(-50%); background: #ffffff; padding: 0 8px; font-size: 0.75em; color: #2b6cb0; font-weight: bold; border-radius: 4px;">
      evtl. zirkulärer Re-Analyseprozess
    </span>
  </div>

</div>

**Code zum Kopieren**:

```html
<div style="position: relative; margin: 30px 0 60px 0;">

  <div style="display: flex; gap: 15px; justify-content: space-between; align-items: center; flex-wrap: wrap;">

    <div style="flex: 1; min-width: 200px; background: #f0f4f8; border-left: 5px solid #2b6cb0; padding: 15px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.05);">
      <strong style="color: #2b6cb0; font-size: 1.1em; display: block; margin-bottom: 5px;">1. Datenerhebung</strong>
      <span style="font-size: 0.9em; color: #4a5568;">z. B. Leitfadeninterviews, teilnehmende/nicht-teilnehmende Beobachtungen</span>
    </div>

    <div style="font-size: 1.5em; color: #a0aec0; font-weight: bold;">➔</div>

    <div style="flex: 1; min-width: 200px; background: #f0f4f8; border-left: 5px solid #2b6cb0; padding: 15px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.05);">
      <strong style="color: #2b6cb0; font-size: 1.1em; display: block; margin-bottom: 5px;">2. Datenaufbereitung</strong>
      <span style="font-size: 0.9em; color: #4a5568;">z. B. Transkription, Anonymisierung, Erstellung des Feldporträts</span>
    </div>

    <div style="font-size: 1.5em; color: #a0aec0; font-weight: bold;">➔</div>

    <div style="flex: 1; min-width: 200px; background: #f0f4f8; border-left: 5px solid #2b6cb0; padding: 15px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.05);">
      <strong style="color: #2b6cb0; font-size: 1.1em; display: block; margin-bottom: 5px;">3. Analyse & Interpretation</strong>
      <span style="font-size: 0.9em; color: #4a5568;">z. B. Kodierung, Typenbildung</span>
    </div>

  </div>

  <div style="position: absolute; right: 5%; left: 5%; bottom: -35px; height: 30px;">
    <svg width="100%" height="100%" viewBox="0 0 500 40" fill="none" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none">
      <path d="M 480 5 C 480 35, 20 35, 20 12" stroke="#2b6cb0" stroke-width="2" stroke-dasharray="4 3" fill="none" />
      <polygon points="15,14 20,4 25,14" fill="#2b6cb0" />
    </svg>
    <span style="position: absolute; bottom: -14px; left: 50%; transform: translateX(-50%); background: #ffffff; padding: 0 8px; font-size: 0.75em; color: #2b6cb0; font-weight: bold; border-radius: 4px;">
      evtl. zirkulärer Re-Analyseprozess
    </span>
  </div>

</div>
```

**Variante 2: Mit bereits eingefügten Animationen** 

<div style="position: relative; margin: 30px 0 60px 0;">

  <div style="display: flex; gap: 15px; justify-content: space-between; align-items: center; flex-wrap: wrap;">

    <div class="animate__animated animate__fadeInUp" style="flex: 1; min-width: 200px; background: #f0f4f8; border-left: 5px solid #2b6cb0; padding: 15px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.05);">
      <strong style="color: #2b6cb0; font-size: 1.1em; display: block; margin-bottom: 5px;">1. Datenerhebung</strong>
      <span style="font-size: 0.9em; color: #4a5568;">z. B. Leitfadeninterviews, teilnehmende/nicht-teilnehmende Beobachtungen</span>
    </div>

    <div class="animate__animated animate__fadeInUp animate__delay-1s" style="font-size: 1.5em; color: #a0aec0; font-weight: bold;">➔</div>

    <div class="animate__animated animate__fadeInUp animate__delay-1s" style="flex: 1; min-width: 200px; background: #f0f4f8; border-left: 5px solid #2b6cb0; padding: 15px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.05);">
      <strong style="color: #2b6cb0; font-size: 1.1em; display: block; margin-bottom: 5px;">2. Datenaufbereitung</strong>
      <span style="font-size: 0.9em; color: #4a5568;">z. B. Transkription, Anonymisierung, Erstellung des Feldporträts</span>
    </div>

    <div class="animate__animated animate__fadeInUp animate__delay-2s" style="font-size: 1.5em; color: #a0aec0; font-weight: bold;">➔</div>

    <div class="animate__animated animate__fadeInUp animate__delay-2s" style="flex: 1; min-width: 200px; background: #f0f4f8; border-left: 5px solid #2b6cb0; padding: 15px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.05);">
      <strong style="color: #2b6cb0; font-size: 1.1em; display: block; margin-bottom: 5px;">3. Analyse & Interpretation</strong>
      <span style="font-size: 0.9em; color: #4a5568;">z. B. Kodierung, Typenbildung</span>
    </div>

  </div>

  <div style="position: absolute; right: 5%; left: 5%; bottom: -35px; height: 30px;">
    <svg width="100%" height="100%" viewBox="0 0 500 40" fill="none" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none">
      <path d="M 480 5 C 480 35, 20 35, 20 12" stroke="#2b6cb0" stroke-width="2" stroke-dasharray="4 3" fill="none" />
      <polygon points="15,14 20,4 25,14" fill="#2b6cb0" />
    </svg>
    <span style="position: absolute; bottom: -14px; left: 50%; transform: translateX(-50%); background: #ffffff; padding: 0 8px; font-size: 0.75em; color: #2b6cb0; font-weight: bold; border-radius: 4px;">
      evtl. zirkulärer Re-Analyseprozess
    </span>
  </div>

</div>


**Code zum Kopieren**: 

```html
<div style="position: relative; margin: 30px 0 60px 0;">

  <div style="display: flex; gap: 15px; justify-content: space-between; align-items: center; flex-wrap: wrap;">

    <div class="animate__animated animate__fadeInUp" style="flex: 1; min-width: 200px; background: #f0f4f8; border-left: 5px solid #2b6cb0; padding: 15px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.05);">
      <strong style="color: #2b6cb0; font-size: 1.1em; display: block; margin-bottom: 5px;">1. Datenerhebung</strong>
      <span style="font-size: 0.9em; color: #4a5568;">z. B. Leitfadeninterviews, teilnehmende/nicht-teilnehmende Beobachtungen</span>
    </div>

    <div class="animate__animated animate__fadeInUp animate__delay-1s" style="font-size: 1.5em; color: #a0aec0; font-weight: bold;">➔</div>

    <div class="animate__animated animate__fadeInUp animate__delay-1s" style="flex: 1; min-width: 200px; background: #f0f4f8; border-left: 5px solid #2b6cb0; padding: 15px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.05);">
      <strong style="color: #2b6cb0; font-size: 1.1em; display: block; margin-bottom: 5px;">2. Datenaufbereitung</strong>
      <span style="font-size: 0.9em; color: #4a5568;">z. B. Transkription, Anonymisierung, Erstellung des Feldporträts</span>
    </div>

    <div class="animate__animated animate__fadeInUp animate__delay-2s" style="font-size: 1.5em; color: #a0aec0; font-weight: bold;">➔</div>

    <div class="animate__animated animate__fadeInUp animate__delay-2s" style="flex: 1; min-width: 200px; background: #f0f4f8; border-left: 5px solid #2b6cb0; padding: 15px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.05);">
      <strong style="color: #2b6cb0; font-size: 1.1em; display: block; margin-bottom: 5px;">3. Analyse & Interpretation</strong>
      <span style="font-size: 0.9em; color: #4a5568;">z. B. Kodierung, Typenbildung</span>
    </div>

  </div>

  <div style="position: absolute; right: 5%; left: 5%; bottom: -35px; height: 30px;">
    <svg width="100%" height="100%" viewBox="0 0 500 40" fill="none" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none">
      <path d="M 480 5 C 480 35, 20 35, 20 12" stroke="#2b6cb0" stroke-width="2" stroke-dasharray="4 3" fill="none" />
      <polygon points="15,14 20,4 25,14" fill="#2b6cb0" />
    </svg>
    <span style="position: absolute; bottom: -14px; left: 50%; transform: translateX(-50%); background: #ffffff; padding: 0 8px; font-size: 0.75em; color: #2b6cb0; font-weight: bold; border-radius: 4px;">
      evtl. zirkulärer Re-Analyseprozess
    </span>
  </div>

</div>
```

### Mind-Map Style 

(Hier am Beispiel einer Übersicht über verschiedene Interviewarten)

**Variante 1: Ohne Animation**

<div style="position: relative; width: 100%; max-width: 680px; height: 360px; margin: 20px auto; font-family: sans-serif;">

  <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); width: 120px; height: 120px; border-radius: 50%; background-color: #ffffff; border: 3px solid #cbd5e1; display: flex; flex-direction: column; align-items: center; justify-content: center; box-shadow: 0 8px 20px rgba(0,0,0,0.08); z-index: 10;">
    <span style="font-size: 34px;">🎙️</span>
    <strong style="font-size: 13px; color: #334155; margin-top: 2px;">Interviews</strong>
  </div>

  <div style="position: absolute; top: 8%; left: 14%; width: 210px; height: 55px; background-color: #fef08a; color: #854d0e; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #fde047; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Leitfadengestütztes Interview
  </div>

  <div style="position: absolute; top: 8%; right: 14%; width: 210px; height: 55px; background-color: #e9d5ff; color: #6b21a8; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #d8b4fe; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Narratives Interview
  </div>

  <div style="position: absolute; top: 50%; left: 2%; transform: translateY(-50%); width: 240px; height: 65px; background-color: #bbf7d0; color: #166534; font-weight: 600; border-radius: 30px; font-size: 12px; border: 1px solid #86efac; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px; line-height: 1.2;">
    Fokussiertes / Problemzentriertes Interview
  </div>

  <div style="position: absolute; top: 50%; right: 2%; transform: translateY(-50%); width: 210px; height: 55px; background-color: #fed7aa; color: #9a3412; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #fdba74; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Episodisches Interview
  </div>

  <div style="position: absolute; bottom: 8%; left: 14%; width: 210px; height: 55px; background-color: #bfdbfe; color: #1e40af; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #93c5fd; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Expert:inneninterview
  </div>

  <div style="position: absolute; bottom: 8%; right: 14%; width: 210px; height: 55px; background-color: #fbcfe8; color: #9d174d; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #f9a8d4; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Gruppendiskussion / Fokusgruppe
  </div>

</div>

**Code zum Kopieren**
```html
<div style="position: relative; width: 100%; max-width: 680px; height: 360px; margin: 20px auto; font-family: sans-serif;">

  <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); width: 120px; height: 120px; border-radius: 50%; background-color: #ffffff; border: 3px solid #cbd5e1; display: flex; flex-direction: column; align-items: center; justify-content: center; box-shadow: 0 8px 20px rgba(0,0,0,0.08); z-index: 10;">
    <span style="font-size: 34px;">🎙️</span>
    <strong style="font-size: 13px; color: #334155; margin-top: 2px;">Interviews</strong>
  </div>

  <div style="position: absolute; top: 8%; left: 14%; width: 210px; height: 55px; background-color: #fef08a; color: #854d0e; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #fde047; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Leitfadengestütztes Interview
  </div>

  <div style="position: absolute; top: 8%; right: 14%; width: 210px; height: 55px; background-color: #e9d5ff; color: #6b21a8; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #d8b4fe; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Narratives Interview
  </div>

  <div style="position: absolute; top: 50%; left: 2%; transform: translateY(-50%); width: 240px; height: 65px; background-color: #bbf7d0; color: #166534; font-weight: 600; border-radius: 30px; font-size: 12px; border: 1px solid #86efac; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px; line-height: 1.2;">
    Fokussiertes / Problemzentriertes Interview
  </div>

  <div style="position: absolute; top: 50%; right: 2%; transform: translateY(-50%); width: 210px; height: 55px; background-color: #fed7aa; color: #9a3412; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #fdba74; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Episodisches Interview
  </div>

  <div style="position: absolute; bottom: 8%; left: 14%; width: 210px; height: 55px; background-color: #bfdbfe; color: #1e40af; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #93c5fd; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Expert:inneninterview
  </div>

  <div style="position: absolute; bottom: 8%; right: 14%; width: 210px; height: 55px; background-color: #fbcfe8; color: #9d174d; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #f9a8d4; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Gruppendiskussion / Fokusgruppe
  </div>

</div>
```

**Varainte 2: Mit Animationen**

<div style="position: relative; width: 100%; max-width: 680px; height: 360px; margin: 20px auto; font-family: sans-serif;">

  <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); width: 120px; height: 120px; border-radius: 50%; background-color: #ffffff; border: 3px solid #cbd5e1; display: flex; flex-direction: column; align-items: center; justify-content: center; box-shadow: 0 8px 20px rgba(0,0,0,0.08); z-index: 10;">
    <span style="font-size: 34px;">🎙️</span>
    <strong style="font-size: 13px; color: #334155; margin-top: 2px;">Interviews</strong>
  </div>

  <div class="animate__animated animate__slideInLeft" style="position: absolute; top: 8%; left: 14%; width: 210px; height: 55px; background-color: #fef08a; color: #854d0e; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #fde047; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Leitfadengestütztes Interview
  </div>

  <div class="animate__animated animate__slideInRight" style="position: absolute; top: 8%; right: 14%; width: 210px; height: 55px; background-color: #e9d5ff; color: #6b21a8; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #d8b4fe; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Narratives Interview
  </div>

  <div class="animate__animated animate__slideInLeft" style="position: absolute; top: 50%; left: 2%; transform: translateY(-50%); width: 240px; height: 65px; background-color: #bbf7d0; color: #166534; font-weight: 600; border-radius: 30px; font-size: 12px; border: 1px solid #86efac; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px; line-height: 1.2;">
    Fokussiertes / Problemzentriertes Interview
  </div>

  <div class="animate__animated animate__slideInRight" style="position: absolute; top: 50%; right: 2%; transform: translateY(-50%); width: 210px; height: 55px; background-color: #fed7aa; color: #9a3412; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #fdba74; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Episodisches Interview
  </div>

  <div class="animate__animated animate__slideInLeft" style="position: absolute; bottom: 8%; left: 14%; width: 210px; height: 55px; background-color: #bfdbfe; color: #1e40af; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #93c5fd; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Expert:inneninterview
  </div>

  <div class="animate__animated animate__slideInRight" style="position: absolute; bottom: 8%; right: 14%; width: 210px; height: 55px; background-color: #fbcfe8; color: #9d174d; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #f9a8d4; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Gruppendiskussion / Fokusgruppe
  </div>

</div>

**Code zum Kopieren**

```html
<div style="position: relative; width: 100%; max-width: 680px; height: 360px; margin: 20px auto; font-family: sans-serif;">

  <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); width: 120px; height: 120px; border-radius: 50%; background-color: #ffffff; border: 3px solid #cbd5e1; display: flex; flex-direction: column; align-items: center; justify-content: center; box-shadow: 0 8px 20px rgba(0,0,0,0.08); z-index: 10;">
    <span style="font-size: 34px;">🎙️</span>
    <strong style="font-size: 13px; color: #334155; margin-top: 2px;">Interviews</strong>
  </div>

  <div class="animate__animated animate__slideInLeft" style="position: absolute; top: 8%; left: 14%; width: 210px; height: 55px; background-color: #fef08a; color: #854d0e; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #fde047; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Leitfadengestütztes Interview
  </div>

  <div class="animate__animated animate__slideInRight" style="position: absolute; top: 8%; right: 14%; width: 210px; height: 55px; background-color: #e9d5ff; color: #6b21a8; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #d8b4fe; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Narratives Interview
  </div>

  <div class="animate__animated animate__slideInLeft" style="position: absolute; top: 50%; left: 2%; transform: translateY(-50%); width: 240px; height: 65px; background-color: #bbf7d0; color: #166534; font-weight: 600; border-radius: 30px; font-size: 12px; border: 1px solid #86efac; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px; line-height: 1.2;">
    Fokussiertes / Problemzentriertes Interview
  </div>

  <div class="animate__animated animate__slideInRight" style="position: absolute; top: 50%; right: 2%; transform: translateY(-50%); width: 210px; height: 55px; background-color: #fed7aa; color: #9a3412; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #fdba74; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Episodisches Interview
  </div>

  <div class="animate__animated animate__slideInLeft" style="position: absolute; bottom: 8%; left: 14%; width: 210px; height: 55px; background-color: #bfdbfe; color: #1e40af; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #93c5fd; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Expert:inneninterview
  </div>

  <div class="animate__animated animate__slideInRight" style="position: absolute; bottom: 8%; right: 14%; width: 210px; height: 55px; background-color: #fbcfe8; color: #9d174d; font-weight: 600; border-radius: 28px; font-size: 12px; border: 1px solid #f9a8d4; box-shadow: 0 4px 6px rgba(0,0,0,0.04); display: flex; align-items: center; justify-content: center; text-align: center; padding: 0 12px;">
    Gruppendiskussion / Fokusgruppe
  </div>

</div>
```

## Für Details 