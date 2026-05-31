# Chapter Guide: 03 – Konzeption

## Zweck dieser Datei

Diese Datei steuert, wie du bei Aufgaben zu Kapitel 3 vorgehst.
Lies sie vollständig bevor du schreibst, prüfst oder überarbeitest.

---

## Aufgaben die du in diesem Kapitel übernimmst

- Textentwürfe für einzelne Abschnitte auf Basis von Stichpunkten ausformulieren
- Bestehende Abschnitte auf Stil, Wissenschaftlichkeit und Konsistenz prüfen
- Stilmängel und Fehler korrigieren
- Überprüfe ob gewiße Aussagen ohne Quelle getroffen worden sind

Warte auf konkrete Aufgaben. Arbeite immer nur am angefragten Abschnitt.

---

## Struktur & Funktion der Abschnitte

Kapitel 3 umfasst S. 19–39 und bildet die DSR-Phase **Design** ab.
Es übersetzt die in Kap. 2 definierten Anforderungen in eine konkrete Systemkonzeption.

Stelle sicher, dass der folgende logische Fluss erhalten bleibt:

**Softwarearchitektur → Backend-Grundlage → Kritische Betrachtung → Komponentendiagramm → Navigationskonzept → Mockups → Aktivitätsdiagramm**

### Einleitungsabsatz
- Stelle sicher, dass der Bezug zu Kapitel 2 explizit hergestellt wird.
- Der Absatz soll alle Abschnitte des Kapitels kurz ankündigen.

### §3.1 Softwarearchitektur

#### §3.1.1 Architekturübersicht
- Stelle sicher, dass die drei Schichten (Präsentationsschicht, Anwendungsschicht, Datenschicht) klar definiert und voneinander abgegrenzt werden.
- Softwarearchitektur, Schichtenarchitektur, Client-Server-Prinzip und REST-API müssen beim ersten Auftreten definiert und mit `\cite{}` belegt werden.
- Prüfe die REST-Operationen: Im Text steht „POST, PUT, GET und DELETE (Erstellen, Bearbeiten, Bearbeiten, Löschen)" — „PUT" wird zweimal als „Bearbeiten" übersetzt. Korrigiere auf „POST, PUT, GET und DELETE (Erstellen, Aktualisieren, Abrufen, Löschen)" wenn du den Abschnitt überarbeitest.
- Stelle sicher, dass der Fokus auf die Präsentationsschicht klar begründet wird: Das Backend existiert bereits als Vorleistung.

#### §3.1.2 Bestehende Backend-Architektur als Grundlage
- Stelle sicher, dass das ER-Diagramm korrekt referenziert wird (`\ref{fig:erdiagramm}`).
- Prüfe auf Tippfehler Im Text steht zum Beispiel „ein Tier kann nicht ohne eine Person exitieren" → „existieren".
- Prüfe auf grammatikalische Inkonsistenz: „1 Tiertyp kann wiederum mehrere Rassen umfassen, aber mehrere 1 Rassen entstehen aus 1 Tiertyp" — der Satz ist unklar. Formuliere ihn auf Anfrage um.
- Beschreibe das ER-Diagramm sachlich und ohne Wertung.

#### §3.1.3 Kritische Betrachtung der Backend-Infrastruktur
- Stelle sicher, dass alle Kritikpunkte sachlich und ohne subjektive Wertung formuliert sind.
- Jeder Kritikpunkt muss klar benannt und begründet sein.
- Der abschließende Satz muss explizit festhalten, dass die Korrektur dieser Schwachstellen außerhalb des Umfangs dieser Arbeit liegt.
- Verwende keine Formulierungen wie „leider" oder „bedauerlicherweise".

### §3.2 Komponentendiagramm des Frontends
- Stelle sicher, dass die drei Schichten (Präsentationsschicht, Business-Schicht, Datenzugriffsschicht) konsistent mit §3.1.1 benannt werden.
- Der Begriff „Komponentendiagramm" muss beim ersten Auftreten definiert und mit `\cite{sparxsystems2026}` belegt werden.
- Stelle sicher, dass die Abbildungsreferenz (`\ref{fig:komponentendiagramm}`) korrekt gesetzt ist.
- Prüfe auf Tippfehler: Im Text steht „zeigen zeigen" (doppeltes Wort) in §3.4 — entferne die Dopplung wenn du den Abschnitt überarbeitest.

### §3.3 Navigationskonzeptdiagramme des Frontends
- Stelle sicher, dass die drei Navigationsbereiche (Auth Stack, Tab Navigation, Modal Stacks) klar unterschieden werden.
- Die Rollenabhängigkeit der Navigation (Tierhalter vs. Tierarztpraxis) muss explizit benannt werden.
- Stelle sicher, dass beide Abbildungsreferenzen korrekt gesetzt sind (`\ref{fig:nav-tierhalter}`, `\ref{fig:nav-tierarzt}`).
- Verwende „Nutzende" statt „Nutzer".

### §3.4 Mockups zur Darstellung des User Interface
- Stelle sicher, dass der einleitende Absatz Mockups als Konzept kurz definiert und mit `\cite{pohl2021}` und `\cite{galitz2002}` belegt.
- Prüfe auf Tippfehler: Im Einleitungsabsatz steht „zeigen  zeigen" (doppeltes Wort) → entferne die Dopplung.
- Prüfe auf fehlenden Leerzeichen: „\cite[S.~112]{pohl2021}für" → Leerzeichen vor „für" ergänzen.
- Die vier Unterabschnitte (Authentifizierung, Tab-Ansichten Tierhalter, Buchungsprozess, Tab-Ansichten Tierarztpraxis) müssen jeweils die zugehörige Abbildung referenzieren.
- Beschreibe die Mockups strukturell und sachlich — keine subjektiven Bewertungen wie „ansprechend" oder „übersichtlich".

