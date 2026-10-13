# Style-Book 🎨  
<section>

## Für Folien mit dem gewissen Etwas

Hier findest du **Gestaltungselemente zum Kopieren**: Boxen, Tabellen, Aufklappbares, Abbildungen und viels mehr. Damit werden aus langen Stichpunktlisten Folien, durch die man sich gern klickt.

<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem;">
Jedes Element ist <b>kurz erklärt</b>, hat eine <b>Vorschau</b> und einen <b>Code zum Kopieren</b> 📋.
</div>

### So ist jeder Beitrag aufgebaut

1. **Name und Einsatzzweck:** wann lohnt sich das Element?
2. **Vorschau:** so sieht es aus.
3. **Code zum Kopieren:** kopieren, einfügen, Text austauschen, fertig.
4. **Anpassen:** an welchen Stellschrauben du drehen kannst (Farbe, Rundung, Abstand).
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

## Aufklappen und Enthüllen

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

## Für Details 