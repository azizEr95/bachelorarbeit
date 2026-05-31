# Chapter Guide: 04 – Technische Grundlagen

## Zweck dieser Datei

Diese Datei steuert, wie du bei Aufgaben zu Kapitel 4 vorgehst.
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

Kapitel 4 umfasst S. 40–48 und bildet die DSR-Phase **Design** ab.
Es begründet die Technologieauswahl für das Frontend auf Basis der Anforderungen aus Kap. 2 und der Konzeption aus Kap. 3.

Stelle sicher, dass der folgende logische Fluss erhalten bleibt:

**Backend-Technologien (Überblick) → Framework-Vergleich → Expo → Server-State → Client-State → UI-Bibliothek → Internationalisierung → Zusammenspiel**

Jeder Vergleichsabschnitt folgt demselben Muster:
1. Kandidaten vorstellen (neutral, belegt)
2. Jeweils Vor- und Nachteile nennen
3. Begründung der Wahl für petappoint

### Einleitungsabsatz
- Stelle sicher, dass der Bezug zu Kap. 3 explizit hergestellt wird.
- Der Absatz soll knapp ankündigen, was in diesem Kapitel behandelt wird.

### §4.1 Technologien im bereits bestehenden Backend
- Beschreibe die Backend-Technologien sachlich als gegebene Grundlage — keine erneute Begründung nötig, da das Backend eine Vorleistung ist.
- Stelle sicher, dass alle Technologien in der Tabelle mit den im Fließtext genannten übereinstimmen.
- ACID muss beim ersten Auftreten definiert und mit `\cite{postgresql_transactions}` belegt werden.

### §4.2 Plattformübergreifende Frameworks
- Stelle sicher, dass alle drei Kandidaten (React Native, Flutter, .NET MAUI) nach demselben Schema beschrieben werden: Herkunft, Grundprinzip, Vorteile, Nachteile.
- Beschreibe jeden Kandidaten sachlich und ohne Vorab-Wertung — die Wertung erfolgt ausschließlich in §4.2.4.
- Stelle sicher, dass .NET MAUI als Nachfolger von Xamarin korrekt eingeordnet wird (Support eingestellt Mai 2024).

### §4.3 Expo
- Stelle sicher, dass Expo als Folgeentscheidung aus der React-Native-Wahl begründet wird.
- Expo Router, Development Build und Expo SDK müssen als separate Konzepte klar voneinander abgegrenzt werden.

### §4.4 Server-State-Management
- Stelle sicher, dass alle drei Kandidaten (TanStack Query, SWR, RTK Query) nach demselben Schema beschrieben werden.
- Das Stale-While-Revalidate-Prinzip muss beim ersten Auftreten klar definiert werden.
- Stelle sicher, dass Prinzip (Stale-While-Revalidate) und Bibliothek (SWR von Vercel) klar voneinander unterschieden werden.

### §4.5 Client-State-Management
- Stelle sicher, dass beide Kandidaten (Zustand, Redux Toolkit) nach demselben Schema beschrieben werden.
- Stelle sicher, dass die Abgrenzung zwischen Client-State und Server-State klar bleibt.

### §4.6 UI-Komponentenbibliotheken
- Stelle sicher, dass alle drei Kandidaten (Gluestack UI, React Native Paper, StyleSheet) nach demselben Schema beschrieben werden.
- StyleSheet ist keine externe Bibliothek — stelle sicher, dass das im Text klar benannt wird.
- Stelle sicher, dass der Token-Begriff beim ersten Auftreten kurz erklärt wird.

### §4.7 Internationalisierung
- Stelle sicher, dass beide Kandidaten (i18next, react-intl) nach demselben Schema beschrieben werden.
- Stelle sicher, dass der Begründungsabschnitt als eigener `\subsection` vorhanden ist.

