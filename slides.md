<!-- .slide: class="title-slide" data-background-color="#00374f" -->

<p class="eyebrow">Coffee Talk</p>

# Videos as Code

<p class="subtitle">Mit Remotion und Codex zur automatisierten Videoproduktion</p>
<p class="presenter">Jens-Christian Hübner</p>

<div class="hero-visual compact" aria-hidden="true">
  <div class="screen-frame">
    <div class="window-dots"><span></span><span></span><span></span></div>
    <div class="code-line w80"></div>
    <div class="code-line w55 accent"></div>
    <div class="code-line w70"></div>
    <div class="video-card">
      <div class="play-mark"></div>
      <div class="timeline"><span></span></div>
    </div>
  </div>
  <div class="flow-orbit"><span>Prompt</span><span>Code</span><span>Render</span></div>
</div>

Note:
Einstieg: Es geht nicht um ein weiteres Videotool, sondern um einen anderen Produktionsansatz. Videos werden beschreibbar, versionierbar und automatisierbar.

---

<!-- .slide: class="content-slide" -->

<p class="section-kicker">Ausgangslage</p>

## Warum reden wir darüber?

- Klassischer Videoworkflow ist oft langsam.
- Änderungen kosten Zeit.
- Wiederverwendung ist schwierig.
- Automatisierung ist begrenzt.

<div class="callout">
<strong>Videos können wie Software behandelt werden.</strong>
</div>

Note:
Kurz den bekannten Schmerz nennen: kleine Textänderungen, andere Farben, neue Versionen für mehrere Formate. Dann die Brücke zu Softwareprinzipien schlagen.

---

<!-- .slide: class="content-slide wide-slide" -->

<p class="section-kicker">Workflow</p>

## Der neue Workflow

<div class="workflow large" aria-label="Idee zu Render Workflow">
  <div class="step"><span>Idee</span></div>
  <div class="arrow"></div>
  <div class="step"><span>Prompt</span></div>
  <div class="arrow"></div>
  <div class="step"><span>Codex</span></div>
  <div class="arrow"></div>
  <div class="step"><span>React-Code</span></div>
  <div class="arrow"></div>
  <div class="step"><span>Remotion Preview</span></div>
  <div class="arrow"></div>
  <div class="step"><span>Feedback</span></div>
  <div class="arrow"></div>
  <div class="step"><span>Render</span></div>
</div>

<p class="big-statement">Die meiste Zeit verbringt man nicht mehr mit Tippen, sondern mit Entscheiden.</p>

Note:
Diese Folie setzt das mentale Modell für die Demo. Wichtig: Codex ist Teil der Schleife, aber Entscheidungen, Geschmack und Review bleiben bei uns.

---

<!-- .slide: class="content-slide" -->

<p class="section-kicker">Grundlage</p>

## Was ist Remotion?

- Videos als React-Komponenten
- Animationen mit Code
- Datengetriebene Inhalte
- Renderbar als echtes Video

```tsx
import {AbsoluteFill} from "remotion";

export const Intro = () => (
  <AbsoluteFill className="slide">
    <h1>Videos as Code</h1>
    <p>Prompt. Code. Render.</p>
  </AbsoluteFill>
);
```

Note:
Remotion kurz erklären: React rendert Frames. Aus Komponenten, Props und Daten wird am Ende eine MP4 oder ein anderes Videoformat.

---

<!-- .slide: class="content-slide wide-slide" -->

<p class="section-kicker">Vergleich</p>

## Warum Code für Videos?

| Timeline | Remotion |
| --- | --- |
| Manuelle Bearbeitung | Deklarativer Code |
| Schwer reproduzierbar | Git-Versionierung |
| Copy & Paste | Komponenten |
| Statisch | Datengetrieben |
| Einzelstück | Automatisierbare Pipeline |

Note:
Nicht als Entweder-oder verkaufen. Timeline-Tools bleiben stark, aber Code ist besonders interessant, wenn Varianten, Daten oder wiederkehrende Formate wichtig sind.

---

<!-- .slide: class="content-slide" -->

<p class="section-kicker">Pair Programming</p>

## Wo kommt Codex ins Spiel?

- Codex erzeugt React-/TypeScript-Code.
- Codex schreibt Animationen.
- Codex repariert Fehler.
- Codex verbessert Layouts.
- Codex iteriert über Prompts.

<div class="callout strong">
<strong>Codex wird zum Pair Programmer für Videoprojekte.</strong>
</div>

