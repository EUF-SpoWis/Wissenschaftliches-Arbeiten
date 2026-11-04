<!--
author: Tjari Klimpki
version: 0.0.1
language: de
narrator: Deutsch Female

import:  https://raw.githubusercontent.com/EUF-SpoWis/Wissenschaftliches-Arbeiten/refs/heads/main/config.md

import: https://raw.githubusercontent.com/LiaTemplates/citations/refs/heads/main/README.md

link: https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css

-->
[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/EUF-SpoWis/Wissenschaftliches-Arbeiten/refs/heads/main/02_Qualitative_Inhaltsanalyse.md)

# Das Beispielinterview

Dieses Interview begleitet dich durch den gesamten Kurs. Schau dich zuerst in Ruhe um, bevor wir anfangen zu codieren.

So kannst du das Transkript erkunden:

- Klicke in der **Übersichtsleiste** auf einen Abschnitt, um nur diesen Teil zu sehen.
- Die **Zeilennummern** helfen dir beim Zitieren und Vergleichen (z. B. "Z. 17").
- Mit **Nur Aussagen des Kindes** blendest du die Fragen der Interviewerin aus.
- Die **Suche** markiert alle Stellen mit einem Begriff, z. B. "Trainer" oder "Gruppe".

<div id="tv-widget"></div>

<script>
// ============================================================
// 1) DATEN: Metadaten und Transkript
// ============================================================
var META = [
  ['Kind', '14 Jahre, Volleyball'],
  ['Datum', '29.07.2026, 11:20'],
  ['Dauer', '23:05 Minuten'],
  ['Form', 'Nicht-standardisiertes Leitfadeninterview']
];
var FRAGE = 'Welche Bedingungen und Handlungen erleben Kinder im Training als förderlich für ihr eigenes Kompetenzerleben?';

