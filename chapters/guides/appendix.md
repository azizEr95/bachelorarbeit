# Chapter Guide: Anhang (appendix)

## Zweck dieser Datei

Diese Datei steuert, wie du bei Aufgaben zum Anhang vorgehst.
Lies sie vollständig bevor du schreibst, prüfst oder überarbeitest.

---

## Aufgaben die du in diesem Kapitel übernimmst

- Bestehende Abschnitte auf Stil, Konsistenz und korrekte Referenzierung prüfen
- Stilmängel und Fehler korrigieren
- Überprüfe ob gewiße Aussagen ohne Quelle getroffen worden sind
- Verwende bei der Nennung von petappoint diesen Still `\textit{petappoint}` im ganzen Kapitel.

Warte auf konkrete Aufgaben. Arbeite immer nur am angefragten Abschnitt.

---

## Struktur & Funktion der Abschnitte

Der Anhang gliedert sich in drei Kapitel:

- **Anhang A** – Zusätzliche Abbildungen (`\label{appendix:abbildungen}`)
- **Anhang B** – Fragebogen der Nutzerstudie (`\label{appendix:fragebogen}`)
- **Anhang C** – Rohdaten der Nutzerstudie (`\label{appendix:rohdaten}`)

### Anhang A – Zusätzliche Abbildungen
- Stelle sicher, dass alle vier Abbildungen korrekt referenziert sind — die Labels werden in Kap. 5 verwendet:
  - `\label{fig:anhang_authentication}` → referenziert in §5.5.3
  - `\label{fig:anhang_tab-light}` → referenziert in §5.5.3
  - `\label{fig:anhang_tab-dark}` → referenziert in §5.5.3
  - `\label{fig:anhang_booking-process}` → referenziert in §5.5.3
- Stelle sicher, dass die Bildunterschriften konsistent mit den Beschreibungen in §5.5.3 sind.

### Anhang B – Fragebogen der Nutzerstudie
- Stelle sicher, dass der einleitende Absatz die Gesamtzahl der Fragen (33) und die fünf Abschnitte korrekt benennt — konsistent mit §6.1.2.
- Die fünf Abschnitte müssen mit den in §6.1.2 genannten übereinstimmen:
  1. Allgemeine App-Erfahrung
  2. Aufgabenbezogene Fragen
  3. System Usability Scale
  4. Plattformwahrnehmung
  5. Offene Fragen
- Abschnittsüberschriften verwenden `\section*{}` (ohne Nummerierung) — das ist korrekt und soll so bleiben.

### Anhang C – Rohdaten der Nutzerstudie
- Stelle sicher, dass alle drei Rohdaten-Links korrekt und vollständig sind.
- Prüfe auf Begriffsfehler: Im Text steht „SUS-Scores jedes einzelnen Teilnehmer" — fehlender Genitiv-s und nicht geschlechtsneutral. Korrigiere auf Anfrage auf: „SUS-Scores der einzelnen Teilnehmenden".
- Prüfe auf fehlende Beschriftung: Die CSV- und Excel-Dateien sind zwar verlinkt, aber nicht mit `\caption` oder ähnlichem beschriftet — das ist im Anhang akzeptabel, da sie als Listenelemente dargestellt werden.

---

## Begriffe & Quellen

### Einheitliche Begriffe im Anhang

| Falsch                    | Richtig        |
|---------------------------|----------------|
| Teilnehmer (ohne Kontext) | `Teilnehmende` |
| Nutzer                    | `Nutzende`     |

### Verwendete Quellen

Der Anhang enthält keine `\cite{}`-Referenzen. Externe Daten werden über URLs verlinkt.

---

## Grenzen des Anhangs

Der Anhang enthält ausschließlich ergänzendes Material — keine inhaltlichen Aussagen oder Interpretationen. Füge keine neuen Argumente oder Schlussfolgerungen ein.

Verweise aus dem Haupttext auf den Anhang erfolgen ausschließlich über `\ref{appendix:abbildungen}`, `\ref{appendix:fragebogen}` oder `\ref{appendix:rohdaten}`.