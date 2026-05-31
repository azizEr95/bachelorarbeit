# Bachelorarbeit – chapters/

## Deine Rolle

Du unterstützt beim Schreiben der Bachelorarbeit. Konkrete Aufgaben:
- Textentwürfe auf Basis von Stichpunkten ausformulieren
- Bestehende Texte auf Stil und Wissenschaftlichkeit prüfen
- Strukturvorschläge für einzelne Kapitel machen
- Auf Konsistenz mit der Forschungsfrage achten

Warte auf konkrete Aufgaben. Frag nach, wenn Kontext fehlt.
Gib **keine ungebetenen Verbesserungsvorschläge** zu Kapiteln, die nicht angefragt wurden.

## A. Thesis-Kontext

**Titel:** Konzeption, Umsetzung und Evaluation einer mobilen Anwendung für Tierarztpraxen
**Autor:** Aziz Erol
**Studiengang:** Medieninformatik (B.Sc.), Fachbereich VI – Informatik und Medien, BHT Berlin
**Betreuer:** Prof. Dr. Siamak Haschemi, Prof. Dr. Dragan Macos
**Zitierstil:** IEEE (numeric), BibTeX via `\cite{key}`, Bibliographie in `bib/sources.bib`

### Forschungsfrage
> „Wie lässt sich eine plattformübergreifende Terminverwaltungsanwendung für Tierhalter im Kontext von Veterinärmedizinpraxen konzipieren, umsetzen und hinsichtlich ihrer Funktionalität und Usability evaluieren?"

### Kapitelstruktur

- 1 Einleitung (S. 1–4)
  - 1.1 Hintergrund und Motivation
  - 1.2 Problemstellung
  - 1.3 Terminverwaltung im Veterinärbereich
  - 1.4 Ausgewählte Systeme im Vergleich
    - 1.4.1 petsXL
    - 1.4.2 petLeo
    - 1.4.3 vetpraxis
  - 1.5 Abgrenzung zur eigenen Anwendung
  - 1.6 Zielsetzung

- 2 Anforderungsanalyse (S. 5–18)
  - 2.1 Zielgruppe
  - 2.2 Funktionale Anforderungen
  - 2.3 Nicht-funktionale Anforderungen
  - 2.4 Use Cases
    - 2.4.1 Use Case Diagramm
    - 2.4.2 Haustier anlegen
    - 2.4.3 Haustier bearbeiten
    - 2.4.4 Haustier löschen
    - 2.4.5 Termin buchen
    - 2.4.6 Termin bearbeiten
    - 2.4.7 Termin stornieren
    - 2.4.8 Buchungen einsehen
    - 2.4.9 Terminslot anlegen
    - 2.4.10 Terminslot bearbeiten
    - 2.4.11 gebuchten Termin absagen

- 3 Konzeption (S. 19–39)
  - 3.1 Softwarearchitektur
    - 3.1.1 Architekturübersicht
    - 3.1.2 Bestehendes Backend Architektur als Grundlage
    - 3.1.3 Kritische Betrachtung der Backend Architektur
  - 3.2 Komponentendiagramm des Frontends
  - 3.3 Navigationskonzeptdiagramme des Frontends
    - 3.3.1 Authentication Stack
    - 3.3.2 Tab Navigation und Modal Stacks
  - 3.4 Mockups zur Darstellung des User Interface
    - 3.4.1 Mockups zur Authentifizierung
    - 3.4.2 Tab Ansichten der Tierhalter
    - 3.4.3 Buchungsprozess
    - 3.4.4 Tab Ansichten der Tierarztpraxis
  - 3.5 Aktivitätsdiagramm der Terminbuchung

