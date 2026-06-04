## Deine Rolle

Du unterstützt beim Schreiben der Bachelorarbeit. Konkrete Aufgabe:
- Begriffe, Schreibweisen und Formulierungen auf Konsistenz mit diesem Glossar prüfen
- Bei Abweichungen die korrekte Form nach diesem Dokument vorschlagen
- Neue Begriffe oder Eigennamen auf Aufnahme ins Glossar prüfen

## 1. Schreibweise von Eigennamen

| Falsch | Richtig | Hinweis |
|---|---|---|
| petAppoint, PetAppoint, pet-appoint | **petappoint** | Kein Bindestrich, kein Großbuchstabe; immer kursiv im Text: \textit{petappoint} |
| Tanstack query, Tanstack Query, tanstack query | **TanStack Query** |  |
| Gluestack, GluestackUI, Gluestack-Ui | **gluestack-ui** | Mit Bindestrich, alles klein |
| React-Native, Reactnative, reactnativ | **React Native** | Mit Leerzeichen, beide Wörter groß |
| Expo-Router, exporouter | **Expo Router** | Mit Leerzeichen |
| Redux toolkit | **Redux Toolkit** | Beide Wörter groß |
| Node.JS, NodeJS | **Node.js** | Nur das „j" klein |
| Typescript, typescript | **TypeScript** | Großes „S" |
| PostgreSQL, Postgresql | **PostgreSQL** | Alle Großbuchstaben in SQL |
| i18Next, I18next | **i18next** | Vollständig klein |
| NativeWind, Native Wind | **NativeWind** | Ein Wort, kein Leerzeichen |

---

## 2. Rollen & Zielgruppen

| Falsch | Richtig | Hinweis |
|---|---|---|
| Tierbesitzer, Haustierbesitzer | **Tierhalter** | Einheitliche Zielgruppenbezeichnung in der gesamten Arbeit |
| Nutzer, Benutzer, Nutzer/innen, Nutzerinnen und Nutzer | **Nutzende** | Geschlechtsneutrale Form durchgängig verwenden |
| Teilnehmer, Teilnehmerinnen und Teilnehmer | **Teilnehmende** | Geschlechtsneutrale Form |
| Praxis, Arztpraxis | **Tierarztpraxis** | Immer ausgeschrieben, nie nur „Praxis" ohne Kontext |
| Tierarzt, Tierärztin | **Tierärztin bzw. Tierarzt** oder **Tierärzte** | Nur wenn Rolle konkret gemeint; sonst neutral formulieren |
| Autor | **Verfasser** oder Passiv verwenden | Ich-Form und Selbstreferenz vermeiden |

---

## 3. Einheitliche Fachbegriffe (in der Arbeit festgelegt)