// HIER das komplette Transkript einfügen (ersetzt den Beispieltext).
// Format: Abschnittsüberschriften in eckigen Klammern, die mit
// Einstiegsphase, Themenblock oder Ausklang beginnen.
// Sprecherzeilen mit S1: oder S2:. Andere Zeilen in eckigen Klammern
// werden als Regieanweisung dargestellt.
var RAW = `
[Einstiegsphase, Warm-up]
S1: Dann heiße ich dich hiermit nochmal ganz offiziell herzlich Willkommen. Vielen Dank, dass du dir die Zeit genommen hast, heute mit mir zu sprechen! Ich würde ja heute gerne etwas mehr über dein Volleyball-Training hier im <Vereinsname> erfahren. Magst du mir zuerst aber mal erzählen, wie du überhaupt zum Volleyball gekommen bist?
S2: Mhm. Also meine Schwester hat das schon gespielt ähm, und dann bin ich einfach mal mitgegangen zum Training, und dann hat's mir gefallen und ich bin geblieben. 
S1: Ah, so ist das. Und wie lange spielst du schon Volleyball? 
S2: Seit zwei Jahren ungefähr.
S1: Das ist ja schon eine lange Zeit. Was gefällt dir denn so daran?
S2: Am meisten mag ich's, wenn wir richtige Spiele gegeneinander machen. Das äh (.) ist immer cool. 
S1:Ja, das ist echt cool. Spielst du denn auch manchmal mit deiner Schwester zusammen?
S2: Ähm (--) nee, nicht wirklich. Also (--) ich meine, hier im Training nicht, weil sie ist ja in einer anderen Gruppe. Aber sonnst spielen wir oft im Garten bei uns oder auch ähm (.) so im Urlaub am Strand. Hier beim richtigen Training macht es mir aber mehr Spaß, weil wir dann ja auch richtige Spiele machen können und nicht nur so hin und her wie zu zweit.
S1: Mhm, verstehe. Dann lass und doch gerne mal genauer über dein Training im Verein sprechen. 
S2: Okay.

[Themenblock 1: Trainer*innenverhalten]
S1: Mich würde erstmal interessieren, wie so ein ganz normales Training bei euch abläuft. So von Anfang bis Ende.
S2: Mh (--) also wir machen immer erst Aufwärmen, so Laufen und Dehnen und so. Und dann zeigt uns der Trainer meistens irgendeine neue Übung oder wir machen halt Übungen, die wir schon kennen. Dann am Ende äh (.) spielen wir meistens noch so richtig gegeneinander. 
S1: Ah okay. Also der Trainer zeigt euch Sachen? Ich kann mir das nicht ganz so gut vorstellen, wie das genau abläuft. Kannst du mir das vielleicht nochmal genauer erklären?
S2: Also meistens stehen wir nach dem Aufwärmen alle so in einem Kreis halt. Und ähm (.) der Trainer macht dann eine Ansage, welche Übung wir machen. Wenn wir die noch gar nicht kennen, dann macht er das einmal vor wie das geht. Manchmal braucht er da auch Hilfe, weil (--) naja die Übungen halt meistens nicht alleine gehen. Und dann machen wir das so nach, wie er das gemacht hat. 
S1: Ach so läuft das also ab, danke für deine Erklärung. Und wenn ihr dann die Übungen macht, was macht dein Trainer dann in dieser Zeit? 
S2: Der guckt uns immer genau zu und geht in der Halle rum. Wenn wir was falsch machen oder ähm (--) halt nicht so gut, dann hilft er uns. 
S1: Kommt er dann manchmal auch zu dir und hilft dir?
S2: Ja genau. Letzte da ähm (--) hat er mir sogar extra gezeigt, wie (.) also wie ich besser aufschlagen kann. Und er äh (.) hat sich dann so richtig Zeit dafür genommen, obwohl die anderen alle schon fertig waren. Das fand ich richtig toll und hat mir geholfen. 
S1: Habe ich das richtig verstanden, dass es dir wichtig war, dass der Trainer dir extra Zeit gegeben hat?
S2: Ja das fand ich richtig nett von ihm! Weil danach habe ich die Übung halt auch echt besser gemacht so. Also mein Aufschlag hat sich so richtig dadurch verbessert glaube ich. 
S1: Das freut mich! Und wie ist das, wenn er euch was erklärt (--), also verstehst du das meistens direkt gut, was er sagt?
S2: Meistens schon. Manchmal zeigt er’s auch nochmal extra selber vor mit dem Ball, wenn manche das nicht so direkt kapieren. 
S1: Mhm. Gibt’s da auch mal Rückmeldungen von ihm, also, dass er sagt, wie’s gelaufen ist?
S2: Ja schon. Meistens so ähm (.) kurz nach der Übung dann. Oder manchmal auch erst später.
S1: Was meinst du mit später? 
S2: Ähm (---), naja wenn wir die Übung halt fertig haben. Da sammeln wir uns ja dann wieder im Kreis und äh (.) er sagt dann so allen zusammen, was gut war und was schlecht noch.
S1: Achso, verstehe. Was findest du denn besser? Wenn er das so danach sagt oder schon während ihr die Übung macht? 
S2: Dabei.
S1: Wieso?
S2: Mhh (--), weil ich das dann direkt besser machen kann, glaube ich. 
S1: Mhm. Und so ganz allgemein, wie findest du deinen Trainer so?
S2: Er ist gut. 
S1: Fällt dir eine konkrete Situation ein, in der du das gemerkt hast?
S2: Mh (---) ja. Also das letztens, was ich schon meinte, da hat er mir ja extra gezeigt, wie ich meinen Aufschlag besser machen kann, obwohl alle anderen schon fertig waren mit der Übung, das war ja schon nett von ihm. 
S1: Mhm, verstehe. Und wie ist das eigentlich, wenn mal was nicht so klappt im Training?
S2: Ähm, ja das ist manchmal blöd, aber passiert halt.
S1: Sagt der Trainer dann was dazu, wenn ein Fehler passiert?
S2: Also meistens sagt er einfach, wie man’s besser machen kann. Nicht so, dass er schimpft oder so. 
S1: Findest du es nicht blöd, wenn du im Spiel Fehler machst?
S2: Weiß nicht, ähm. Glaub’ schon, keine Ahnung. 
S1: Also ich meine, es ist ja auch ganz normal, dass man nicht alles direkt perfekt kann.
S2: Mhm, das stimmt. 
[Themenblock 2: Übungs-/Aufgabengestaltung]
S1: Okay, dann (--) ähm. Du hast eben schon ein bisschen davon erzählt, dass ihr verschiedene Übungen macht. Magst du mir einmal genauer erzählen, was ihr da im Training so übt? 
S2: Ja, also wir machen ganz viel Aufschlagen und Baggern und Pritschen halt. Und manchmal halt auch so Spiele oder ähm (.) Aufgaben, wo man dann quasi alles zusammen braucht. 
S1: Mhm, okay. Und was davon machst du am liebsten?
S2: Ich glaube ähm (--), also Baggern üben finde ich schon cool. Schon komisch eigentlich (--) weil, äh ich bin ja gar nicht so gut da drin. 
S1: Mhm. Gibt es denn andere Übungen, bei denen du denkst: Das kann ich richtig gut?
S2: Mh (.) beim Aufschlag glaub' ich bin ich richtig gut, weil ich den schon oft geübt habe. Mit meinem Papa im Garten auch. Und ähm (.) also Baggern klappt schon auch immer besser, seit der Trainer mir das mit den Armen gezeigt hat. 
S1: Habe ich das jetzt richtig verstanden, dass du beim Aufschlagen schon sehr gut bist, aber am liebsten magst du es, wenn ihr Baggern übt?
S2: Ja genau. Das ist irgendwie schon so. Ich ähm (--) weiß auch gar nicht wieso. Also natürlich übe ich auch super gerne Aufschlagen, weil äh (.) ich das ja gut kann. Die anderen fragen da auch immer nach Tipps und so, das finde ich cool. Beim Baggern aber, da frage ich auch die anderen mal nach Tipps. Das finde ich aber gar nicht schlimm, weil dadurch äh werd’ ich ja auch besser. Also glaube ich. Und (--) und Aufschlagen kann halt schon auch schnell mal langweilig sein, ehrlich gesagt. Beim Baggern muss ich mich aber immer so richtig konzentrieren und tausend Dinge gleichzeitig beachten. Ähm (--) das ist voll anstrengend, aber ich mag das Gefühl danach, wenn man die Übung gemacht hat und dann vielleicht halt auch was gelernt hat und besser geworden ist.
S1: Ah, ich verstehe! Das ist ja interessant. Wie lange macht ihr so eine Übung denn eigentlich so?
S2: Mh (---) weiß nicht, ist unterschiedlich. Wenn wir Technik machen (.) so fünf bis zehn Minuten vielleicht.
S1: Mhm. Geht dir das manchmal zu schnell oder zu langsam?
S2: Mh (--) manchmal ist es schon zu schnell. Äh, zum Beispiel (.) wenn wir so Reihen-Übungen machen und man direkt wieder dran ist. 
S1: Kannst du mir das erklären, ich weiß gar nicht, wie so eine Übung aussieht.
S2: Na ja, also wir stehen dann alle in einer Reihe an der Seite und einer nach dem anderen rennt nach vorne, baggert den Ball und stellt sich hinten wieder an. Aber ähm (--) weil die Schlange so kurz ist, ist man sofort wieder dran und hat gar keine Zeit zum Durchatmen! Da kommt man total aus dem Puste und (.) und ich schaff’s dann gar nicht mehr, die Arme richtig durchstrecken, wie das halt richtig ist. Aber ich versuche dann halt trotzdem irgendwie mitzumachen. Manchmal ruft der Trainer dann auch von der Seite: ‚Schnell! Gleich nochmal, das schaffst du!‘. Das hilft mir dann schon ein bisschen, mich nochmal anzustrengen. Aber richtig gut klappt die Übung bei mir erst, seitdem <Name> mir gezeigt hat, wie ich mich vorher schon richtig hinstellen muss. Und wenn ein schöner Ball gelingt, dann klatscht sie auch mit mir ab, das fühlt sich richtig gut an!
S1: Achso ist das! Und was machst du dann, wenn dir das zu schnell geht?
S2: Keine Ahnung. Mache dann halt irgendwie trotzdem mit. 
S1: Aha okay. Machen dir diese Übungen dann Spaß?
S2: Naja (--) mh. Wenn das so schnell geht alles und ich nicht mitkomme, vor allem wenn ich die Einzige bin, die nicht mitkommt, dann nervt das schon. Also ich fühle mich dann einfach blöd, wenn alle das besser können als ich. Es stresst halt auch, wenn man so hektisch hin- und her rennen muss. 
S1: Mhm, verstehe. Bekommt ihr eigentlich alle die gleichen Übungen?
S2: Ja schon. Also meistens machen alle das Gleiche. Nur manchmal, wenn wer das schon richtig gut kann, darf der was Schweres machen. 
S1: Darfst du auch manchmal was Schweres machen? 
S2: Ich durfte das letztens ähm (--) bei so einer Übung, ja. Da war ich sogar die Einzige. 
S1: Okay und wie war das für dich?
S2: Das war cool (--), weil das andere war halt schon sehr langweilig irgendwann. Fand ich dann gut, als der Trainer gesagt hat, dass ich auch was anderes machen kann. 
S1: Und du sagtest ja, dass du die einzige warst, die dann was anderes machen durfte. Wie hast du dich da gefühlt?
S2: Ähm (--) schon (.) besonders glaube ich. Aber auch ein bisschen (--) komisch. 
S1: Wieso komisch?
S2: Naja äh (.) die anderen haben dann schon geguckt. Vielleicht wollten die auch lieber dann meine Übung machen, weil die ja nicht so langweilig war. Da habe ich mich dann schon ein bisschen doof gefühlt also äh (.) ich meine das hat mir Leid getan.
S1: Hättest du dann auch lieber wieder die andere Übung gemacht? 
S2: Ne das nicht. Aber es wäre glaube ich besser gewesen wenn (--), ja wenn noch andere das auch gemacht hätten halt. 
S1: Mhm, das verstehe ich. Habe ich das dann auch richtig verstanden, dass du nicht alle Übung gleich gerne magst? 
S2: Nicht so wirklich, ähm. Also manchmal hab’ ich nicht so viel Lust auf Technikübungen. 
S1: Aha, okay. Magst du mir erzählen, wann dir das besonders so geht?
S2: Mh (--) also wenn wir voll lange immer nur das Gleiche machen, so wie (--) äh Pritschen gegen die Wand oder so. Das ist dann halt irgendwann langweilig.
S1: Das verstehe ich. Aber gibt es auch Übungen, die nie langweilig werden?
S2: Mh (---) ja doch! Also so richtig Spielen ist nie langweilig. Und wenn wir jetzt Technik machen, dann mache ich das einfach viel lieber mit anderen zusammen, weißt du? Also bei jetzt nur gegen die Wand, da bin ich ja alleine. Aber so zu zweit, da könnte ich das glaube ich stundenlang machen ((lacht)). So wie mit meinem Papa oder meiner Schwester am Strand oder im Garten. 
S1: Aha, interessant. 
[S1 erzählt im Anschluss noch etwas länger und sehr detailliert weiter, wie sie mit ihrem Papa zuhause den Aufschlag übt. S1 lässt ihn ausreden, statt ihn zu unterbrechen und leitet dann erst den nächsten Themenblock, etwas später als geplant, ein]
S2: Und dann üben wir so lange bis es klappt. Also das wollte ich nur kurz nochmal erzählen ähm (--) danke. 
S1: Das ist spannend! Magst du es gerne, mit anderen zu üben und zu spielen?
S2: Ja! Das ist eigentlich immer das beste beim Training.
S1: Aha, wieso ist das das Beste?
S2: Mhm (--) naja. Wir sind halt eine coole Gruppe. Also ich mag die meisten richtig gerne und wir machen auch manchmal sogar auch was zusammen. Äh also so in der Freizeit meine ich (.), wenn wir nicht beim Training sind. 
[Themenblock 3: Gruppendynamiken]
S1: Das ist ja schön. Seid ihr beim Training denn immer eine feste Gruppe, also immer die gleichen Leute?
S2: Ja genau. Manchmal aber (--) ähm teilen wir uns die Halle ja aber auch mit so anderem Gruppen aus unserem Verein. Die sind dann meistens älter als wir. Und am Ende spielen wir dann auch mal mit denen zusammen.
S1: Ah, okay. Und wie findest du das so?
S2: Ehrlich gesagt (--), weiß nicht so recht. Ist schon manchmal einschüchternd, weil viele von denen sind ja auch so richtig gut. Die sind ja älter und konnten schon mehr Üben als wir. Letztens, da haben wir so ein kleines Turnier gespielt mit denene beim Training. DAS hat richtig Spaß gemacht. 
S1: Oh wie cool. Wieso hat das so Spaß gemacht?
S2: Ähm (--) weiß nicht so recht. Vielleicht weil (---) wir da auch mal andere Teams hatten
S1: Was heißt andere Teams?
S2: Halt nicht die aus dem Training. Wir haben da Teams gemischt mit den Älteren. Da habe ich dann mit ein paar aus meiner Mannschaft gespielt und auch mit ein paar Älteren. 
S1: Mhm, magst du mir davon vielleicht etwas genauer erzählen? 
S2: Mhm. Joa also (--) jetzte Woche war dieses Turnier (.) und bei dem habe ich ein Ball gerettet so, der eigentlich schon viel zu weit weg war so. Die ganze Mannschaft hat danach total gejubelt, das war richtig cool! 
S1: Wie war das für dich, als die anderen so gejubelt haben?
S2: MEGA gut, also da fühlt man sich schon irgendwie wichtig (.) so für’s Team auch. 
S1: Ja sehr cool. Und wie ist es sonnst so mit den anderen im Team, also aus deiner Mannschaft; helft ihr euch da gegenseitig?
S2: Ja klar. Also wenn zum Beispiel ähm (--) jemand was nicht so gut kann, zeigen die anderen das manchmal auch. Ich habe letztens da ner anderen meinen kleinen Trick für’s Baggern gezeigt. Hat danach auch besser geklappt!
S1: Oh wow. Wird dir auch manchmal geholfen von anderen?
S2: Ja auch. Die eine kann das besser, der andere halt das.
S1: Und wie ist das für dich, wenn andere etwas besser können?
S2: Ähm (--) ist mir (.) irgendwie egal, glaube ich. Also wenn jetzt jemand damit total angibt, finde ich das schon blöd. Das passiert bei uns aber eigentlich eher nicht so in der Gruppe. 
S1: Mhm, verstehe. Vergleicht ihr euch denn manchmal untereinander, wer was besser kann?
S2: Mh, schon ein bisschen, aber nicht gemein oder so, sondern eher aus Spaß. 
S1: Wie meinst du das, aus Spaß?
S2: Ja also (--) es ist halt schon alles eher so lustig und locker bei uns. Wir lachen ganz viel zusammen, auch mit dem Trainer. Der macht dann manchmal so Späße auch. <Name> aus meier Gruppe kann zum Beispiel so mega gut Baggern und auch Pritschen. Aber äh (.) ihr Aufschlag ist immer so la la. Und dann wenn wir beim Spiel rotieren und sie das machen soll, also den Aufschalg, dann (.) sagt der Trainer immer so: Ohhh nee, Achtung <Name> schlägt auf. Wir lachend dann immer und sie auch ((lacht)).
S1: Das ist wirklich lustig. 
S2: Und wenn ich mal nen Ball verhaue, so richtig weit weg, dann äh (.) lache ich da ja auch drüber.
S1: Und stört dich das manchmal, wenn jemand was besser kann als du? 
S2: Nö, eigentlich nicht. Ist ja auch okay so, kann ja nicht jeder alles gleich gut.
S1: Das stimmt. Okay (--) danke, dass du mir so viel über dein Training erzählen konntest. Ich kann mir das jetzt schon viel besser vorstellen. Ich wollte dich noch eine letzte Sache fragen, wenn das okay ist?
S2: Mhm.
S1: Stell dir mal vor, du dürftest für einen Tag mal das Training selber zusammenstellen. Eins, in dem du dich so richtig gut und stark fühlst. Wie würde das aussehen?
S2: Oh (.) mh. Also (--) auf jeden Fall würden wir ganz viel Aufschlag machen, weil ich da ja gut bin, aber nicht nur, so (.) auch Sachen, die ich noch nicht so kann, aber nicht zu schwer. Also so, dass man’s schafft, wenn man sich ein bisschen anstrengt. Und der Trainer würde zwischendurch immer mal kurz zu einem hinkommen und was sagen, so wie ‘Das war schon gut’ oder so, und dann zeigen, was man noch besser machen kann. Und ähm (.) wir würden ganz am Anfang schon ein Spiel machen, nicht erst am Ende, weil das ist ja das Coolste. Und dass die anderen halt auch so mitjubeln, wenn was klappt, so wie beim Turnier. Das ist schon richtig nice, wenn man merkt, dass die sich mitfreuen. Und (.) ja, dass man auch mal selber entscheiden darf, was man üben will. Dann würde ich, glaub’ ich, zum Beispiel erstmal Baggern machen, weil ich da noch besser werden will. Das wär’ dann so (--) ja, das wär’ mein perfektes Training.
S1: Mhm, das klingt richtig gut. Du hast gesagt, du würdest merken, dass du etwas schaffst, wenn du dich ein bisschen anstrengst. Wie fühlt sich das für dich an?
S2: So (.) stolz irgendwie. Und auch so, ich kann das jetzt. Dann will man gleich noch mehr machen.
S1: Danke dir, das war richtig schön zu hören. Gibt’s sonst noch was, das du mir erzählen möchtest oder das ich nicht gefragt habe?
S2: Nee, eigentlich nicht. Doch (.) vielleicht noch, dass das Training eigentlich echt gut ist so, ich geh da immer gern hin.
S1: Das freut mich. Dann danke ich dir ganz herzlich fürs Mitmachen <Name>.
`;

