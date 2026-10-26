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
    --blau:      #028ad8;   /* Titel, Balken, Linien */
    --blau-hell: #e7e9e5;   /* Akzente, Rand der Karten */
    --flaeche:   #dad9df;   /* Hintergründe von Kästen */
    --flaeche-2: #dad9df;   /* zweiter Hintergrundton */
    --flaeche-3: #dad9df;   /* dritter Hintergrundton */
    --flaeche-4: #ecf2f5;   /* Karten */
    --gelb:      #19fa04;   /* Hervorhebung */
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
    font-size: 23px;
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
    width: 90%;
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
    font-size: 20px;
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
    font-size: 20px;
  }
---
<div class="titel">

# Passwortmanager

</div>

<div class="merksatz">

# Leitfrage:
Welchem Passwortmanager vertraue ich eigentlich täglich meine wichtigen Passwörter an?
Microsoft Edge Passwortmanager / Samsung Pass / Google Passwortmanager
</div>

<div class="box">

- Was möchte ich zeigen oder klären? 

was ist für mich der beste Passwortmanager


</div>

<div class="fusszeile">
  · johannes.vervoort, 9d
</div>



---

<div class="titel">

# Wozu benötige ich einen Passwortmanager
</div>
<div class="liste">

1. **Was ist ein Passwortmanager?**
Der Passwortmanager ist ein Programm, das Zugangsdaten verschlüsselt an einem sichereren Ort abspeichert.  Viele dieser Programme bieten auch die Möglichkeit, Passwörter automatisch zu erstellen. Dies soll die Sicherheit erhöhen.

2. **Welche Probleme löst ein Passwortmanager?**
Für jedes Konto im Internet sollte man ein anderes Passwort verwenden. Da ich mir aber nicht viele Passwörter merken kann, übernimmt der Passwortmanager diese Aufgabe. Ich brauche dann nur noch ein Masterpasswort für den Passwortmanager.
3. **Warum brauche ich überhaupt ein sicheres Passwort?**
Ein sicheres Passwort schützt meine Daten vor Angriffen von Hackern oder anderen unbefugten Zugriffen. Wenn ich für viele verschiedene Onlinekonten dasselbe Passwort benutze, werden bei einem Passwortdiebstahl direkt viele meiner Konten im Internet bedroht.


</div>

---
<div class="titel">

# Meine drei Fragen

</div>

<div class="liste">

1. **Wo finde ich den Passwortmanager?**
- Mir ist wichtig zu erfahren, ob es mir leicht gemacht wird, meine wichtigen Daten gut zu schützen. Wenn das schon zu kompliziert ist, möchte ich lieber einen einfacheren Manager haben.
1.  **Welchen Funktionsumfang hat der Passwortmanager?**
- Ich frage mich, wie gut meine Daten geschützt werden und welche Möglichkeiten mir für den Zugriff geboten werden.
1. **Wie viel kostet der Passwortmanager?**
- Ist der Schutz meiner Passwörter kostenlos, oder verlangen die Anbieter für diesen Schutz Geld? Und wenn ja, wie viel?

</div>

---
<div class="titel">

# Meine drei meistgenutzten Passwortmanager

</div>

<div class="karten">
  <div class="karte">

  **Microsoft Edge Passwortmanager**

 Der Microsoft Edge Passwortmanager gehört zu Microsoft und ist direkt im Edge-Browser verfügbar. Er ist Bestandteil des Browsers und benötigt keine zusätzliche Installation.
  

  </div>
  <div class="karte">

  **Samsung Pass**

Samsung Pass ist ein Passwortmanager von Samsung Electronics. Er wurde speziell für Samsung-Geräte entwickelt.  Mit ihm kann ich mich unter anderem mit biometrischen Merkmalen wie dem Fingerabdruck anmelden.
  
  </div>
  <div class="karte">

 **Google Passwortmanager**

Der Google Passwortmanager ist von Google. Er ist in Google Chrome und Android integriert und kann gespeicherte Passwörter über das Google-Konto zwischen unterstützten Geräten synchronisieren – z.B. kann er ein Passwort auch auf mehreren Geräten abgleichen.
  
  

</div>





---

