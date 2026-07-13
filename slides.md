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

<!-- .slide: class="content-slide wide-slide ai-video-slide" -->

<p class="section-kicker">KI-Videoworkflows</p>

## Zwei Wege, KI für Videos zu nutzen

<div class="ai-paths">
  <article class="ai-path-card">
    <header>
      <span class="path-icon" aria-hidden="true">
        <svg viewBox="0 0 24 24" role="img"><path d="m15 4 5 5L9 20l-5-5L15 4Z"></path><path d="m13 6 5 5M6 4V2M5 3H3m17 12v-2m1 1h2M6 21v-2m1 1H5"></path></svg>
      </span>
      <h3>Prompt <span aria-hidden="true">→</span> Video</h3>
    </header>
    <ul>
      <li>KI erzeugt direkt das fertige Video</li>
      <li>Fokus auf kreative Inhalte</li>
      <li>Änderungen erfolgen über neue Prompts</li>
      <li>Ergebnis ist nur begrenzt reproduzierbar</li>
      <li>Ideal für einmalige Marketing- oder Social-Media-Videos</li>
    </ul>
  </article>

  <div class="path-divider" aria-hidden="true"><span>→</span></div>

  <article class="ai-path-card highlighted">
    <header>
      <span class="path-icon" aria-hidden="true">
        <svg viewBox="0 0 24 24" role="img"><rect x="3" y="4" width="18" height="16" rx="2"></rect><path d="m7 9 3 3-3 3m6 0h4"></path></svg>
      </span>
      <h3>Prompt <span aria-hidden="true">→</span> Code <span aria-hidden="true">→</span> Video</h3>
    </header>
    <ul>
      <li>KI schreibt React- und Remotion-Code</li>
      <li>Das Video entsteht durch Software</li>
      <li>Änderungen sind im Code nachvollziehbar</li>
      <li>Versionierung mit Git</li>
      <li>Ideal für Templates, Automatisierung und datengetriebene Videos</li>
    </ul>
  </article>
</div>

<div class="callout ai-video-callout">
  <strong>Wir lassen die KI nicht das Video erstellen.<br>Wir lassen die KI die Software entwickeln, die das Video erzeugt.</strong>
</div>

<div class="ai-process" aria-label="Prompt zu beliebig vielen Videos">
  <span>Prompt</span><i>→</i><span>Codex</span><i>→</i><span>React + Remotion</span><i>→</i><span>Render</span><i>→</i><strong>beliebig viele Videos</strong>
</div>

Note:
Viele kennen KI-Videogeneratoren wie Sora oder Veo. Unser Ansatz ist ein anderer: Wir erzeugen nicht einzelne Videos, sondern entwickeln mit KI eine wiederverwendbare Videopipeline. Dadurch profitieren wir von Softwareentwicklung: Git, Komponenten, Tests, Wiederverwendbarkeit und Automatisierung.

---

<!-- .slide: class="content-slide wide-slide editing-slide" -->

<p class="section-kicker">Vergleich</p>

## Warum Code statt Timeline?

<div class="ai-paths editing-compare">
  <article class="ai-path-card editing-card">
    <header>
      <span class="path-icon" aria-hidden="true">
        <svg viewBox="0 0 24 24" role="img"><rect x="3" y="5" width="18" height="14" rx="2"></rect><path d="M7 5v14m10-14v14M3 9h4m10 0h4M3 15h4m10 0h4"></path></svg>
      </span>
      <h3>Klassische Videobearbeitung</h3>
    </header>
    <ul>
      <li>Arbeiten auf einer visuellen Timeline</li>
      <li>Inhalte werden per Maus verschoben</li>
      <li>Animationen werden manuell angepasst</li>
      <li>Änderungen erfolgen direkt im Projekt</li>
      <li>Optimal für individuelle, kreative Einzelprojekte</li>
    </ul>
    <p class="tool-examples">DaVinci Resolve <span>•</span> Final Cut Pro <span>•</span> Premiere Pro</p>
  </article>

  <div class="path-divider editing-divider" aria-hidden="true"><span>vs.</span></div>

  <article class="ai-path-card editing-card highlighted">
    <header>
      <span class="path-icon" aria-hidden="true">
        <svg viewBox="0 0 24 24" role="img"><path d="m8 9-3 3 3 3m8-6 3 3-3 3m-3-9-2 12"></path></svg>
      </span>
      <h3>Videos as Code</h3>
    </header>
    <ul>
      <li>Videos werden als React-Komponenten beschrieben</li>
      <li>Layouts und Animationen entstehen im Code</li>
      <li>Inhalte können aus Daten erzeugt werden</li>
      <li>Änderungen sind versionierbar und reproduzierbar</li>
      <li>Optimal für Templates, Automatisierung und skalierbare Videoproduktion</li>
    </ul>
    <p class="tool-examples">Remotion <span>•</span> React <span>•</span> TypeScript</p>
  </article>
</div>

<div class="callout editing-callout">
  <strong>Wir ersetzen keine Videoschnittsoftware.<br>Wir ergänzen sie um einen Softwareentwicklungs-Workflow.</strong>