// ============================================================
// 2) AB HIER: Programmlogik, normalerweise nichts ändern
// ============================================================
var BLOCKS = [];
var cur = null;
var nr = 0;
var sel = -1;
var onlyKid = false;
var showNr = true;
var q = '';
// bewusst neutrale Farben: Blau, Orange und Grün bleiben den Codes vorbehalten
var TINTS = ['#e4e4e4', '#d8dcf0', '#e6d8f0', '#d8ecec', '#e4e4e4'];

function newBlock(title){
  cur = {title: title, items: []};
  BLOCKS.push(cur);
}
function parse(){
  var lines = RAW.split('\n');
  for(var i = 0; i < lines.length; i++){
    var l = lines[i].trim();
    if(!l) continue;
    var m = l.match(/^\[(Einstiegsphase|Themenblock|Ausklang)[^\]]*\]$/);
    if(m){ newBlock(l.slice(1, -1)); continue; }
    if(!cur) newBlock('Beginn');
    var n = l.match(/^S([12])\s*:\s*(.*)$/);
    if(n){
      nr++;
      cur.items.push({typ: 'turn', s: n[1], text: n[2], nr: nr});
    } else if(l.charAt(0) === '[' && l.charAt(l.length - 1) === ']'){
      cur.items.push({typ: 'note', text: l.slice(1, -1)});
    } else if(cur.items.length){
      var last = cur.items[cur.items.length - 1];
      if(last.typ === 'turn'){ last.text += ' ' + l; }
    }
  }
}
function esc(t){
  return String(t).split('&').join('&amp;').split('<').join('&lt;').split('>').join('&gt;');
}
function hl(text, query){
  if(!query) return esc(text);
  var low = text.toLowerCase();
  var ql = query.toLowerCase();
  var out = '';
  var i = 0;
  var j = low.indexOf(ql, i);
  while(j > -1){
    out += esc(text.slice(i, j)) + '<mark>' + esc(text.slice(j, j + query.length)) + '</mark>';
    i = j + query.length;
    j = low.indexOf(ql, i);
  }
  return out + esc(text.slice(i));
}
function shortTitle(t){
  var m = t.match(/^Themenblock\s*(\d+)\s*:\s*(.*)$/);
  if(m) return m[1] + ' · ' + m[2];
  if(t.indexOf('Einstieg') === 0) return 'Einstieg';
  return t;
}
function turnCount(b){
  var c = 0;
  for(var i = 0; i < b.items.length; i++){ if(b.items[i].typ === 'turn') c++; }
  return c;
}
function addCss(){
  if(document.getElementById('tv-css')) return;
  var s = document.createElement('style');
  s.id = 'tv-css';
  s.textContent =
    '.tv-card{background:#fafafa;color:#222;border:1px solid #ccc;border-radius:8px;padding:14px;margin:12px 0;line-height:1.55}' +
    '.tv-meta{display:flex;flex-wrap:wrap;gap:8px;margin-bottom:10px}' +
    '.tv-meta div{background:#fff;border:1px solid #ddd;border-radius:6px;padding:6px 10px;font-size:0.9em}' +
    '.tv-meta span{display:block;font-size:0.75em;color:#777;text-transform:uppercase}' +
    '.tv-frage{font-size:0.9em;margin-bottom:12px;padding:8px 10px;border-left:4px solid #888;background:#f0f0f0}' +
    '.tv-bar{display:flex;flex-wrap:wrap;gap:4px}' +
    '.tv-seg{cursor:pointer;border-radius:6px;padding:6px 8px;font-size:0.85em;border:2px solid transparent;min-width:0}' +
    '.tv-seg b{display:block}' +
    '.tv-seg span{font-size:0.8em;color:#555}' +
    '.tv-seg.active{border-color:#333}' +
    '.tv-all{margin:8px 0;color:#222;border:1px solid #888;border-radius:6px;padding:4px 10px;cursor:pointer;background:#e8e8e8}' +
    '.tv-all.active{font-weight:bold;box-shadow:0 0 0 2px #333}' +
    '.tv-tools{display:flex;flex-wrap:wrap;gap:12px;align-items:center;margin:8px 0 12px 0;font-size:0.9em}' +
    '.tv-tools input[type=search]{padding:4px 8px;border:1px solid #aaa;border-radius:6px;color:#222;background:#fff}' +
    '.tv-bh{font-weight:bold;margin:16px 0 4px 0;padding:4px 8px;background:#e4e4e4;border-radius:4px}' +
    '.tv-row{display:flex;gap:8px;margin:6px 0}' +
    '.tv-nr{flex:0 0 2.2em;text-align:right;color:#888;font-size:0.8em;padding-top:8px}' +
    '.tv-wrap{flex:1;display:flex}' +
    '.tv-row.kid .tv-wrap{justify-content:flex-end}' +
    '.tv-bub{max-width:88%;padding:8px 12px;border-radius:12px}' +
    '.tv-row.int .tv-bub{background:#e9e9ee}' +
    '.tv-row.kid .tv-bub{background:#fff;border:1px solid #bbb}' +
    '.tv-who{font-size:0.7em;font-weight:bold;color:#666;margin-bottom:2px}' +
    '.tv-note{margin:8px 0;padding:6px 10px;font-size:0.85em;font-style:italic;color:#555;background:#f3f3f3;border-radius:6px;text-align:center}' +
    '.tv-card mark{background:#ffe066;color:#222}';
  document.head.appendChild(s);
}
function head(){
  var h = '<div class="tv-meta">';
  for(var i = 0; i < META.length; i++){
    h += '<div><span>' + esc(META[i][0]) + '</span>' + esc(META[i][1]) + '</div>';
  }
  h += '</div>';
  h += '<div class="tv-frage"><b>Forschungsfrage:</b> ' + esc(FRAGE) + '</div>';
  h += '<div id="tv-nav"></div>';
  h += '<div class="tv-tools">' +
       '<label><input type="checkbox" data-opt="nr" checked> Zeilennummern</label>' +
       '<label><input type="checkbox" data-opt="kid"> Nur Aussagen des Kindes</label>' +
       '<input type="search" id="tv-q" placeholder="Im Transkript suchen ...">' +
       '</div>';
  h += '<div id="tv-list"></div>';
  return h;
}
function nav(){
  var el = document.getElementById('tv-nav');
  if(!el) return;
  var h = '<div class="tv-bar">';
  for(var b = 0; b < BLOCKS.length; b++){
    var n = turnCount(BLOCKS[b]);
    h += '<div class="tv-seg' + (sel === b ? ' active' : '') + '" data-sel="' + b +
         '" style="flex:' + Math.max(n, 4) + ' 1 90px;background:' + TINTS[b % TINTS.length] + '">' +
         '<b>' + esc(shortTitle(BLOCKS[b].title)) + '</b><span>' + n + ' Beiträge</span></div>';
  }
  h += '</div>';
  h += '<button type="button" class="tv-all' + (sel === -1 ? ' active' : '') + '" data-sel="-1">Gesamtes Interview anzeigen</button>';
  el.innerHTML = h;
}
function list(){
  var el = document.getElementById('tv-list');
  if(!el) return;
  var ql = q.toLowerCase();
  var out = '';
  for(var b = 0; b < BLOCKS.length; b++){
    if(sel !== -1 && sel !== b) continue;
    var rows = '';
    var items = BLOCKS[b].items;
    for(var k = 0; k < items.length; k++){
      var it = items[k];
      if(it.typ === 'note'){
        if(!q){ rows += '<div class="tv-note">' + esc(it.text) + '</div>'; }
        continue;
      }
      if(onlyKid && it.s === '1') continue;
      if(q && it.text.toLowerCase().indexOf(ql) < 0) continue;
      var kid = (it.s === '2');
      rows += '<div class="tv-row ' + (kid ? 'kid' : 'int') + '">' +
              (showNr ? '<span class="tv-nr">' + it.nr + '</span>' : '') +
              '<div class="tv-wrap"><div class="tv-bub"><div class="tv-who">' +
              (kid ? 'S2 · Kind' : 'S1 · Interviewerin') + '</div>' + hl(it.text, q) + '</div></div></div>';
    }
    if(rows){ out += '<div class="tv-bh">' + esc(BLOCKS[b].title) + '</div>' + rows; }
  }
  el.innerHTML = out || '<p>Keine Treffer.</p>';
}
function onClick(e){
  var el = e.target.closest('[data-sel]');
  if(!el) return;
  sel = parseInt(el.getAttribute('data-sel'), 10);
  nav();
  list();
}
function onChange(e){
  var o = e.target.getAttribute('data-opt');
  if(o === 'nr'){ showNr = e.target.checked; }
  if(o === 'kid'){ onlyKid = e.target.checked; }
  list();
}
function onInput(e){
  if(e.target.id === 'tv-q'){
    q = e.target.value.trim();
    list();
  }
}
function init(tries){
  var root = document.getElementById('tv-widget');
  if(!root){
    if(tries > 0){ setTimeout(function(){ init(tries - 1); }, 250); }
    return;
  }
  if(root.getAttribute('data-ready')) return;
  root.setAttribute('data-ready', '1');
  parse();
  addCss();
  root.innerHTML = '<div class="tv-card">' + head() + '</div>';
  nav();
  list();
  root.addEventListener('click', onClick);
  root.addEventListener('change', onChange);
  root.addEventListener('input', onInput);
}
init(40);
</script>