### §3.5 Aktivitätsdiagramm der Terminbuchung
- Stelle sicher, dass beide Abbildungsreferenzen korrekt gesetzt sind (`\ref{fig:aktivitaet-buchung-1}`, `\ref{fig:aktivitaet-buchung-2}`).
- Der Ablauf muss vollständig und in der richtigen Reihenfolge beschrieben sein.
- Verwende „Nutzende" statt „Nutzer".

---

## Bekannte Probleme

### Problem 1 – Falsche REST-Operationsübersetzung (§3.1.1)
Im Text steht „POST, PUT, GET und DELETE (Erstellen, Bearbeiten, Bearbeiten, Löschen)" — PUT wird zweimal als „Bearbeiten" übersetzt.
→ Korrigiere auf: „POST, PUT, GET und DELETE (Erstellen, Aktualisieren, Abrufen, Löschen)"

### Problem 2 – Tippfehler „exitieren" (§3.1.2)
Im Text steht „ein Tier kann nicht ohne eine Person exitieren".
→ Korrigiere auf: „existieren"

### Problem 3 – Unklarer Satz Kardinalität (§3.1.2)
Im Text steht: „1 Tiertyp kann wiederum mehrere Rassen umfassen, aber mehrere 1 Rassen entstehen aus 1 Tiertyp".
→ Formuliere um auf Anfrage, z.B.: „Ein Tiertyp kann mehrere Rassen umfassen, wobei jede Rasse genau einem Tiertyp zugeordnet ist, was einer $1{:}n$-Beziehung zwischen \textit{animal\_types} und \textit{animal\_races} entspricht."

### Problem 4 – Doppeltes Wort „zeigen zeigen" (§3.4)
Im Einleitungsabsatz von §3.4 steht „zeigen  zeigen".
→ Entferne die Dopplung.

### Problem 5 – Fehlendes Leerzeichen (§3.4)
Im Text steht „\cite[S.~112]{pohl2021}für" ohne Leerzeichen.
→ Ergänze ein Leerzeichen: „\cite[S.~112]{pohl2021} für"

### Problem 6 – „Nutzer" statt „Nutzende" (§3.3, §3.5)
In den Navigations- und Aktivitätsdiagramm-Abschnitten wird mehrfach „Nutzer" verwendet.
→ Ersetze durch „Nutzende" überall im Kapitel.

---

## Begriffe & Quellen

### Einheitliche Begriffe in diesem Kapitel

| Falsch                          | Richtig                           |
|---------------------------------|-----------------------------------|
| Nutzer                          | `Nutzende`                        |
| nicht funktionale Anforderungen | `Nicht-funktionale Anforderungen` |
| Tierbesitzer                    | `Tierhalter`                      |
| cross-platform                  | `plattformübergreifend`           |

### Verwendete Quellen

Entnimm alle konkreten Inhalte immer aus dem aktuellen `.tex`-Text. Die Cite-Keys dienen zur Orientierung:

| Cite-Key                  | Inhalt                                              |
|---------------------------|-----------------------------------------------------|
| `\cite{richards2021}`     | Softwarearchitektur — keine einheitliche Definition |
| `\cite{gharbi2020}`       | Softwarearchitektur — inhaltliche Definition        |
| `\cite{tanenbaum2007}`    | Schichtenarchitektur, Client-Server, REST-API       |
| `\cite{watt2014}`         | ER-Diagramm — Definition und Grundkonzepte          |
| `\cite{sparxsystems2026}` | Komponentendiagramm — Definition                    |
| `\cite{sommerville2018}`  | Austauschbarkeit von Schichten                      |
| `\cite{pohl2021}`         | Mockups als visuelle Grundlage                      |
| `\cite{galitz2002}`       | UI-Elemente — Definition                            |
| `\cite{v0-vercel}`        | v0 von Vercel — KI-gestütztes Prototyping-Tool      |

---

## Grenzen dieses Kapitels

Füge folgende Inhalte **nicht** in Kapitel 3 ein — sie gehören in spätere Kapitel:

- Technologieentscheidungen (React Native, Expo, TanStack Query usw.) → Kap. 4
- Implementierungsdetails → Kap. 5
- Evaluationsergebnisse → Kap. 6
- Anforderungsdefinitionen (FA#, NFA#) → Kap. 2

Umfang: S. 19–39 (ca. 21 Seiten).

---

## DSR-Prüfung

Prüfe bei jeder Überarbeitung, ob folgende DSR-Kriterien erfüllt sind:

- Das Kapitel ist klar der DSR-Phase **Design** zuzuordnen: Die Anforderungen aus Kap. 2 werden in eine konkrete Systemkonzeption überführt.
- Die Architekturentscheidungen sind nachvollziehbar begründet — keine unbegründeten Designentscheidungen.
- Der Scope ist transparent: Der Fokus liegt auf der Präsentationsschicht, da das Backend als Vorleistung existiert.
- Die kritische Betrachtung des Backends (§3.1.3) zeigt, dass Limitationen offen kommuniziert werden — das stärkt die wissenschaftliche Glaubwürdigkeit.
- Mockups und Diagramme müssen als Designartefakte erkennbar sein, die direkt aus den Anforderungen abgeleitet wurden.