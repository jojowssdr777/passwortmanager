---
marp: true
paginate: true
style: |
  /* ==============================================================
     Vorlage für Marp
     Diese Datei ist dein Gerüst. Ändere Werte, niemals die Namen
     der Klassen – die müssen zum Text passen, sonst passiert nichts.

     Wichtig: Diese Vorlage nutzt HTML (<div class="...">). Marp
     blockiert das standardmäßig. Aktiviere HTML:
       - VS Code: Einstellung "markdown.marp.enableHtml"
       - Marp CLI: Option --html
     ============================================================== */

  /* --- Die Farben ------------------------------------------------
     Jede Farbe steht genau einmal hier. Alle Klassen weiter unten
     benutzen nur noch den Namen. Willst du das Aussehen ändern,
     änderst du nur diese sieben Zeilen – nicht die Klassen. */

  :root {
    --blau:      #17324d;   /* Titel, Balken, Linien */
    --blau-hell: #24527a;   /* Akzente, Rand der Karten */
    --flaeche:   #f7f9fc;   /* Hintergründe von Kästen */
    --flaeche-2: #edf5fb;   /* zweiter Hintergrundton */
    --flaeche-3: #e8f1f8;   /* dritter Hintergrundton */
    --flaeche-4: #eef5f9;   /* Karten */
    --gelb:      #f4d35e;   /* Hervorhebung */
  }

  /* --- Die Folie selbst ------------------------------------------
     Jede Folie wird zu einem <section>. Alles hier gilt für alle. */
  section {
    display: flex;
    flex-direction: column;
    align-items: center;
    min-height: 100%;
    padding: 40px;
    font-family: Arial, Helvetica, sans-serif;
  }

  /* --- Der Folientitel ------------------------------------------- */
  .titel {
    width: 100%;
    text-align: center;
    color: var(--blau);
    margin-bottom: 24px;
  }

  /* --- Eine einfache Liste --------------------------------------- */
  .liste {
    width: 80%;
    padding: 18px 24px;
    background: var(--flaeche);
    border-left: 6px solid var(--blau);
    text-align: left;
  }

  /* --- Ein hervorgehobener Satz ---------------------------------- */
  .merksatz {
    width: 80%;
    margin-bottom: 20px;
    padding: 20px;
    background: var(--gelb);
    font-weight: bold;
    border-radius: 20px;
    text-align: left;
  }

  /* --- Ein einzelner Kasten -------------------------------------- */
  .box {
    width: 80%;
    padding: 18px 24px;
    background: var(--flaeche-2);
    border-left: 6px solid var(--blau);
    text-align: left;
  }

  /* --- Zwei Spalten: legt die Aufteilung fest -------------------- */
  .grid-2 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 24px;
    width: 100%;
  }

  /* Spaltenverhältnisse zum Ausprobieren:
       1fr 1fr  -> zwei gleich breite Spalten
       2fr 1fr  -> links doppelt so breit wie rechts
       1fr 2fr  -> rechts doppelt so breit wie links               */

  /* Eine breite und eine schmale Spalte:
     .grid-2 { grid-template-columns: 2fr 1fr; align-items: center; } */

  /* --- Die Spalte: nur das Aussehen ------------------------------ */
  .spalte {
    padding: 18px;
    background: var(--flaeche-3);
    border-radius: 14px;
    text-align: left;
  }

  /* --- Karten: drei Dinge nebeneinander -------------------------- */
  .karten {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 18px;
    width: 100%;
  }

  .karte {
    min-height: 150px;
    padding: 16px;
    background: var(--flaeche-4);
    border-top: 5px solid var(--blau-hell);
    text-align: left;
  }

  /* --- Bilder ---------------------------------------------------- */
  .bild {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
  }

  .bild img {
    width: 320px;
    height: auto;
  }

  /* --- Die Fußzeile ---------------------------------------------- */
  .fusszeile {
    width: 100%;
    margin-top: auto;
    padding-top: 12px;
    border-top: 1px solid var(--blau);
    text-align: center;
    font-size: 0.6em;
  }
---

<div class="titel">

# Titel deiner Präsentation

</div>

<div class="liste">

- Heutige Bedeutung: Warum ist das Thema gerade jetzt wichtig?
- Leitfrage und Ziel: Was möchte ich zeigen oder klären?
- Name
- Klasse
- Datum

</div>

<div class="fusszeile">
  Titel · Name, Klasse
</div>

---

<div class="titel">

# Eine Folie mit einer Aussage

</div>

<div class="liste">

- Erster Stichpunkt
- Zweiter Stichpunkt
- Dritter Stichpunkt

</div>

<div class="fusszeile">
  Einleitung · Name, Klasse
</div>

---

<div class="titel">

# Kostenmodell und Quellcode getrennt betrachten

</div>

<div class="grid-2">
  <div class="spalte">

  **Kostenmodell**

  - kostenpflichtig oder kostenlos?
  - kostenlose Grundfunktionen, Zusatzangebote?

  </div>
  <div class="spalte">

  **Quellcode**

  - öffentlich zugänglich?
  - Lizenz und Beleg prüfen

  </div>
</div>

<div class="fusszeile">
  Überblick · Name, Klasse
</div>

---

<div class="titel">

# Eine breite und eine schmale Spalte

</div>