### Check-up Farbcodierung

Du bekommst vier kurze Ausschnitte aus einem Interview mit einem Kind aus dem Volleyballtraining. Aufgabe: **Markiere die Sätze des Kindes farbig** und ordne sie damit einer Kategorie zu. Danach bestimmst du, welche Subkategorie am besten passt.

> **Hinweis:** Die Zuordnung ist nicht immer eindeutig. Nutze die Musterlösung als Orientierung und Anregung für den Vergleich im Plenum, nicht als "die einzig richtige" Antwort.

So geht's:

1. Wähle oben einen Markierstift (Blau = K1, Orange = K2, Grün = K3).
2. Klicke auf einen Satz des Kindes, um ihn zu markieren. Erneutes Klicken entfernt die Markierung.
3. Die Fragen der Interviewerin sind nur Kontext und werden nicht codiert. Sätze ohne Bezug zur Forschungsfrage bleiben unmarkiert.
4. Klicke auf **Weiter zu Schritt 2** und wähle für jeden markierten Satz die passende Subkategorie.
5. Klicke auf **Auswerten**, um die Musterlösung zu sehen.

<div id="qc-widget"></div>

<script>
// ============================================================
// EINSTELLUNG: false = nur Hauptkategorien codieren (Schritt 2 entfällt)
// ============================================================
var SUBS_AN = true;

