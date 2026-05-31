# Chapter Guide: 01 – Einleitung

## Zweck dieser Datei

Diese Datei steuert, wie du bei Aufgaben zu Kapitel 1 vorgehst.
Lies sie vollständig bevor du schreibst, prüfst oder überarbeitest.

---

## Aufgaben die du in diesem Kapitel übernimmst

- Textentwürfe für einzelne Abschnitte auf Basis von Stichpunkten ausformulieren
- Bestehende Abschnitte auf Stil, Wissenschaftlichkeit und Konsistenz prüfen
- Den fehlenden „Aufbau der Arbeit"-Absatz am Ende von §1.6 ausformulieren (siehe unten)
- Begriffsfehler und stilistische Mängel auf Anfrage korrigieren

Warte auf konkrete Aufgaben. Arbeite immer nur am angefragten Abschnitt.

---

## Struktur & Funktion der Abschnitte

Kapitel 1 umfasst S. 1–4 und führt vom allgemeinen Kontext zur konkreten Forschungsfrage.
Stelle sicher, dass der folgende logische Fluss erhalten bleibt:

**Digitalisierung allgemein → Veterinärmarkt → Problemlücke → bestehende Systeme → Abgrenzung petappoint → Forschungsfrage**

### §1.1 Hintergrund und Motivation
- Stelle sicher, dass der Abschnitt vom Allgemeinen (Digitalisierung, Humanmedizin) zum Konkreten (Veterinärmarkt) führt.
- Alle Marktdaten müssen mit `\cite{}` belegt sein. Keine unbelegten Zahlen einfügen.
- Doctolib dient als Vergleichsreferenz für den Reifegrad digitaler Terminlösungen in der Humanmedizin — nicht als Vorbild für petappoint.

### §1.2 Problemstellung
- Stelle sicher, dass die Problemlücke explizit benannt wird: Es fehlt eine fokussierte, plattformübergreifende Terminverwaltungslösung im Veterinärbereich.
- Der Abschnitt darf keine Lösung vorwegnehmen — keine Erwähnung von petappoint hier.
- Verwende ausschließlich `.NET MAUI`, nicht `Xamarin` (veraltet). Falls `Xamarin` im Text vorkommt, ersetze es durch `.NET MAUI`.

### §1.3 Terminverwaltungen im Veterinärbereich
- Stelle sicher, dass die zwei Markttypen klar unterschieden werden: reine Buchungslösungen vs. vollständige Praxismanagementsysteme.
- Keine Detailbeschreibungen einzelner Systeme hier — diese folgen in §1.4.

### §1.4 Ausgewählte Systeme im Vergleich (§1.4.1–1.4.3)
- Halte die Reihenfolge ein: petsXL (§1.4.1) → petLeo (§1.4.2) → vetpraxis (§1.4.3).
- Beschreibe jedes System sachlich und belegt. Keine wertenden Adjektive wie „leistungsstark" oder „modern".
- Jedes System muss mit seinem `\cite{}`-Key referenziert werden (siehe Quellentabelle unten).

### §1.5 Abgrenzung petappoint
- Stelle sicher, dass die drei Alleinstellungsmerkmale von petappoint klar benannt werden: (1) Fokus ausschließlich auf Terminverwaltung, (2) Softwareunabhängigkeit, (3) kostenlose Nutzung für beide Seiten.
- Keine Implementierungsdetails — diese folgen in Kap. 5.
- Verwende `\textit{petappoint}` bei der ersten Nennung im Abschnitt.

### §1.6 Zielsetzung
- Stelle sicher, dass die Forschungsfrage **ausschließlich hier** wörtlich zitiert wird — nicht in anderen Abschnitten.
- DSR nach Hevner 2004 muss explizit genannt und kurz begründet werden.
- Der Scope muss klar abgegrenzt werden: Eigenleistung umfasst Frontend + Backend-Integration; das Backend war eine Vorleistung aus einem vorangegangenen Projektmodul.
- Am Ende von §1.6 fehlt noch der „Aufbau der Arbeit"-Absatz (siehe TODO unten).