<div class="grid-2" style="grid-template-columns: 2fr 1fr; align-items: center;">
  <div class="spalte">

  - Erklärung, Aufzählung oder Fließtext
  - Der Text bekommt zwei Teile der Breite

  </div>
  <div class="spalte">

  **Kurzfassung**

  - Ein Satz

  </div>
</div>

<div class="fusszeile">
  Detail und Überblick · Name, Klasse
</div>

---

<div class="titel">

# Drei Dienste im Überblick

</div>

<div class="karten">
  <div class="karte">

  **Dienst A**

  - Kostenmodell: …
  - Quellcode: …
  - Unterschied: …

  </div>
  <div class="karte">

  **Dienst B**

  - Kostenmodell: …
  - Quellcode: …
  - Unterschied: …

  </div>
  <div class="karte">

  **Dienst C**

  - Kostenmodell: …
  - Quellcode: …
  - Unterschied: …

  </div>
</div>

<div class="fusszeile">
  Überblick · Name, Klasse
</div>

---

<div class="titel">

# Merksatz oder Kasten

</div>

<div class="merksatz">
  Ein Satz, den das Publikum behalten soll.
</div>

<div class="box">

- Ein Punkt
- Ein weiterer Punkt

</div>

<div class="fusszeile">
  Merksatz · Name, Klasse
</div>

---

<div class="titel">

# Bild mit Beschreibung

</div>

<div class="bild">

![Kurze Beschreibung des Bildes](bilder/beispiel.png)

</div>

<div class="fusszeile">
  Bild · Name, Klasse
</div>

---

<div class="titel">

# Quellen

</div>

<div class="liste">

- [Titel der Quelle](https://beispiel.de), abgerufen am TT.MM.JJ
- [Titel der zweiten Quelle](https://beispiel.de), vom TT.MM.JJ

</div>

<div class="fusszeile">
  Quellen · Name, Klasse
</div>

---



#  Einstieg: Warum ist überhaupt ein Passwortmanager wichtig. 
 <div class="fusszeile">
  Passwortmanager · von Johannes, 9D
</div>

---

<div class="titel">

# Einstieg: Warum ist überhaupt ein Passwortmanager wichtig.

</div>

<div class="liste">

- Heutige Bedeutung: Warum ist das Thema gerade jetzt wichtig?
- Leitfrage und Ziel: Was möchte ich zeigen oder klären?
- Johannes
- 9D
- 9.10.26

</div>

<div class="fusszeile">
  Titel · Name, Klasse
</div>

---
1. <div class="titel">

# Warum ist es unsicher, dasselbe Passwort bei mehreren Diensten zu verwenden?

</div>

<div class="grid-2">
  <div class="spalte">

  

  - Da Häcker wenn sie das eine Passwort heraus gefunden haben sie es auch bei anderen Webseiten versuchen ein zu loggen um Daten oder Geld zu stehlen


  </div>
  <div class="spalte">

  **Quellcode**

  - Hier könnt ihr auf haveibeenpwned.com recherchieren
  - Ob ihr schon mal gehackt wurdet

  </div>
</div>

<div class="fusszeile">
   Johannes, 9D
</div>


---
2. <div class="titel">

# Was kann bei einem Datenleck passieren?

</div>

<div class="merksatz">
  Bei einem Datenleck kann passiren das vertrauliche oder personenbezogene Daten unbefugt
</div>

<div class="box">

- an die Öffentlichkeit
- in die Hände von Cyberkriminellen kommen kann

</div>

<div class="fusszeile">
  johannes, 9D
</div> 

---
3.

<div class="titel">

# Warum sind lange, einzigartige und zufällig erzeugte Passwörter schwer selbst zu verwalten?

</div>

<div class="liste">

- Weil man nicht alle Paswörter im kopf behalten kan.
- Wenn ich mir passwörter Uber meine email schicke und vergesse die webseiten dazu zu schreiben 
- Dritter Stichpunkt

</div>

<div class="fusszeile">
   Johannes, 9D
</div>

   
---
4. welche vorteile bitet ein passwortmanager

   - ein passwort maneger kann einem die vorteile verleien sich nur ein Passwort merken zu müssen und man dann alle log-in codes hat. 
---
5. Welche Risiken oder Nachteile bleiben trotz Passwortmanager bestehen?

   - ein großes risiko ist es dich bei deinen Passwort-Manager auf einem ungesperrten Gerät nicht zu schließen, weil dan jeder, der physischen Zugriff auf das Gerät hat, alle deine Passwörter einsehen kann.
---
6. Was ist zusätzlich zur Passwortverwaltung wichtig, zum Beispiel bei Zwei-Faktor-Authentifizierung oder Phishing? 

---
7. Was gibt es überhaupt für passwortmanager
  
   
---

8. <div class="titel">

# Quellen

</div>

<div class="liste">

- [Titel der Quelle](https://beispiel.de), abgerufen am TT.MM.JJ
- [Titel der zweiten Quelle](https://beispiel.de), vom TT.MM.JJ
- [Titel der Quelle](https://beispiel.de), abgerufen am TT.MM.JJ
- [Titel der zweiten Quelle](https://beispiel.de), vom TT.MM.JJ

</div>

<div class="fusszeile">
  Quellen · Name, Klasse
</div>

 