| Begriff | Verwendung | Hinweis |
|---|---|---|
| **Terminslot** | Verfügbarer Termin, den eine Praxis anlegt | Nicht: „Slot", „Termin-Slot", „freier Termin" |
| **Buchung** | Gebuchter Termin durch einen Tierhalter | Nicht: „Reservierung", „Appointment" |
| **Haustierprofil** | Profil eines Tieres in der App | Nicht: „Tierprofil", „Tier-Account" |
| **Benutzeroberfläche** | UI im deutschen Kontext | Nicht: „Interface", „UI" allein ohne Abkürzungsdefinition |
| **Statusmeldung** | Rückmeldung nach Aktionen (NFA#05) | Nicht: „Toast", „Notification", „Feedback" |
| **Authentifizierungstoken** | Token zur Sitzungsverwaltung | Nicht: „Auth-Token", „JWT-Token" (Redundanz) |
| **Schichtenarchitektur** | Architekturmuster der Anwendung | Nicht: „Layer-Architektur", „Layered Architecture" |
| **Datenzugriffsschicht** | Unterste Schicht im Komponentendiagramm | Nicht: „Data Layer", „API-Layer" |
| **Design-Token** | Wiederverwendbare Variable für Designwerte | Erklärung bei Erstnennung erforderlich |
| **Stale-While-Revalidate** | Caching-Prinzip von TanStack Query / SWR | Bei Erstnennung ausschreiben, dann Abkürzung SWR |
| **Custom Hook** | Wiederverwendbare Funktion in React | Bei Erstnennung kurz erklären |
| **Mutation** | Schreiboperation über TanStack Query | Im Kontext von TanStack Query, nicht allgemein |

---

## 4. Englische Begriffe ohne deutsche Entsprechung

Laut Kapitel 3 wurden folgende englische Begriffe bewusst übernommen,
da keine standardisierten deutschen Entsprechungen existieren:

| Begriff | Begründung |
|---|---|
| **Stack** | Kein deutsches Äquivalent im Kontext mobiler Navigation |
| **Screen** | Kein deutsches Äquivalent im Kontext mobiler Entwicklung |
| **Tab Navigation** | Kein deutsches Äquivalent |
| **Modal** | Kein deutsches Äquivalent |
| **Hook** / **Custom Hook** | Kein deutsches Äquivalent im React-Kontext |
| **Boilerplate** | Kein deutsches Äquivalent; bei Erstnennung erklären |
| **Caching** / **Cache** | Etablierter Fachbegriff ohne deutsche Entsprechung |
| **Framework** | Etablierter Fachbegriff; kein Anführungszeichen nötig |
| **State** / **Server-State** / **Client-State** | Im React-Kontext kein deutsches Äquivalent |

---

## 5. Abkürzungen

Alle Abkürzungen müssen bei Erstnennung ausgeschrieben werden.
In der Arbeit werden Abkürzungen über `\gls{}` eingebunden. Bei Eigennamen wie Gluestack-ui ignorieren

| Abkürzung | Ausgeschrieben | Erstnennung (Kapitel) |
|---|---|---|
| SUS | System Usability Scale | Kap. 6.1 |
| FA | Funktionale Anforderung | Kap. 2.2 |
| NFA | Nicht-funktionale Anforderung | Kap. 2.3 |
| API | Application Programming Interface | Kap. 3 oder 4 |
| REST | Representational State Transfer | Kap. 3.1.1 |
| HTTP | Hypertext Transfer Protocol | Kap. 3.1.1 |
| UI | User Interface | Kap. 3 oder 4 |
| ER | Entity-Relationship | Kap. 3.1.2 |
| ACID | Atomicity, Consistency, Isolation, Durability | Kap. 4.1 |
| JSI | JavaScript Interface | Kap. 4.2.1 |
| SDK | Software Development Kit | Kap. 4.3 |
| SWR | Stale-While-Revalidate | Kap. 4.4.2 |
| RTK | Redux Toolkit Query | Kap. 4.4.3 |
| GPS | Global Positioning System | Kap. 2 (Use Cases) |
| UML | Unified Modeling Language | Kap. 3 (Diagramme) |
| JWT | JSON Web Token | Kap. 5 (Implementierung) |

---

## 6. Verbotene Formulierungen

| Verboten | Richtig | Grund |
|---|---|---|
| Tierbesitzer | Tierhalter | Festgelegte Zielgruppenbezeichnung |
| Nutzer / Nutzer und Nutzerinnen | Nutzende | Geschlechtsneutrale Form |
| Teilnehmer | Teilnehmende | Geschlechtsneutrale Form |
| Ich habe / Wir haben | Es wurde / In dieser Arbeit wird | Keine Ich-Form |
| eigentlich, quasi, sozusagen | streichen oder präzise formulieren | Umgangssprache |
| wie allgemein bekannt | streichen | Unzulässige Allgemeinaussage |
| Die Anwendung – die … – wurde | Die Anwendung, die … wurde | Kein Gedankenstrich als Einschub |
| JWT-Token | JWT | „Token" ist bereits in JWT enthalten (Redundanz) |
| App (informell) | Anwendung | Im Fließtext bevorzugt; „App" nur in UI-Kontext |
| petappoint App | \textit{petappoint} | Kein nachgestelltes „App" |