---

## Offene Aufgaben

### Aufgabe 1 – „Aufbau der Arbeit"-Absatz (§1.6, Ende)
Wenn du gebeten wirst, diesen Absatz zu schreiben, formuliere eine kurze Kapitelübersicht mit je einem Satz pro Kapitel (Kap. 1–7). Entnimm die Kapitelinhalte aus der Kapitelstruktur der Master-Datei. Der Absatz endet mit dem Satz: „…womit die Forschungsfrage abschließend beantwortet wird."

### Aufgabe 2 – Begriffsfehler
Im Fließtext kommt einmalig „Tierbesitzern" vor. Ersetze es durch „Tierhaltern" wenn du auf Anfrage den betreffenden Abschnitt überarbeitest.

### Aufgabe 3 – Stilredundanz
Im Text kommt die Formulierung „Als Basis dieser Arbeit basiert das Backend…" vor. Formuliere sie auf Anfrage um, z.B.: „Das Backend von petappoint, das im Rahmen eines vorangegangenen Projektmoduls in Teamarbeit entwickelt wurde, bildet die technische Grundlage dieser Arbeit."

---

## Begriffe & Quellen

### Einheitliche Begriffe in diesem Kapitel

| Falsch | Richtig |
|---|---|
| petAppoint, PetAppoint | `petappoint` |
| Tierbesitzer, Haustierbesitzer | `Tierhalter` |
| Appointment Management | `Terminverwaltung` |
| Xamarin | `.NET MAUI` |
| Petleo | `petLeo` |

### Verwendete Quellen

Entnimm alle konkreten Zahlen und Fakten immer aus dem aktuellen `.tex`-Text, nicht aus dieser Datei. Die Cite-Keys dienen zur Orientierung:

| Cite-Key | Inhalt |
|---|---|
| `\cite{doctolibreport}` | Doctolib Wachstumsbericht |
| `\cite{btk2025}` | Bundestierärztekammer 2025 — Anzahl Tierärzte in Deutschland |
| `\cite{vsmreport}` | Veterinary Software Market Report — Marktgröße + Wachstum |
| `\cite{doctolib2020}` | Anteil mobiler Online-Buchungen |
| `\cite{diez2023}` | Umfrage Tierhalter — Online-Präferenz + Wartezeiten (S. 69) |
| `\cite{petleo-info}` | petLeo Produktinformation |
| `\cite{petsxl-info}` | petsXL Produktinformation |
| `\cite{vetpraxis-info}` | vetpraxis Produktinformation |
| `\cite{hevner2004}` | Design Science Research Methodik |

---

## Grenzen dieses Kapitels

Füge folgende Inhalte **nicht** in Kapitel 1 ein — sie gehören in spätere Kapitel:

- Implementierungsdetails → Kap. 5
- Evaluationsergebnisse → Kap. 6
- Technologievergleiche (React Native, Flutter, .NET MAUI) → Kap. 4
- Anforderungsdefinitionen (FA#, NFA#) → Kap. 2

Umfang: max. 4 Seiten.

---

## DSR-Prüfung

Prüfe bei jeder Überarbeitung, ob folgende DSR-Kriterien erfüllt sind:

- Der Problemraum ist klar als DSR-Phase **Analyze** erkennbar: Ein praxisrelevantes Problem wird identifiziert und mit Daten belegt.
- Alle drei Teile der Forschungsfrage sind im Kapitel motiviert — auch wenn sie nicht explizit genannt werden:
  - **Konzipieren** → Marktlücke belegt, Abgrenzung definiert
  - **Umsetzen** → Plattformübergreifender Bedarf begründet
  - **Evaluieren** → Nutzerwunsch nach Benutzerfreundlichkeit als Qualitätskriterium erkennbar
- DSR nach Hevner 2004 wird in §1.6 explizit eingeführt und begründet.
- Das Artefakt (petappoint) wird benannt, aber noch nicht definiert — das folgt in Kap. 3–5.