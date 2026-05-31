# Chapter Guide: 06 – Evaluation

## Zweck dieser Datei

Diese Datei steuert, wie du bei Aufgaben zu Kapitel 6 vorgehst.
Lies sie vollständig bevor du schreibst, prüfst oder überarbeitest.

---

## Aufgaben die du in diesem Kapitel übernimmst

- Textentwürfe für einzelne Abschnitte auf Basis von Stichpunkten ausformulieren
- Bestehende Abschnitte auf Stil, Wissenschaftlichkeit und Konsistenz prüfen
- Stilmängel und Fehler korrigieren
- Überprüfe ob gewiße Aussagen ohne Quelle getroffen worden sind
- Verwende bei der Nennung von petappoint diesen Still `\textit{petappoint}` im ganzen Kapitel.

Warte auf konkrete Aufgaben. Arbeite immer nur am angefragten Abschnitt.

---

## Struktur & Funktion der Abschnitte

Kapitel 6 umfasst S. 61–70 und bildet die DSR-Phase **Evaluate** ab.
Es überprüft, inwieweit das entwickelte Artefakt (petappoint) die in Kap. 2 definierten Anforderungen erfüllt und wie die Benutzerfreundlichkeit aus Nutzendenperspektive bewertet wird.

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

## Begriffe & Quellen

### Einheitliche Begriffe in diesem Kapitel

| Falsch                                 | Richtig                                           |
|----------------------------------------|---------------------------------------------------|
| Nutzer, Nutzerinnen und Nutzer         | `Nutzende`                                        |
| Tierbesitzer                           | `Tierhalter`                                      |
| System Usability Scale (erste Nennung) | `System Usability Scale (SUS)` — danach nur `SUS` |

### Verwendete Quellen

Entnimm alle konkreten Inhalte immer aus dem aktuellen `.tex`-Text. Die Cite-Keys dienen zur Orientierung:

| Cite-Key                          | Inhalt                           |
|-----------------------------------|----------------------------------|
| `\cite{brooke}`                   | SUS — Originalformel nach Brooke |
| `\cite[S.~161]{susbenchmark2008}` | SUS-Bewertungsskala nach Sauro   |

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