# Chapter Guide: 06 – Evaluation

## Zweck dieser Datei

Diese Datei steuert, wie du bei Aufgaben zu Kapitel 6 vorgehst.
Lies sie vollständig bevor du schreibst, prüfst oder überarbeitest.

---

## Aufgaben die du in diesem Kapitel übernimmst

- Textentwürfe für einzelne Abschnitte auf Basis von Stichpunkten ausformulieren
- Bestehende Abschnitte auf Stil, Wissenschaftlichkeit und Konsistenz prüfen
- Bekannte Fehler und Duplikate auf Anfrage korrigieren

Warte auf konkrete Aufgaben. Arbeite immer nur am angefragten Abschnitt.

---

## Struktur & Funktion der Abschnitte

Kapitel 6 umfasst S. 61–70 und bildet die DSR-Phase **Evaluate** ab.
Es überprüft, inwieweit das entwickelte Artefakt (petappoint) die in Kap. 2 definierten Anforderungen erfüllt und wie die Gebrauchstauglichkeit aus Nutzendenperspektive bewertet wird.

Stelle sicher, dass der folgende logische Fluss erhalten bleibt:

**Methodik → Studiendesign → Datenerhebung → Auswertungsverfahren → Ergebnisse → Diskussion → Limitationen**

### Einleitungsabsatz
- Stelle sicher, dass der Bezug zu Kap. 5 (Implementierung) und Kap. 2 (Anforderungen) explizit hergestellt wird.
- Das Ziel der Evaluation muss klar benannt werden: Überprüfung der Anforderungsabdeckung und Usability.

### §6.1.1 Studiendesign
- Stelle sicher, dass n=20, Plattformaufteilung (10 iOS / 10 Android) und die verwendeten Geräte korrekt benannt werden.
- Die drei Aufgabenszenarien müssen konsistent mit den FA#01–FA#05 aus Kap. 2 sein.
- Stelle sicher, dass SUS beim ersten Auftreten als standardisiertes Instrument eingeführt und mit `\cite{brooke}` belegt wird.
- Prüfe auf Inkonsistenz: Im Einleitungsabsatz werden „drei aufgabenbasierte Szenarien" genannt, aber an anderer Stelle werden „vier Aufgaben" ausgewertet. Kläre und vereinheitliche auf Anfrage.

### §6.1.2 Beschreibung der Datenerhebung
- Stelle sicher, dass quantitative und qualitative Daten klar unterschieden werden.
- Prüfe auf Großschreibungsfehler: Im Text steht „ob Sie die Aufgabe erfolgreich abgeschlossen haben" — „Sie" muss kleingeschrieben werden: „ob sie die Aufgabe erfolgreich abgeschlossen haben."
- Prüfe auf Redundanz: Der demografische Absatz (Alter 16–54, Durchschnitt 31 Jahre) erscheint sowohl in §6.1.2 als auch in §6.2.1 wortgleich. Entferne die Doppelung — entweder in §6.1.2 kürzen oder in §6.2.1 auf §6.1.2 verweisen.
- Verwende „Nutzende" statt „Nutzerinnen und Nutzer".

### §6.1.3 Auswertungsverfahren
- Stelle sicher, dass die SUS-Formel nach Brooke korrekt beschrieben und mit `\cite{brooke}` belegt wird.
- Stelle sicher, dass die Bewertungsskala nach Sauro mit `\cite[S.~161]{susbenchmark2008}` belegt wird.
- Stelle sicher, dass alle drei Auswertungsschritte (SUS-Score, Plattformvergleich, Qualitative Auswertung) in der Einleitung von §6.1.3 angekündigt und dann in eigenen `\subsubsection`-Abschnitten behandelt werden.

### §6.2 Ergebnisse
- Stelle sicher, dass alle Abbildungsreferenzen korrekt gesetzt sind (`\ref{fig:boxplot_aufgaben}`, `\ref{fig:sus_scores}`, `\ref{fig:sus_plattformvergleich}`, `\ref{fig:plattformvergleich}`).
- Prüfe auf doppelten Abschnitt: §6.2.2 „Aufgabenauswertung" erscheint zweimal im Text — der erste Abschnitt enthält nur Fließtext, der zweite enthält zusätzlich die Boxplot-Abbildung. Fasse beide auf Anfrage zu einem einzigen Abschnitt zusammen.
- Prüfe auf doppelten Abschnitt: „Anforderungsabdeckung der funktionalen und nicht-funktionalen Anforderungen" und „Anforderungsabdeckung" erscheinen als zwei separate `\subsection`-Abschnitte — entferne den ersten (leeren) Abschnitt auf Anfrage.
- Beschreibe Ergebnisse sachlich — keine Interpretation hier, diese gehört in §6.3.

### §6.3.1 Interpretation der Ergebnisse
- Stelle sicher, dass alle Ergebnisse aus §6.2 hier interpretiert werden.
- Prüfe auf unbelegte Kausalaussage: „lassen sich eher auf individuelle Unterschiede der Teilnehmenden als auf plattformspezifische Probleme zurückführen" — diese Aussage ist spekulativ. Formuliere auf Anfrage vorsichtiger: „Ein möglicher Erklärungsansatz sind individuelle Unterschiede der Teilnehmenden."
- Stelle sicher, dass der Bezug zur Forschungsfrage am Ende des Abschnitts hergestellt wird.