// ============================================================
// KATEGORIENSYSTEM
// ============================================================
var KAT = {
  k1: {n: 'K1: Trainer:innenverhalten', kurz: 'K1', farbe: '#a6cee3', rand: '#1f78b4',
       subs: {fb: 'Feedback', ins: 'Instruktion', feh: 'Umgang mit Fehlern', kom: 'Kommunikation'}},
  k2: {n: 'K2: Übungs-/Aufgabengestaltung', kurz: 'K2', farbe: '#fdbf6f', rand: '#d9730d',
       subs: {sch: 'Passung der Schwierigkeit', tem: 'Passung der Geschwindigkeit', mit: 'Mitbestimmung', dif: 'Differenzierung'}},
  k3: {n: 'K3: Gruppendynamiken', kurz: 'K3', farbe: '#b2df8a', rand: '#33a02c',
       subs: {unt: 'Unterstützung/Kooperation', wet: 'Wettkampf/Vergleich'}}
};

// ============================================================
// DATEN
// S1 = ['S1', 'Text']   S2 = ['S2', [Sätze]]
// Satz = [Text, Hauptkategorie|null, Subkategorie|null, Erklärung, Grenzfall(1)]
// ============================================================
var AUS = [
  {titel: 'Ausschnitt 1', turns: [
    ['S1', 'Ah okay. Also der Trainer zeigt euch Sachen? Ich kann mir das nicht ganz so gut vorstellen, wie das genau abläuft. Kannst du mir das vielleicht nochmal genauer erklären?'],
    ['S2', [
      ['Also meistens stehen wir nach dem Aufwärmen alle so in einem Kreis halt.', null, null, 'Reine Beschreibung der Trainingsorganisation ohne Bezug zur Forschungsfrage. Bleibt unmarkiert.'],
      ['Und ähm (.) der Trainer macht dann eine Ansage, welche Übung wir machen.', 'k1', 'ins'],
      ['Wenn wir die noch gar nicht kennen, dann macht er das einmal vor wie das geht.', 'k1', 'ins', 'Der Trainer erklärt und demonstriert eine neue Übung: typische Instruktion.'],
      ['Manchmal braucht er da auch Hilfe, weil (--) naja die Übungen halt meistens nicht alleine gehen.', null, null, 'Organisatorisches Detail ohne Bezug zum Kompetenzerleben. Unmarkiert.'],
      ['Und dann machen wir das so nach, wie er das gemacht hat.', 'k1', 'ins', 'Grenzfall: Das Kind beschreibt sein eigenes Handeln, aber als direkte Folge der Instruktion. Auch unmarkiert wäre vertretbar.', 1]
    ]],
    ['S1', 'Ach so läuft das also ab, danke für deine Erklärung. Und wenn ihr dann die Übungen macht, was macht dein Trainer dann in dieser Zeit?'],
    ['S2', [
      ['Der guckt uns immer genau zu und geht in der Halle rum.', 'k1', 'ins', 'Grenzfall: Begleitendes Beobachten passt keiner Subkategorie ideal. Hier als Anleitung (Instruktion) gewertet.', 1],
      ['Wenn wir was falsch machen oder ähm (--) halt nicht so gut, dann hilft er uns.', 'k1', 'feh']
    ]],
    ['S1', 'Kommt er dann manchmal auch zu dir und hilft dir?'],
    ['S2', [
      ['Ja genau. Letzte Woche ähm (--) hat er mir sogar extra gezeigt, wie (.) also wie ich besser aufschlagen kann.', 'k1', 'ins'],
      ['Und er äh (.) hat sich dann so richtig Zeit dafür genommen, obwohl die anderen alle schon fertig waren.', 'k1', 'kom', 'Zuwendung und Zeit des Trainers: hier Kommunikation. Instruktion wäre ebenfalls vertretbar.', 1],
      ['Das fand ich richtig toll und hat mir geholfen.', 'k1', 'kom']
    ]],
    ['S1', 'Habe ich das richtig verstanden, dass es dir wichtig war, dass der Trainer dir extra Zeit gegeben hat?'],
    ['S2', [
      ['Ja das fand ich richtig nett von ihm!', 'k1', 'kom'],
      ['Weil danach habe ich die Übung halt auch echt besser gemacht so. Also mein Aufschlag hat sich so richtig dadurch verbessert, glaube ich.', null, null, 'Das ist die Wirkung auf das eigene Können (Kompetenzerleben), keine Bedingung im Training. Mit den drei Hauptkategorien bleibt der Satz unmarkiert. Guter Diskussionspunkt fürs Plenum.']
    ]]
  ]},
  {titel: 'Ausschnitt 2', turns: [
    ['S1', 'Habe ich das jetzt richtig verstanden, dass du beim Aufschlagen schon sehr gut bist, aber am liebsten magst du es, wenn ihr Baggern übt?'],
    ['S2', [
      ['Ja genau. Das ist irgendwie schon so. Ich ähm (--) weiß auch gar nicht wieso.', null, null],
      ['Also natürlich übe ich auch super gerne Aufschlagen, weil äh (.) ich das ja gut kann.', 'k2', 'sch', 'Die Übung passt zum eigenen Können (gut beherrscht).'],
      ['Die anderen fragen da auch immer nach Tipps und so, das finde ich cool.', 'k3', 'unt', 'Mitspielende holen sich Tipps: gegenseitige Unterstützung, nicht Trainerverhalten.'],
      ['Beim Baggern aber, da frage ich auch die anderen mal nach Tipps.', 'k3', 'unt'],
      ['Das finde ich aber gar nicht schlimm, weil dadurch äh werd’ ich ja auch besser. Also glaube ich.', 'k3', 'unt'],
      ['Und (--) und Aufschlagen kann halt schon auch schnell mal langweilig sein, ehrlich gesagt.', 'k2', 'sch', 'Zu leicht bzw. wenig fordernd (Langeweile): Passung der Schwierigkeit.'],
      ['Beim Baggern muss ich mich aber immer so richtig konzentrieren und tausend Dinge gleichzeitig beachten.', 'k2', 'sch'],
      ['Ähm (--) das ist voll anstrengend, aber ich mag das Gefühl danach, wenn man die Übung gemacht hat und dann vielleicht halt auch was gelernt hat und besser geworden ist.', 'k2', 'sch', 'Grenzfall: Die Anforderung passt (anstrengend, aber schaffbar). Gleichzeitig steckt Kompetenzerleben im Satz.', 1]
    ]],
    ['S1', 'Ah, ich verstehe! Das ist ja interessant. Wie lange macht ihr so eine Übung denn eigentlich so?'],
    ['S2', [
      ['Mh (---) weiß nicht, ist unterschiedlich. Wenn wir Technik machen (.) so fünf bis zehn Minuten vielleicht.', null, null, 'Sachliche Auskunft zur Dauer ohne Bewertung. Unmarkiert.']
    ]],
    ['S1', 'Mhm. Geht dir das manchmal zu schnell oder zu langsam?'],
    ['S2', [
      ['Mh (--) manchmal ist es schon zu schnell. Äh, zum Beispiel (.) wenn wir so Reihen-Übungen machen und man direkt wieder dran ist.', 'k2', 'tem']
    ]],
    ['S1', 'Kannst du mir das erklären, ich weiß gar nicht, wie so eine Übung aussieht.'],
    ['S2', [
      ['Na ja, also wir stehen dann alle in einer Reihe an der Seite und einer nach dem anderen rennt nach vorne, baggert den Ball und stellt sich hinten wieder an.', null, null, 'Beschreibung des Ablaufs ohne Bewertung. Unmarkiert.'],
      ['Aber ähm (--) weil die Schlange so kurz ist, ist man sofort wieder dran und hat gar keine Zeit zum Durchatmen!', 'k2', 'tem'],
      ['Da kommt man total aus dem Puste und (.) und ich schaff’s dann gar nicht mehr, die Arme richtig durchstrecken, wie das halt richtig ist.', 'k2', 'tem'],
      ['Aber ich versuche dann halt trotzdem irgendwie mitzumachen.', null, null],
      ['Manchmal ruft der Trainer dann auch von der Seite: ‚Schnell! Gleich nochmal, das schaffst du!‘.', 'k1', 'fb', 'Grenzfall: Anfeuern und Zuspruch. Feedback oder Kommunikation sind beide vertretbar; die Hauptkategorie K1 ist eindeutig.', 1],
      ['Das hilft mir dann schon ein bisschen, mich nochmal anzustrengen.', 'k1', 'fb'],
      ['Aber richtig gut klappt die Übung bei mir erst, seitdem <Name> mir gezeigt hat, wie ich mich vorher schon richtig hinstellen muss.', 'k3', 'unt', '<Name> ist eine Mitspielerin, nicht der Trainer. Deshalb K3, obwohl es inhaltlich um eine Instruktion geht.'],
      ['Und wenn ein schöner Ball gelingt, dann klatscht sie auch mit mir ab, das fühlt sich richtig gut an!', 'k3', 'unt']
    ]]
  ]},
  {titel: 'Ausschnitt 3', turns: [
    ['S2', [
      ['Ehrlich gesagt (--), weiß nicht so recht. Ist schon manchmal einschüchternd, weil viele von denen sind ja auch so richtig gut.', 'k3', 'wet'],
      ['Die sind ja älter und konnten schon mehr Üben als wir.', 'k3', 'wet'],
      ['Letztens, da haben wir so ein kleines Turnier gespielt mit denen beim Training.', null, null, 'Rahmeninformation ohne Erleben oder Bewertung. Unmarkiert; K3 wäre aber vertretbar.', 1],
      ['DAS hat richtig Spaß gemacht.', 'k3', 'wet', 'Grenzfall: Allgemeine Bewertung des gemeinsamen Turniers mit den Älteren, daher knapp K3.', 1]
    ]],
    ['S1', 'Oh wie cool. Wieso hat das so Spaß gemacht?'],
    ['S2', [
      ['Ähm (--) weiß nicht so recht. Vielleicht weil (---) wir da auch mal andere Teams hatten.', 'k3', 'unt', 'Grenzfall: Teamzusammensetzung ist ein Gruppenthema. Keine Subkategorie passt wirklich gut, hier Kooperation.', 1]
    ]],
    ['S1', 'Was heißt andere Teams?'],
    ['S2', [
      ['Halt nicht die aus dem Training. Wir haben da Teams gemischt mit den Älteren. Da habe ich dann mit ein paar aus meiner Mannschaft gespielt und auch mit ein paar Älteren.', 'k3', 'unt', null, 1]
    ]],
    ['S1', 'Mhm, magst du mir davon vielleicht etwas genauer erzählen?'],
    ['S2', [
      ['Mhm. Joa also (--) letzte Woche war dieses Turnier (.) und bei dem habe ich ein Ball gerettet so, der eigentlich schon viel zu weit weg war so.', null, null, 'Erfolgserlebnis des Kindes selbst (Kompetenzerleben), keine Bedingung. Unmarkiert.'],
      ['Die ganze Mannschaft hat danach total gejubelt, das war richtig cool!', 'k3', 'unt', 'Anerkennung durch das Team: am ehesten Unterstützung. Wettkampf/Vergleich wäre diskutierbar.', 1]
    ]],
    ['S1', 'Wie war das für dich, als die anderen so gejubelt haben?'],
    ['S2', [
      ['MEGA gut, also da fühlt man sich schon irgendwie wichtig (.) so für’s Team auch.', 'k3', 'unt']
    ]],
    ['S1', 'Ja sehr cool. Und wie ist es sonst so mit den anderen im Team, also aus deiner Mannschaft; helft ihr euch da gegenseitig?'],
    ['S2', [
      ['Ja klar. Also wenn zum Beispiel ähm (--) jemand was nicht so gut kann, zeigen die anderen das manchmal auch.', 'k3', 'unt'],
      ['Ich habe letztens da ner anderen meinen kleinen Trick für’s Baggern gezeigt. Hat danach auch besser geklappt!', 'k3', 'unt']
    ]]
  ]},
  {titel: 'Ausschnitt 4', turns: [
    ['S1', 'Stell dir mal vor, du dürftest für einen Tag mal das Training selber zusammenstellen. Eins, in dem du dich so richtig gut und stark fühlst. Wie würde das aussehen?'],
    ['S2', [
      ['Oh (.) mh. Also (--) auf jeden Fall würden wir ganz viel Aufschlag machen, weil ich da ja gut bin, aber nicht nur, so (.) auch Sachen, die ich noch nicht so kann, aber nicht zu schwer.', 'k2', 'sch'],
      ['Also so, dass man’s schafft, wenn man sich ein bisschen anstrengt.', 'k2', 'sch', 'Fordernd, aber schaffbar: fast ein Lehrbuchsatz für die Passung der Schwierigkeit.'],
      ['Und der Trainer würde zwischendurch immer mal kurz zu einem hinkommen und was sagen, so wie ‚Das war schon gut‘ oder so, und dann zeigen, was man noch besser machen kann.', 'k1', 'fb', 'Lob und Hinweis in einem Satz: Feedback. Für den zweiten Teil wäre auch Instruktion denkbar.'],
      ['Und ähm (.) wir würden ganz am Anfang schon ein Spiel machen, nicht erst am Ende, weil das ist ja das Coolste.', 'k2', 'mit', 'Grenzfall: Wunsch zur Ablaufgestaltung, am ehesten Mitbestimmung (das Kind gestaltet das Training).', 1],
      ['Und dass die anderen halt auch so mitjubeln, wenn was klappt, so wie beim Turnier.', 'k3', 'unt'],
      ['Das ist schon richtig nice, wenn man merkt, dass die sich mitfreuen.', 'k3', 'unt'],
      ['Und (.) ja, dass man auch mal selber entscheiden darf, was man üben will.', 'k2', 'mit'],
      ['Dann würde ich, glaub’ ich, zum Beispiel erstmal Baggern machen, weil ich da noch besser werden will.', 'k2', 'mit', 'Grenzfall: Das Kind wählt selbst eine Übung (Mitbestimmung), passend zu seinem Entwicklungsziel (Schwierigkeit).', 1],
      ['Das wär’ dann so (--) ja, das wär’ mein perfektes Training.', null, null]
    ]]
  ]}
];