### §4.8 Zusammenspiel der gewählten Technologien
- Stelle sicher, dass alle gewählten Technologien erwähnt werden.
- Keine neuen Argumente einführen — bestehende zusammenführen.
- Stelle sicher, dass die abschließende Tabelle alle Frontend-Technologien vollständig auflistet.

---

## Begriffe & Quellen

### Einheitliche Begriffe in diesem Kapitel

| Falsch         | Richtig                                    |
|----------------|--------------------------------------------|
| cross-platform | `plattformübergreifend`                    |
| Nutzer         | `Nutzende`                                 |
| Xamarin        | Nur als Vorgänger von `.NET MAUI` erwähnen |

### Verwendete Quellen

Entnimm alle konkreten Inhalte immer aus dem aktuellen `.tex`-Text. Die Cite-Keys dienen zur Orientierung:

| Cite-Key                         | Inhalt                               |
|----------------------------------|--------------------------------------|
| `\cite{nodejs-docs}`             | Node.js Dokumentation                |
| `\cite{express-docs}`            | Express Dokumentation                |
| `\cite{postgresql_transactions}` | PostgreSQL — ACID-Eigenschaften      |
| `\cite{postgresql_about}`        | PostgreSQL — allgemeine Beschreibung |
| `\cite{typescript-docs}`         | TypeScript Dokumentation             |
| `\cite{zod-docs}`                | Zod Dokumentation                    |
| `\cite{brevo-docs}`              | Brevo — E-Mail-Dienst                |
| `\cite{react-native-docs}`       | React Native Dokumentation           |
| `\cite{react-native-new-arch}`   | React Native neue Architektur / JSI  |
| `\cite{flutter-docs}`            | Flutter Dokumentation                |
| `\cite{maui-docs}`               | .NET MAUI Dokumentation              |
| `\cite{expo-docs}`               | Expo Dokumentation                   |
| `\cite{expo-router}`             | Expo Router                          |
| `\cite{expo-build}`              | Expo Development Build / SDK         |
| `\cite{expo-service}`            | Expo Secure Store                    |
| `\cite{tanstack-query-docs}`     | TanStack Query Dokumentation         |
| `\cite{swr-docs}`                | SWR Dokumentation                    |
| `\cite{redux-toolkit-docs}`      | Redux Toolkit Dokumentation          |
| `\cite{zustand-docs}`            | Zustand Dokumentation                |
| `\cite{gluestack-docs}`          | Gluestack UI Dokumentation           |
| `\cite{react-native-paper-docs}` | React Native Paper Dokumentation     |
| `\cite{i18n-docs}`               | i18next Dokumentation                |
| `\cite{react-intl-docs}`         | react-intl Dokumentation             |
| `\cite{galitz2002}`              | UI-Elemente — Definition             |

---

## Grenzen dieses Kapitels

Füge folgende Inhalte **nicht** in Kapitel 4 ein — sie gehören in spätere Kapitel:

- Konkrete Implementierungsdetails → Kap. 5
- Evaluationsergebnisse → Kap. 6
- Architekturentscheidungen → Kap. 3
- Anforderungsdefinitionen (FA#, NFA#) → Kap. 2

Umfang: S. 40–48 (ca. 9 Seiten).

---

## DSR-Prüfung

Prüfe bei jeder Überarbeitung, ob folgende DSR-Kriterien erfüllt sind:

- Das Kapitel ist klar der DSR-Phase **Design** zuzuordnen: Technologieentscheidungen werden nachvollziehbar aus den Anforderungen abgeleitet.
- Jede Technologieentscheidung ist explizit begründet — keine Auswahl ohne Argumentation.
- Alle Begründungsabschnitte referenzieren die Anforderungen aus Kap. 2 oder die Konzeption aus Kap. 3 wo relevant.
- §4.8 macht das Zusammenspiel als kohärenten Stack sichtbar — das stärkt die Nachvollziehbarkeit der Designentscheidungen.

@guides/stil.md