Note:
Beispiele nennen: Komponente anlegen, Timing anpassen, Layout vereinfachen, Fehler aus der Preview beheben. Der Wert liegt in der kurzen Iterationsschleife.

---

<!-- .slide: class="content-slide" -->

<p class="section-kicker">Live-Demo</p>

## Vom Prompt zum Video

<div class="prompt-box">
  <span class="badge">Demo-Prompt</span>
  <p>Erstelle einen modernen Intro-Screen für ein Produktvideo mit animierter Headline, Subline und Call-to-Action.</p>
</div>

- Farbe anpassen
- Timing verbessern
- Layout vereinfachen
- Icon oder Diagramm ergänzen
- Final rendern

Note:
Hier in die Live-Demo wechseln. Vorher einen funktionierenden Remotion-Startzustand bereithalten. Ziel ist nicht Perfektion im ersten Versuch, sondern sichtbare Iteration.

---

<!-- .slide: class="content-slide wide-slide" -->

<p class="section-kicker">Einsatzfelder</p>

## Was eignet sich besonders gut?

<div class="icon-grid">
  <article class="icon-card"><span class="icon">▶</span><h3>Intro-Animationen</h3></article>
  <article class="icon-card"><span class="icon">?</span><h3>Erklärvideos</h3></article>
  <article class="icon-card"><span class="icon">#</span><h3>Social-Media-Clips</h3></article>
  <article class="icon-card"><span class="icon">%</span><h3>Statistik-Animationen</h3></article>
  <article class="icon-card"><span class="icon">◆</span><h3>Produktvideos</h3></article>
  <article class="icon-card"><span class="icon">↗</span><h3>Datengetriebene Visualisierungen</h3></article>
</div>

Note:
Gute Beispiele sind stark strukturiert: wiederkehrende Layouts, klare Templates, datenbasierte Inhalte und kurze Formate.

---

<!-- .slide: class="content-slide" -->

<p class="section-kicker">Realität</p>

## Was funktioniert nicht automatisch perfekt?

- Komplexes Corporate Design
- Exaktes Timing
- Audioabstimmung
- Sehr individuelle Storyboards
- Finale Qualitätskontrolle

<div class="callout">
<strong>KI ersetzt nicht den Menschen. Sie beschleunigt die Iteration.</strong>
</div>

Note:
Bewusst Erwartungen erden. Für markennahe Arbeit braucht es weiterhin Review, Geschmack, Timinggefühl und finale Kontrolle.

---

<!-- .slide: class="content-slide" -->

<p class="section-kicker">Arbeitsweise</p>

## Best Practices

- Klein anfangen
- Klare Prompts schreiben
- Komponenten modular halten
- Regelmäßig in der Preview prüfen
- Visuelle Änderungen konkret beschreiben
- Git nutzen

Note:
Praktischer Rat für die Live-Demo und eigene Projekte. Besonders wichtig: nicht alles in einem Prompt lösen wollen.

---

<!-- .slide: class="content-slide" -->

<p class="section-kicker">Takeaways</p>

## Erkenntnisse

- Weniger Boilerplate
- Schnelleres Prototyping
- Mehr Experimente
- Änderungen per Prompt
- Code Review statt Pixel-Schubsen

<div class="mini-workflow" aria-hidden="true">
  <span>Prompt</span>
  <span>Preview</span>
  <span>Review</span>
  <span>Render</span>
</div>

Note:
Als Zusammenfassung vor dem Fazit nutzen. Die größte Veränderung ist die Art der Zusammenarbeit mit dem Material.

---

<!-- .slide: class="statement-slide" data-background-color="#00374f" -->

<p class="section-kicker inverted">Fazit</p>

## Videos werden Software.

<div class="keyword-row">
  <span>Komponenten</span>
  <span>Prompts</span>
  <span>Reviews</span>
  <span>Git</span>
  <span>Automatisierung</span>
</div>

Note:
Die Kernbotschaft wiederholen. Nicht jedes Video muss Code sein, aber viele wiederkehrende Videoformate profitieren stark davon.

---

<!-- .slide: class="closing-slide" data-background-color="#f5f5f5" -->

<p class="section-kicker">Vielen Dank!</p>

## Fragen?

<p class="closing-claim">Prompt. Code. Render.</p>

Note:
Optional: Link zum Demo-Repository, gerenderter Beispielclip oder QR-Code ergänzen.