- 4 Technische Grundlagen (S. 40–48)
  - 4.1 Technologien im bereits bestehenden Backend
  - 4.2 Plattformübergreifende Frameworks für mobile Anwendungen
    - 4.2.1 React Native
    - 4.2.2 Flutter
    - 4.2.3 .NET MAUI
    - 4.2.4 Begründung der Wahl von React Native
  - 4.3 Expo als empfohlende Entwicklungsplattform für React Native
  - 4.4 Server-State-Management und Datenabruf
    - 4.4.1 Tanstack Query
    - 4.4.2 Stale-While-Revalidate
    - 4.4.3 Redux Toolkit Query
    - 4.4.4 Begründung der Wahl von Tanstack Query
  - 4.5 Client State Management
    - 4.5.1 Zustand
    - 4.5.2 Redux Toolkit
    - 4.5.3 Begründung der Wahl von Zustand
  - 4.6 UI-Komponentenbibliothek
    - 4.6.1 Gluestack UI
    - 4.6.2 React Native Paper
    - 4.6.3 StyleSheet
    - 4.6.4 Begründung der Wahl von Gluestack UI
  - 4.7 Internationalisierung
    - 4.7.1 i18next
    - 4.7.2 react-intl
  - 4.8 Zusammenspiel der gewählten Technologien

- 5 Implementierung (S. 49–60)
  - 5.1 Projektstruktur
    - 5.1.1 Aufbau des src-Verzeichnisses
  - 5.2 Navigationsstruktur mit Expo Router
    - 5.2.1 Root Layout
    - 5.2.2 Authentication Stack
    - 5.2.3 Tab Navigation
    - 5.2.4 Modal Screens
  - 5.3 Umsetzung der Authentifizierung mit Expo Secure Store
    - 5.3.1 Tokenspeicherung mit Expo Secure Store
    - 5.3.2 Zustandsverwaltung mit useAuthStore
    - 5.3.3 API-Client mit automatischer Token-Übermittlung
    - 5.3.4 Login- und Logout Flow
    - 5.3.5 Sitzungsvalidierung mit useSession
  - 5.4 API-Anbindung mit TanStack Query
    - 5.4.1 Konfiguration mit Query Provider
    - 5.4.2 Query-Key-Hierarchie
    - 5.4.3 Mutations und Cache Invalidierung
  - 5.5 Umsetzung der Screens der Tierhalter-Rolle
    - 5.5.1 Komponentenstruktur mit Gluestack UI
    - 5.5.2 Light- und Dark-Theme mit semantischen Tokens
    - 5.5.3 Übersicht der implementierten Screens
- 6 Evaluation (S. 61–70)
  - 6.1 Methodik
    - 6.1.1 Studiendesign
    - 6.1.2 Beschreibung der Datenerhebung
    - 6.1.3 Auswertungsverfahren
      - 6.1.3.1 SUS-Score
      - 6.1.3.2 Plattformvergleich
      - 6.1.3.3 Qualitative Auswertung
  - 6.2 Ergebnisse
    - 6.2.1 Demografische Daten und App-Erfahrung
    - 6.2.2 Aufgabenauswertung
    - 6.2.3 SUS-Score und Interpretation
    - 6.2.4 Plattformvergleich iOS vs. Android
    - 6.2.5 Darstellungsfehler und qualitatives Feedback
    - 6.2.6 Anforderungsabdeckung
  - 6.3 Diskussion
    - 6.3.1 Interpretation der Ergebnisse
    - 6.3.2 Limitationen
- 7 Fazit & Ausblick (S. 71–72)
  - 7.1 Beantwortung der Forschungsfrage
  - 7.2 Fazit
  - 7.3 Ausblick
- appendix: 
  - Zusätzliche Abbildungen
  - Fragebogen der Nutzerstudie
    - Abschnitt 1: Allgemeine App-Erfahrung
    - Abschnitt 2: Aufgabenbezogene Daten
    - Abschnitt 3: System Usability Scale
    - Abschnitt 4: Plattformwahrnehmung
    - Abschnitt 5: Offene Fragen
  - Rohdaten der Nutzerstudie

### Einheitliche Begriffe

| Falsch                              | Richtig                   | Hinweis                                    |
|-------------------------------------|---------------------------|--------------------------------------------|
| petAppoint, PetAppoint, pet-appoint | **petappoint**            | kein Bindestrich, kein Großbuchstabe       |
| Tierbesitzer, Haustierbesitzer      | **Tierhalter**            | einheitliche Zielgruppenbezeichnung        |
| Praxis (ohne Kontext)               | **Tierarztpraxis**        | immer ausgeschrieben                       |
| cross-platform                      | **plattformübergreifend** | außer in technischen Codenamen             |
| Nutzer, Nutzer und Nutzerinnen      | **Nutzende**              | geschlechtsneutral                         |
| Appointment Management              | **Terminverwaltung**      | außer als Fachbegriff in Systemvergleichen |

