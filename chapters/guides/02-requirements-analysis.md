# Chapter Guide: 02 – Anforderungsermittlung

## Zweck dieser Datei

Diese Datei steuert, wie du bei Aufgaben zu Kapitel 2 vorgehst.
Lies sie vollständig bevor du schreibst, prüfst oder überarbeitest.

---

## Aufgaben die du in diesem Kapitel übernimmst

- Textentwürfe für einzelne Abschnitte auf Basis von Stichpunkten ausformulieren
- Bestehende Abschnitte auf Stil, Wissenschaftlichkeit und Konsistenz prüfen
- Use-Case-Tabellen auf Vollständigkeit und Konsistenz prüfen
- Bekannte Stilmängel auf Anfrage korrigieren

Warte auf konkrete Aufgaben. Arbeite immer nur am angefragten Abschnitt.

---

## Struktur & Funktion der Abschnitte

Kapitel 2 umfasst S. 5–18 und bildet die DSR-Phase **Analyze** ab.
Es übersetzt das in Kap. 1 identifizierte Problem in konkrete, dokumentierte Anforderungen.

Stelle sicher, dass der folgende logische Fluss erhalten bleibt:

**Zielgruppenanalyse → Funktionale Anforderungen → Nicht-funktionale Anforderungen → Use Cases**

### Einleitungsabsatz
- Stelle sicher, dass der Bezug zu Kapitel 1 und zur Forschungsfrage hergestellt wird.
- Requirements Engineering muss als Disziplin kurz eingeführt und mit `\cite{pohl2021}` belegt werden.
- Die drei Begriffe „Stakeholder", „Anforderung" und „Requirements Engineering" müssen beim ersten Auftreten definiert werden.

### §2.1 Zielgruppe
- Stelle sicher, dass beide Zielgruppen klar unterschieden werden: **Tierhalter** und **Tierarztpraxen**.
- Prüfe, ob der Verweis auf Kapitel 1 korrekt ist. Im Text steht „in Kapitel 2 wurde deutlich" — das ist falsch, da die Marktanalyse in Kapitel 1 stattfindet. Korrigiere auf „in Kapitel 1" wenn du den Abschnitt überarbeitest.
- Verwende ausschließlich „Nutzende" statt „Nutzende" oder „Nutzer".
- Der zusammenfassende Absatz am Ende des Abschnitts soll beide Perspektiven explizit benennen.

### §2.2 Funktionale Anforderungen
- Stelle sicher, dass FA#01–FA#05 der Tierhalter-Rolle zugeordnet sind und FA#06–FA#07 der Tierarztpraxis-Rolle.
- Halte die Satzschablonen-Struktur einheitlich: „Die mobile Anwendung **muss** [Akteur] ermöglichen, [Funktion]."
- Weise darauf hin, dass FA#06 und FA#07 zwar definiert aber **nicht implementiert** wurden — das muss im Text erkennbar sein oder in einer Fußnote vermerkt werden.
- Verweise auf `\cite{pohl2021}` für die Definition von Satzschablonen und funktionalen Anforderungen.

### §2.3 Nicht-funktionale Anforderungen
- Stelle sicher, dass NFA#01–NFA#05 vollständig und korrekt nummeriert sind.
- Verweise auf `\cite{pohl2021}` für die Definition nicht-funktionaler Anforderungen.
- Schreibe „Nicht-funktionale Anforderungen" mit Bindestrich (nicht „Nicht funktionale").

### §2.4 Use Cases
- Stelle sicher, dass der einleitende Absatz Use Cases als Konzept kurz definiert und mit `\cite{cockburn2001}` belegt.
- Das Use-Case-Diagramm muss in §2.4.1 als erstes Element erscheinen.
- Halte die Tabellenstruktur aller Use Cases einheitlich: Name, Kurzbeschreibung, Akteure, Vorbedingungen, Auslösendes Ereignis, Hauptszenario, Alternativszenario, Nachbedingungen.
- Prüfe bei jeder Use-Case-Tabelle, ob Akteur, Vorbedingungen und Nachbedingungen vollständig und konsistent sind.
- UC-01 bis UC-06 betreffen die Tierhalter-Rolle, UC-07 bis UC-10 die Tierarztpraxis-Rolle — halte diese Zuordnung konsistent.

---

## Bekannte Probleme

### Problem 1 – Falscher Kapitelreferenz
Im Fließtext kommt die Formulierung „in Kapitel 2 wurde deutlich" vor, obwohl die Marktanalyse in Kapitel 1 stattfindet.
→ Ersetze durch „in Kapitel 1 wurde deutlich" wenn du den Abschnitt überarbeitest.

### Problem 2 – Fehlender Bindestrich
„Nicht funktionale Anforderungen" erscheint ohne Bindestrich.
→ Ersetze durch „Nicht-funktionale Anforderungen" überall im Kapitel.

### Problem 3 – Fehlende Kennzeichnung nicht implementierter FAs
FA#06 und FA#07 wurden definiert und konzipiert, aber nicht implementiert und evaluiert.
→ Stelle sicher, dass dieser Scope-Hinweis im Text oder als Fußnote erkennbar ist, z.B.:
„Die Anforderungen FA\#06 und FA\#07 wurden im Rahmen dieser Arbeit konzipiert, jedoch nicht implementiert."

### Problem 4 – „Sie" statt „sie" (Großschreibung)
Im Use-Cases-Einleitungsabsatz steht „werden Sie im Folgenden durch ein Use-Case-Diagramm ergänzt" — das „Sie" ist fälschlicherweise großgeschrieben.
→ Ersetze durch „sie".

---

## Begriffe & Quellen

### Einheitliche Begriffe in diesem Kapitel

| Falsch | Richtig |
|---|---|
| Nutzer, Nutzerinnen und Nutzer | `Nutzende` |
| Nicht funktionale Anforderungen | `Nicht-funktionale Anforderungen` |
| Tierbesitzer | `Tierhalter` |
| Praxis (ohne Kontext) | `Tierarztpraxis` |

### Verwendete Quellen

Entnimm alle konkreten Inhalte immer aus dem aktuellen `.tex`-Text. Die Cite-Keys dienen zur Orientierung:

| Cite-Key | Inhalt |
|---|---|
| `\cite{pohl2021}` | Requirements Engineering — Pohl; Definition von Stakeholder, Anforderung, Satzschablone |
| `\cite{cockburn2001}` | Use Cases — Cockburn; Definition und Struktur |

---

## Grenzen dieses Kapitels

Füge folgende Inhalte **nicht** in Kapitel 2 ein — sie gehören in spätere Kapitel:

- Technologieentscheidungen → Kap. 4
- Implementierungsdetails → Kap. 5
- Evaluationsergebnisse → Kap. 6
- Architekturentscheidungen → Kap. 3

Umfang: S. 5–18 (ca. 14 Seiten).

---

## DSR-Prüfung

Prüfe bei jeder Überarbeitung, ob folgende DSR-Kriterien erfüllt sind:

- Das Kapitel ist klar der DSR-Phase **Analyze** zuzuordnen: Anforderungen werden aus dem identifizierten Problem abgeleitet, nicht erfunden.
- Alle Anforderungen sind nachvollziehbar aus der Zielgruppenanalyse und der Problemstellung (Kap. 1) hergeleitet.
- Der Scope ist transparent: FA#06 und FA#07 sind definiert aber nicht implementiert — das muss erkennbar sein.
- Use Cases konkretisieren die funktionalen Anforderungen — jede FA sollte in mindestens einem Use Case abgebildet sein.