</div>

<div class="editing-example-callout">
  <p>Wenn ich ein <strong>einzelnes Werbevideo</strong> schneiden möchte, nutze ich DaVinci Resolve.</p>
  <p>Wenn ich <strong>500 Videos aus unterschiedlichen Daten</strong> erzeugen möchte, nutze ich Remotion.</p>
</div>

Note:
Die Frage ist nicht "Was ist besser?"

Sondern: Für welchen Anwendungsfall ist welches Werkzeug geeignet?

Videobearbeitungsprogramme sind hervorragend für kreative Einzelproduktionen.

Remotion eignet sich besonders, wenn Videos reproduzierbar, datengetrieben, automatisiert oder als Teil einer Software entstehen sollen.

Die beiden Ansätze schließen sich nicht aus, sondern ergänzen sich.

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

<!-- .slide: class="content-slide wide-slide live-demo-slide" -->

<p class="section-kicker">Remotion + Codex</p>

## Live-Demo

<p class="demo-subtitle">Von der Idee zur wiederverwendbaren Video-Komponente</p>

<div class="demo-roadmap" aria-label="Vier Schritte der Live-Demo">
  <article class="demo-stage">
    <header>
      <span class="demo-number">1</span>
      <span class="path-icon" aria-hidden="true">
        <svg viewBox="0 0 24 24" role="img"><rect x="3" y="5" width="18" height="14" rx="2"></rect><path d="m10 9 5 3-5 3V9Z"></path></svg>
      </span>
    </header>
    <h3>Szene erzeugen</h3>
    <p class="demo-prompt">„4-Sekunden-Intro mit Titel und Unterzeile erstellen.“</p>
    <p class="demo-goal"><span>Ziel</span> Funktionierende Remotion-Composition</p>
  </article>

  <article class="demo-stage">
    <header>
      <span class="demo-number">2</span>
      <span class="path-icon" aria-hidden="true">
        <svg viewBox="0 0 24 24" role="img"><path d="M12 3a9 9 0 1 0 0 18h1.5a1.8 1.8 0 0 0 0-3.6h-1a1.5 1.5 0 0 1 0-3H15a6 6 0 0 0 0-12h-3Z"></path><circle cx="7.5" cy="10" r=".8"></circle><circle cx="10" cy="6.8" r=".8"></circle><circle cx="15" cy="7" r=".8"></circle></svg>
      </span>
    </header>
    <h3>Branding anwenden</h3>
    <p class="demo-prompt">„Farben und Typografie ans Epikur-Branding anpassen.“</p>
    <p class="demo-goal"><span>Ziel</span> Corporate Design per Prompt</p>
  </article>

  <article class="demo-stage">
    <header>
      <span class="demo-number">3</span>
      <span class="path-icon" aria-hidden="true">
        <svg viewBox="0 0 24 24" role="img"><path d="m15 4 5 5L9 20l-5-5L15 4Z"></path><path d="m13 6 5 5M6 4V2M5 3H3m17 12v-2m1 1h2"></path></svg>
      </span>
    </header>
    <h3>Animation verfeinern</h3>
    <p class="demo-prompt">„Headline federnd, Unterzeile verzögert einblenden.“</p>
    <p class="demo-goal"><span>Ziel</span> Iterative Verbesserung statt Neuerstellung</p>
  </article>

  <article class="demo-stage">
    <header>
      <span class="demo-number">4</span>
      <span class="path-icon" aria-hidden="true">
        <svg viewBox="0 0 24 24" role="img"><path d="m8 9-3 3 3 3m8-6 3 3-3 3m-3-9-2 12"></path></svg>
      </span>
    </header>
    <h3>Wiederverwendbar machen</h3>
    <p class="demo-prompt">„Titel und Untertitel über Props konfigurierbar machen.“</p>
    <p class="demo-goal"><span>Ziel</span> Aus der Szene wird eine Komponente</p>
  </article>
</div>

<div class="callout demo-callout">
  <strong>Nicht nur ein Video – eine parametrisierbare Software-Komponente.</strong>
</div>

<div class="demo-result-line" aria-label="Ergebnisprozess">
  <span>Prompt</span><i>→</i><span>Codex</span><i>→</i><span>Remotion-Szene</span><i>→</i><span>Iteration</span><i>→</i><strong>wiederverwendbare Komponente</strong>
</div>

Note:
- Der erste Schritt soll bewusst klein und zuverlässig sein.
- Der eigentliche Mehrwert entsteht durch die kurzen Folgeprompts.
- Die Szene wird nicht jedes Mal neu generiert, sondern schrittweise weiterentwickelt.
- Der letzte Schritt zeigt den Unterschied zu klassischer Videobearbeitung besonders deutlich.
- Nach Einführung der Props soll der Titel in Remotion Studio live von „Videos as Code“ zu „Coffee Talk“ oder „Willkommen bei Epikur“ geändert werden.
- Dadurch wird sichtbar, dass nicht nur ein einzelnes Video entstanden ist, sondern ein wiederverwendbares Template.

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

- Weniger sich wiederholende Arbeitsschritte
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