// ============================================================
// AB HIER: Programmlogik, normalerweise nichts ändern
// ============================================================
var segs = [];
var marks = {};
var subsel = {};
var phase = 1;
var tool = 'k1';
var SYM = {
  ok: '<span class="qc-ok">✓</span>',
  sub: '<span class="qc-half">◐</span>',
  near: '<span class="qc-near">≈</span>',
  bad: '<span class="qc-bad">✗</span>'
};
function esc(t){
  return String(t).split('&').join('&amp;').split('<').join('&lt;').split('>').join('&gt;');
}
function prep(){
  for(var a = 0; a < AUS.length; a++){
    var tr = AUS[a].turns;
    for(var t = 0; t < tr.length; t++){
      if(tr[t][0] !== 'S2') continue;
      var arr = tr[t][1];
      for(var i = 0; i < arr.length; i++){
        var d = arr[i];
        var o = {idx: segs.length, text: d[0], k: d[1] || null, s: d[2] || null, e: d[3] || '', g: !!d[4], a: a};
        arr[i] = o;
        segs.push(o);
      }
    }
  }
}
function res(o){
  var m = marks[o.idx] || null;
  if(m === o.k){
    if(!SUBS_AN || !o.k || subsel[o.idx] === o.s) return 'ok';
    return 'sub';
  }
  return o.g ? 'near' : 'bad';
}
function myLabel(o){
  var m = marks[o.idx] || null;
  if(!m) return 'nicht markiert';
  var l = KAT[m].kurz;
  if(SUBS_AN && subsel[o.idx]){ l += ' · ' + KAT[m].subs[subsel[o.idx]]; }
  return l;
}
function solLabel(o){
  if(!o.k) return 'unmarkiert';
  return KAT[o.k].kurz + (SUBS_AN ? ' · ' + KAT[o.k].subs[o.s] : '');
}
function solStyle(o){
  if(!o.k) return '';
  return ' style="background:' + KAT[o.k].farbe + ';border-bottom:3px solid ' + KAT[o.k].rand + '"';
}
function selectHtml(i, m){
  var subs = KAT[m].subs;
  var h = '<select class="qc-sel" data-sub="' + i + '"><option value="">Subkategorie wählen ...</option>';
  for(var key in subs){
    h += '<option value="' + key + '"' + (subsel[i] === key ? ' selected' : '') + '>' + esc(subs[key]) + '</option>';
  }
  return h + '</select>';
}
function segHtml(o){
  var m = marks[o.idx] || null;
  var st = '';
  var x = '';
  if(m){
    var c = KAT[m];
    st = ' style="background:' + c.farbe + ';border-bottom:3px solid ' + c.rand + '"';
    x = '<sup class="qc-tag">' + c.kurz + '</sup>';
  }
  if(phase === 2 && m && SUBS_AN){ x += selectHtml(o.idx, m); }
  if(phase === 3 && (m || o.k)){ x += ' ' + SYM[res(o)]; }
  return '<span class="qc-seg' + (phase === 1 ? '' : ' locked') + '" data-seg="' + o.idx + '"' + st + '>' + esc(o.text) + '</span>' + x + ' ';
}
function wrap(o){
  return '<span data-w="' + o.idx + '">' + segHtml(o) + '</span>';
}
function fbHtml(a){
  var h = '';
  for(var i = 0; i < segs.length; i++){
    var o = segs[i];
    if(o.a !== a) continue;
    var r = res(o);
    if(r === 'ok' && !o.e) continue;
    h += '<div class="qc-fbi">' + SYM[r] + ' <span class="qc-seg locked"' + solStyle(o) + '>' + esc(o.text) + '</span>' +
         '<div class="qc-small">Deine Codierung: <b>' + esc(myLabel(o)) + '</b> &middot; Musterlösung: <b>' + esc(solLabel(o)) + '</b></div>' +
         (o.e ? '<div>' + esc(o.e) + '</div>' : '') + '</div>';
  }
  return h ? '<div class="qc-fb"><b>Musterlösung zu diesem Ausschnitt</b>' + h + '</div>' : '';
}
function scoreHtml(){
  var n = segs.length;
  var hk = 0;
  var sm = 0;
  var sk = 0;
  for(var i = 0; i < n; i++){
    var o = segs[i];
    if((marks[o.idx] || null) === o.k){
      hk++;
      if(SUBS_AN && o.k){ sm++; if(subsel[o.idx] === o.s){ sk++; } }
    }
  }
  var h = '<div class="qc-score"><b>Hauptkategorie:</b> ' + hk + ' von ' + n + ' Sätzen stimmen mit der Musterlösung überein.';
  if(SUBS_AN){ h += '<br><b>Subkategorie:</b> ' + sk + ' von ' + sm + ' Sätzen (gezählt nur dort, wo die Hauptkategorie stimmt).'; }
  return h + '<br>Die Musterlösung ist ein Vorschlag und Anlass zum Vergleich im Plenum.</div>';
}
function stepText(){
  if(phase === 1){ return '<b>Schritt 1' + (SUBS_AN ? ' von 2' : '') + ':</b> Markiere die Sätze des Kindes mit dem passenden Stift.'; }
  if(phase === 2){ return '<b>Schritt 2 von 2:</b> Wähle für jeden markierten Satz die passende Subkategorie.'; }
  return '<b>Musterlösung:</b> ✓ stimmt &middot; ◐ Hauptkategorie stimmt, Subkategorie weicht ab &middot; ≈ Grenzfall, Abweichung vertretbar &middot; ✗ weicht ab';
}
function addCss(){
  if(document.getElementById('qc-css')) return;
  var s = document.createElement('style');
  s.id = 'qc-css';
  s.textContent =
    '.qc-card{background:#fafafa;color:#222;border:1px solid #ccc;border-radius:8px;padding:14px;margin:12px 0;line-height:1.7}' +
    '.qc-top{position:sticky;top:0;z-index:5;background:#fafafa;padding-bottom:8px;border-bottom:1px solid #ddd;margin-bottom:10px}' +
    '.qc-bar{display:flex;flex-wrap:wrap;gap:8px;align-items:center;margin-bottom:6px}' +
    '.qc-lbl{font-weight:bold}' +
    '.qc-tool{color:#222;border:2px solid #888;border-radius:6px;padding:5px 10px;cursor:pointer;background:#eee;font-size:0.9em}' +
    '.qc-tool.active{box-shadow:0 0 0 3px #333;font-weight:bold}' +
    '.qc-step{font-size:0.9em}' +
    '.qc-aus{margin:16px 0;padding:10px;border:1px solid #ddd;border-radius:8px;background:#fff}' +
    '.qc-h{font-weight:bold;margin-bottom:6px}' +
    '.qc-int{color:#555;font-style:italic;margin:6px 0}' +
    '.qc-turn{margin:6px 0}' +
    '.qc-seg{cursor:pointer;border-bottom:2px dotted #999;padding:1px 2px;border-radius:3px}' +
    '.qc-seg:hover{background:#e6e6e6}' +
    '.qc-seg.locked{cursor:default}' +
    '.qc-tag{font-size:0.7em;font-weight:bold;margin-left:2px}' +
    '.qc-sel{margin-left:4px;font-size:0.8em;color:#222;background:#fff;border:1px solid #999;border-radius:4px}' +
    '.qc-ok{color:#1a7f37;font-weight:bold}' +
    '.qc-half{color:#1a7f37;font-weight:bold}' +
    '.qc-near{color:#9a6700;font-weight:bold}' +
    '.qc-bad{color:#cf222e;font-weight:bold}' +
    '.qc-actions{margin-top:14px;display:flex;flex-wrap:wrap;gap:8px}' +
    '.qc-btn{color:#222;border:1px solid #888;border-radius:6px;padding:6px 14px;cursor:pointer;background:#e8e8e8}' +
    '.qc-fb{margin-top:10px;border-top:2px solid #999;padding-top:8px}' +
    '.qc-fbi{margin:8px 0;padding:8px;background:#fafafa;border:1px solid #ddd;border-radius:6px}' +
    '.qc-small{font-size:0.9em;color:#444;margin-top:4px}' +
    '.qc-score{margin-top:16px;padding:10px;background:#fff;border:2px solid #999;border-radius:8px}';
  document.head.appendChild(s);
}
function render(){
  var root = document.getElementById('qc-widget');
  if(!root) return;
  var h = '<div class="qc-card"><div class="qc-top">';
  if(phase === 1){
    h += '<div class="qc-bar"><span class="qc-lbl">Markierstift:</span>';
    var keys = Object.keys(KAT);
    for(var k = 0; k < keys.length; k++){
      var c = KAT[keys[k]];
      h += '<button type="button" class="qc-tool' + (tool === keys[k] ? ' active' : '') + '" data-tool="' + keys[k] +
           '" style="background:' + c.farbe + ';border-color:' + c.rand + '">' + esc(c.n) + '</button>';
    }
    h += '<button type="button" class="qc-tool' + (tool === 'none' ? ' active' : '') + '" data-tool="none">Radierer</button></div>';
  }
  h += '<div class="qc-step">' + stepText() + '</div></div>';
  for(var a = 0; a < AUS.length; a++){
    h += '<div class="qc-aus"><div class="qc-h">' + esc(AUS[a].titel) + '</div>';
    var tr = AUS[a].turns;
    for(var t = 0; t < tr.length; t++){
      if(tr[t][0] === 'S1'){
        h += '<div class="qc-int"><b>S1:</b> ' + esc(tr[t][1]) + '</div>';
      } else {
        var line = '';
        for(var i = 0; i < tr[t][1].length; i++){ line += wrap(tr[t][1][i]); }
        h += '<div class="qc-turn"><b>S2:</b> ' + line + '</div>';
      }
    }
    if(phase === 3){ h += fbHtml(a); }
    h += '</div>';
  }
  if(phase === 3){ h += scoreHtml(); }
  h += '<div class="qc-actions">';
  if(phase === 1){ h += '<button type="button" class="qc-btn" data-act="next">' + (SUBS_AN ? 'Weiter zu Schritt 2' : 'Auswerten') + '</button>'; }
  if(phase === 2){
    h += '<button type="button" class="qc-btn" data-act="back">Zurück zu Schritt 1</button>';
    h += '<button type="button" class="qc-btn" data-act="check">Auswerten</button>';
  }
  h += '<button type="button" class="qc-btn" data-act="reset">Neu starten</button></div></div>';
  root.innerHTML = h;
}
function onClick(e){
  var el = e.target.closest('[data-tool],[data-seg],[data-act]');
  if(!el) return;
  var root = document.getElementById('qc-widget');
  if(el.hasAttribute('data-tool')){
    tool = el.getAttribute('data-tool');
    var bs = root.querySelectorAll('[data-tool]');
    for(var b = 0; b < bs.length; b++){ bs[b].classList.toggle('active', bs[b].getAttribute('data-tool') === tool); }
  } else if(el.hasAttribute('data-seg')){
    if(phase !== 1) return;
    var i = parseInt(el.getAttribute('data-seg'), 10);
    var old = marks[i] || null;
    marks[i] = (tool === 'none' || old === tool) ? null : tool;
    delete subsel[i];
    root.querySelector('[data-w="' + i + '"]').innerHTML = segHtml(segs[i]);
  } else {
    var act = el.getAttribute('data-act');
    if(act === 'next'){ phase = SUBS_AN ? 2 : 3; }
    if(act === 'back'){ phase = 1; }
    if(act === 'check'){ phase = 3; }
    if(act === 'reset'){ marks = {}; subsel = {}; phase = 1; }
    render();
    root.scrollIntoView();
  }
}
function onChange(e){
  if(!e.target.hasAttribute('data-sub')) return;
  var i = parseInt(e.target.getAttribute('data-sub'), 10);
  if(e.target.value){ subsel[i] = e.target.value; } else { delete subsel[i]; }
}
function init(tries){
  var root = document.getElementById('qc-widget');
  if(!root){
    if(tries > 0){ setTimeout(function(){ init(tries - 1); }, 250); }
    return;
  }
  if(root.getAttribute('data-ready')) return;
  root.setAttribute('data-ready', '1');
  prep();
  addCss();
  render();
  root.addEventListener('click', onClick);
  root.addEventListener('change', onChange);
}
init(40);
</script>