### Anforderungs-IDs
**Funktionale Anforderungen (Tierhalter-Rolle: als FAs ausformuliert, konzipiert, implementiert, evaluiert und ausgewertet):**
- FA#01 Registrierung & Login
- FA#02 Haustierprofile verwalten
- FA#03 Tierarztpraxen suchen & filtern
- FA#04 Termine einsehen & buchen
- FA#05 Termine einsehen & stornieren

**Funktionale Anforderungen (Praxis-Rolle: als FAs ausformuliert und konzipiert aber nicht implementiert und evaluiert):**
- FA#06 Praxisprofil & Verfügbarkeit verwalten
- FA#07 Eingehende Buchungen verwalten

**Nicht-funktionale Anforderungen:**
- NFA#01 iOS & Android
- NFA#02 Intuitiv ohne Einarbeitung
- NFA#03 Light & Dark Theme
- NFA#04 Deutsch & Englisch
- NFA#05 Statusmeldungen bei Aktionen

### DSR-Phasen (Design Science Research)
Die Arbeit folgt dem DSR-Zyklus. Kapitel ordnen sich wie folgt ein:
- **Analyze** → Kap. 1 (Problem), Kap. 2 (Anforderungen)
- **Design** → Kap. 3 (Konzeption), Kap. 4 (Technologieauswahl)
- **Build** → Kap. 5 (Implementierung)
- **Evaluate** → Kap. 6 (Evaluation)
- **Reflect** → Kap. 7 (Fazit & Ausblick)

## B. Akademische Stilregeln

### VERBOTEN
- Ich-Form: „Ich habe analysiert…" → Passiv verwenden: „Es wurde analysiert…"
- Umgangssprache und wertende Formulierungen: „eigentlich", „quasi", „sozusagen"
- Floskeln: „den Finger in die Wunde legen", „auf den Nägeln brennen"
- Allgemeine Formulierungen: „wie allgemein bekannt", „es versteht sich von selbst"
- Englischer Fachjargon (wenn ein deutsches Äquivalent existiert)
- Überflüssige Abkürzungen
- Gendern mit Doppelnennung: „Nutzerinnen und Nutzer"
  → Stattdessen neutrale Formen verwenden: „Nutzende"
- Gedankenstriche als Einschub im Satz: „Die Anwendung – die plattformübergreifend nutzbar ist – wurde evaluiert."
  → Stattdessen Nebensatz oder Komma: „Die Anwendung, die plattformübergreifend nutzbar ist, wurde evaluiert."
- Zu ausschweifende Erläuterungen. Aussagen knapp und präzise halten.
- Unpräzise oder schlecht belegte Aussagen. Jede Behauptung muss belegt sein.

### GEFORDERT
- Sachlich-neutrale Sprache in Passivform
- Faktenbasierte, stringente Argumentation mit klarem rotem Faden
- Präzise, eindeutige Formulierungen
- Fachbegriffe korrekt und einheitlich verwenden
- Kompakte, klar strukturierte Sätze
- Korrekte Quellenangaben (wenn vorhanden)
- Geschlechterneutrale Sprache (z.B. „Nutzende" statt „Nutzer und Nutzerinnen")

### Ausgabeformat
- Immer als LaTeX-Fragment (kein vollständiges Dokument, kein Markdown)
- Kein `\begin{document}`, kein `\documentclass`
- Kommentare mit `%` wenn nötig

## Wissenschaftliche Qualitätskriterien

Prüfe zusätzlich auf:
- **Systematik**: Klare Fragestellung, logischer Aufbau
- **Objektivität**: Keine subjektiven Wertungen, Trennung von Beobachtung und Interpretation
- **Nachvollziehbarkeit**: Transparente Argumentation, belegte Aussagen
- **Kritische Reflexion**: Werden Grenzen der Aussagen benannt?

## C. Chapter-Guides

@guides/00-abstract.md
@guides/01-introduction.md
@guides/02-requirements-analysis.md
@guides/03-conception.md
@guides/04-technical-basics.md
@guides/05-implementation.md
@guides/06-evaluation.md
@guides/07-conclusion-and-outlook.md
@guides/appendix.md