### §6.3.2 Limitationen
- Stelle sicher, dass alle vier Limitationen vollständig und sachlich beschrieben werden:
  1. Convenience-Stichprobe (persönliches Umfeld)
  2. Nur zwei Testgeräte
  3. Nur Tierhalter-Rolle implementiert
  4. Ausreißer Testperson Nr. 14
- Verwende „Nutzende" statt „Nutzerinnen und Nutzer".
- Formuliere Limitationen ohne Entschuldigungscharakter — sachliche Benennung reicht.

---

## Bekannte Probleme

### Problem 1 – Inkonsistenz: drei vs. vier Aufgaben
Im Einleitungsabsatz steht „drei aufgabenbasierte Szenarien", in §6.2.2 werden aber „vier Aufgaben" ausgewertet (Haustier anlegen, Termin buchen, Termin bearbeiten, Termin stornieren).
→ Kläre auf Anfrage: Aufgabe 1 umfasste zwei Teilaufgaben (Haustier anlegen + Termin buchen), die separat gemessen wurden. Formuliere den Einleitungsabsatz entsprechend um: „drei Szenarien, die in vier Messaufgaben unterteilt wurden."

### Problem 2 – Großschreibung „Sie" (§6.1.2)
Im Text steht „ob Sie die Aufgabe erfolgreich abgeschlossen haben".
→ Korrigiere auf: „ob sie die Aufgabe erfolgreich abgeschlossen haben."

### Problem 3 – Doppelter demografischer Absatz (§6.1.2 und §6.2.1)
Die demografischen Daten (Alter 16–54, Durchschnitt 31 Jahre, Berufsgruppen) erscheinen wortgleich in §6.1.2 und §6.2.1.
→ Entferne auf Anfrage den Absatz in §6.1.2 und verweise stattdessen auf §6.2.1, oder kürze §6.2.1 auf einen Verweis.

### Problem 4 – Doppelter Abschnitt §6.2.2 Aufgabenauswertung
Der Abschnitt „Aufgabenauswertung" erscheint zweimal als `\subsection`.
→ Fasse auf Anfrage beide Abschnitte zu einem einzigen zusammen, der sowohl Fließtext als auch die Boxplot-Abbildung enthält.

### Problem 5 – Doppelter Abschnitt Anforderungsabdeckung
Im Text existieren zwei aufeinanderfolgende `\subsection`-Abschnitte zur Anforderungsabdeckung: „Anforderungsabdeckung der funktionalen und nicht-funktionalen Anforderungen" (ohne Inhalt) und „Anforderungsabdeckung" (mit Inhalt).
→ Entferne auf Anfrage den leeren ersten Abschnitt.

### Problem 6 – Spekulativer Kausalschluss (§6.3.1)
Im Text steht „lassen sich weniger auf plattformspezifische Darstellungsprobleme zurückführen, sondern sind vermutlich auf individuelle Unterschiede zurückzuführen."
→ Formuliere auf Anfrage vorsichtiger: „Ein möglicher Erklärungsansatz für die Unterschiede in den Bearbeitungszeiten sind individuelle Unterschiede der Teilnehmenden."

### Problem 7 – „Nutzerinnen und Nutzer" (§6.3.2)
Im Limitationen-Abschnitt steht „unbekannte Nutzerinnen und Nutzer".
→ Ersetze durch „unbekannte Nutzende."

---

## Begriffe & Quellen

### Einheitliche Begriffe in diesem Kapitel

| Falsch | Richtig |
|---|---|
| Nutzer, Nutzerinnen und Nutzer | `Nutzende` |
| Tierbesitzer | `Tierhalter` |
| System Usability Scale (erste Nennung) | `System Usability Scale (SUS)` — danach nur `SUS` |

### Verwendete Quellen

Entnimm alle konkreten Inhalte immer aus dem aktuellen `.tex`-Text. Die Cite-Keys dienen zur Orientierung:

| Cite-Key | Inhalt |
|---|---|
| `\cite{brooke}` | SUS — Originalformel nach Brooke |
| `\cite[S.~161]{susbenchmark2008}` | SUS-Bewertungsskala nach Sauro |

---

## Grenzen dieses Kapitels

Füge folgende Inhalte **nicht** in Kapitel 6 ein — sie gehören in andere Kapitel:

- Implementierungsdetails → Kap. 5
- Anforderungsdefinitionen (FA#, NFA#) → Kap. 2 (nur referenzieren, nicht neu definieren)
- Fazit und Beantwortung der Forschungsfrage → Kap. 7

Umfang: S. 61–70 (ca. 10 Seiten).

---

## DSR-Prüfung

Prüfe bei jeder Überarbeitung, ob folgende DSR-Kriterien erfüllt sind:

- Das Kapitel ist klar der DSR-Phase **Evaluate** zuzuordnen: Das Artefakt wird systematisch anhand der definierten Anforderungen bewertet.
- Die Evaluationsmethode (aufgabenbasierte Nutzerstudie + SUS) ist nachvollziehbar begründet.
- Ergebnisse und Interpretation sind klar getrennt — Ergebnisse in §6.2, Interpretation in §6.3.
- Limitationen werden offen und sachlich kommuniziert — das stärkt die wissenschaftliche Glaubwürdigkeit.
- Die Anforderungsabdeckungstabellen (FA#01–FA#07, NFA#01–NFA#05) stellen den direkten Bezug zu Kap. 2 her.
- Der evaluative Teil der Forschungsfrage wird in §6.3.1 explizit adressiert.