# Meine Passwortmanager im Vergleich

<div class="karten">
  <div class="karte">

  **Wo finde ich den Manager?**
  **Microsoft Edge Passwortmanager:** Direkt im Browser Microsoft Edge
  **Sammsung Pass:** Auf unterstützten Samsunggeräten
  **Google passwortmanager:** Direkt im Browser Google-Chrome und in Android

  </div>
  <div class="karte">

  **Welchen Funktionsumfang hat der Passwortmanager?** 
  **Microsoft Edge Passwortmanager:** Speichert Passwörter und füllt Anmeldedaten automatisch aus. Unterstütz auch Passkeys: Gesicht, Fingerabdruck oder 
  Pin* 2FA-fähig
  **Sammsung Pass:** Biometrischer Authentifizierungsdienst Anmeldung per Fingerabdruck, Pin, Iris-Erkennung, Gesichtserkennung, Muster und Passwort* 2FA-fähig
  **Google passwortmanager:** Speichert Passwörter und füllt sie automatisch aus* 2FA-fähig


 </div>
 <div class="karte">

  **Wie viel kostet der Passwortmanager?** 
  **Microsoft Edge Passwortmanager:** Kostenlos nutzbar
  **Sammsung Pass:** Kostenlos nutzbar
  **Google passwortmanager:** Kostenlos nutzbar

</div>  

</div>

<div class="fusszeile">
 *Funktionsumfang abhängig von Gerät und Plattform
</div>


---
<div class="titel">

# Allgemeine Informationen über Samsung Pass 

</div>

<div class="liste">

1. **Wo finde ich Samsung Pass?**
•	Samsung Pass ist auf unterstützten Samsung-Galaxy-Geräten verfügbar.
•	Auf neueren Geräten ist Samsung Pass in die App Samsung Wallet integriert.
2. **Welche Funktionen bietet Samsung Pass?**
•	Speichert Benutzernamen und Passwörter.
•	Fügt gespeicherte Anmeldedaten automatisch ein.
•	Ermöglicht die Anmeldung per Fingerabdruck oder 
3. **Wie viel kostet Samsung Pass?**
•	Samsung Pass ist kostenlos nutzbar.
•	Für die Passwortverwaltung ist kein zusätzliches kostenpflichtiges Abonnement erforderlich.

</div>


---
# Wie schützt Samsung Pass meine Passwörter?

</div>

<div class="karten">
  <div class="karte">

  **Anmeldung mit Fingerabdruck**

  -  Statt ein Passwort einzutippen, kann ich mich auf unterstützten Geräten mit meinem Fingerabdruck anmelden.
  So muss ich meine gespeicherten Zugangsdaten nicht jedes Mal selbst eingeben.


  </div>
  <div class="karte">

  **Zwei-Faktor-Authentifizierung: 2FA**

  -  Das Samsung-Konto kann mit einer zusätzlichen Sicherheitsabfrage geschützt werden.
  neben dem Passwort wird dann eine zweite Bestätigung benötigt, beispielsweise über das Smartphone.

  </div>
  <div class="karte">

  **Samsung Pass als 2FA-Hilfe**

  - Samsung Pass kann zusätzliche Sicherheitscodes für bestimmte Websites und Apps erzeugen.
Diese Codes ändern sich regelmäßig und dienen als weiterer Schutz bei der Anmeldung.
Wichtig zu wissen: Ein Fingerabdruck allein ist noch keine Zwei-Faktor-Authentifizierung.



 

---

<div class="titel">

# Mein Fazit

</div>
Ich habe mich dafür entschieden, den Samsung Pass genauer zu untersuchen, weil ich von den drei genannten Passwortmanagern diesen am häufigsten verwende, weil ich mein Smartphone öfters nutze als meinen PC. Darum war mir wichtig, herauszufinden, wie gut Samsung Pass meine Passwörter schützt.

<div class="bild">

![alt text](grafik.png)

</div>
<div class="merksatz">
Ich finde, dass Samsung Pass ein guter Passwortmanager ist, der meine Passwörter für mich sicher speichert und mir die Bedienung sehr leicht macht.
</div>

---

# Danke das ich Ihre Zeit in Anspruch nehmen durfte.