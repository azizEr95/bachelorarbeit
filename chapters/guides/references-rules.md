## Deine Rolle

Du unterstützt beim Schreiben der Bachelorarbeit. Konkrete Aufgaben:
- Bestehende Texte auf fehlende oder falsch gesetzte Referenzen prüfen
- Quellentyp anhand der Entscheidungsregeln in diesem Dokument bestimmen
- BibTeX-Einträge auf Vollständigkeit der Pflichtfelder prüfen
- Auf Einhaltung des 15%-Limits für @online-Quellen hinweisen

## Grundprinzipien

- Alles belegen, was nicht als allgemeines Informatik-Grundwissen gilt
- Fachbegriffe, Methoden und Konzepte bei Erstnennung mit Quelle einführen
- Bewertungen und Aussagen mit Wertungscharakter wissenschaftlich belegen
- Definitionen und Standards → möglichst Originalquelle
- Online-Quellen (@online) dürfen maximal 15% aller Quellen ausmachen
- Technische Dokumentation von Herstellern → immer @manual (gilt als Primärquelle)
- Wichtige Quellen mit vollständigen Angaben (DOI oder ISBN)

---

## Quellentypen & BibTeX-Format

### @book – Print-Quellen

Pflichtfelder: `author`, `title`, `year`, `publisher`, `address`, `isbn`

```bibtex
@book{pohl2021,
  author    = {Pohl, Klaus and Rupp, Chris},
  title     = {{Basiswissen Requirements Engineering}},
  year      = {2021},
  publisher = {dpunkt.verlag},
  address   = {Heidelberg},
  edition   = {5., überarbeitete und aktualisierte Auflage},
  isbn      = {978-3-86490-814-9},
  language  = {german},
}
```

### @online – Online-Quellen

Pflichtfelder: `author`, `title`, `year`, `url`, `urldate`, `organization`  
Achtung: max. 15% aller Quellen dürfen @online sein.

```bibtex
@online{doctolibreport,
  author       = {{Business Insider Group}},
  title        = {{So funktioniert das Millionen-Geschäftsmodell von Doctolib}},
  year         = {2024},
  url          = {https://www.businessinsider.de/...},
  urldate      = {2026-05-31},
  organization = {{Business Insider}},
  language     = {german}
}
```

### @manual – Technische Dokumentation

Gilt als Primärquelle. Verwenden für alle offiziellen Hersteller-Dokumentationen.  
Pflichtfelder: `author`, `title`, `year`, `url`, `urldate`, `organization`

```bibtex
@manual{nodejs-docs,
  author       = {{Node.js Development Group}},
  title        = {{Node.js Documentation}},
  year         = {2026},
  url          = {https://nodejs.org/en/about},
  urldate      = {2026-05-31},
  organization = {{Node.js}},
}
```

### Sonstige Typen

| Typ             | Wann verwenden             | Beispiel                            |
|-----------------|----------------------------|-------------------------------------|
| `@article`      | Artikel in Fachzeitschrift | Bangor et al. (2008), Hevner (2004) |
| `@incollection` | Beitrag in Sammelband      | Brooke (1996) – SUS                 |
| `@techreport`   | Institutionelle Berichte   | BTK Tierärztestatistik              |
| `@dataset`      | Datensätze, Umfragen       | Bitkom (2024)                       |

---

## Quellentyp-Entscheidung

### WANN WELCHER TYP

```
Ist es allgemeines Informatik-Grundwissen? (z.B. was eine Variable ist)
└── JA  → keine Quelle nötig
└── NEIN → weiter

Ist es eine offizielle Hersteller-Dokumentation?
└── JA  → @manual
└── NEIN → weiter

Ist es ein institutioneller Bericht oder Datensatz?
└── JA  → @techreport oder @dataset
└── NEIN → weiter

Ist es ein Artikel in einer Fachzeitschrift?
└── JA  → @article (mit DOI wenn vorhanden)
└── NEIN → weiter

Ist es ein Beitrag in einem Sammelband?
└── JA  → @incollection
└── NEIN → weiter

Gibt es ein wissenschaftliches Buch dazu?
└── JA  → @book (mit ISBN)
└── NEIN → weiter

Gibt es keine bessere Quelle?
└── JA  → @online (mit urldate) – aber 15%-Limit beachten!
```

### VERBOTEN

- `@online` verwenden, wenn ein Paper, Buch oder `@manual` existiert
- Webquellen ohne `urldate`
- Sekundärquellen zitieren, wenn die Originalquelle zugänglich ist
- Quellen ohne Autor pauschal mit dem Titel zitieren (Ausnahme: Institution als Autor)
- DOI weglassen, wenn vorhanden (@article, @incollection)
- ISBN weglassen bei @book

### GEFORDERT

- Fachbegriffe bei Erstnennung immer mit Quelle belegen (REST, SUS, ...)
- Originalquellen bevorzugen (z.B. Brooke 1996 für SUS, Fielding 2000 für REST)
- Normen und Standards direkt referenzieren (ISO 9241-11, RFC 7519)
- Bei Technologievergleichen: Entscheidungskriterien mit Quelle begründen
- @manual für jede verwendete Bibliothek/Framework anlegen
- Vollständige Angaben bei Hauptquellen: DOI bei Artikeln, ISBN bei Büchern
