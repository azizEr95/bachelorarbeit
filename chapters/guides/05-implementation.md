# Chapter Guide: 05 – Implementierung

## Zweck dieser Datei

Diese Datei steuert, wie du bei Aufgaben zu Kapitel 5 vorgehst.
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

Kapitel 5 umfasst S. 49–60 und bildet die DSR-Phase **Build** ab.
Es dokumentiert die konkrete Umsetzung der Tierhalter-Rolle auf Basis der Konzeption (Kap. 3) und der Technologieauswahl (Kap. 4).

Stelle sicher, dass der folgende logische Fluss erhalten bleibt:

**Projektstruktur → Navigationsstruktur → Authentifizierung → API-Anbindung → Screens**

### Einleitungsabsatz
- Stelle sicher, dass der Bezug zu Kap. 4 explizit hergestellt wird.
- Der Scope muss klar benannt werden: Nur die Tierhalter-Rolle wurde implementiert.

### §5.1 Projektstruktur
- Stelle sicher, dass die Tabelle der Unterordner vollständig und konsistent mit dem tatsächlichen Projektaufbau ist.
- Prüfe, ob die Tabelle mit `\label{tab:src-structure}` korrekt referenziert wird, falls sie im Text erwähnt wird.
- Beschreibe die Struktur sachlich — keine Implementierungsdetails hier.

### §5.2 Navigationsstruktur mit Expo Router
- Stelle sicher, dass der Bezug zum Navigationskonzept aus Kap. 3 hergestellt wird.
- Jeder Unterabschnitt (Root Layout, Auth Stack, Tab Navigation, Modal Screens) muss das zugehörige Code-Listing referenzieren.
- Prüfe auf grammatikalischen Fehler: Im Text steht „Es stellt und initialisiert die globale Provider und Konfigurationen" — „stellt und initialisiert" ist redundant, außerdem muss „Provider" im Plural als „Provider" (nicht „den globalen Provider") formuliert werden. Korrigiere auf Anfrage.
- Verwende „Nutzende" statt „Nutzer".

### §5.3 Authentifizierung mit Expo Secure Store
- Stelle sicher, dass die vier Bereiche der Authentifizierung klar gegliedert sind: Tokenspeicherung, Zustandsverwaltung, API-Client, Sitzungsvalidierung.
- Prüfe auf grammatikalischen Fehler: Im Text steht „dass heißt ein ungültiges Token soll sofort zur Abmeldung führen" → „das heißt" (kein „dass").
- Prüfe auf stilistischen Fehler: Im Text steht „Token und Nutzerobjekt" mehrfach — „das Nutzerobjekt" ist korrekt, aber „Token und Nutzerobjekt" sollte konsistent als „das Token und das Nutzerobjekt" formuliert werden.
- Prüfe auf grammatikalischen Fehler: Im Text steht „wird \texttt{clearAuth()} automatisch aufgerufen. Der Token wird aus dem Store entfernt wird und leitet den Nutzer" — doppeltes „wird" und „Nutzer" statt „Nutzende". Korrigiere auf Anfrage.
- Code-Listings müssen sachlich im Fließtext eingeführt werden — erkläre was der Code tut, bevor das Listing erscheint.

### §5.4 API-Anbindung mit TanStack Query
- Stelle sicher, dass der Abschnitt „Query-Hooks" klar von §5.4.2 „Query-Key-Hierarchie" abgegrenzt ist — im Text fehlt der `\subsection`-Befehl für „Query-Hooks". Prüfe ob er vorhanden ist.
- Prüfe auf fehlenden Punkt: Im Text steht „für statische Referenzdaten, deren Inhalt sich zur Laufzeit nicht verändert wird \texttt{staleTime: Infinity} gesetzt" — nach „verändert" fehlt ein Komma oder Punkt. Korrigiere auf Anfrage.
- Stelle sicher, dass die Query-Key-Hierarchie vollständig erklärt wird — nicht nur aufgelistet.

### §5.5 Screens der Tierhalter-Rolle
- Stelle sicher, dass alle Anhang-Referenzen korrekt gesetzt sind (`\ref{fig:anhang_authentication}`, `\ref{fig:anhang_tab-light}`, `\ref{fig:anhang_tab-dark}`, `\ref{fig:anhang_booking-process}`).
- Prüfe auf stilistische Formulierung: Im Text steht „Diese klare Trennung trägt zur besseren Wartbarkeit der Codebasis bei" — „besser" ist eine wertende Formulierung. Formuliere auf Anfrage um zu: „Diese Trennung erhöht die Wartbarkeit der Codebasis."
- Stelle sicher, dass der Abschnitt zur Theme-Implementierung (§5.5.2) klar auf NFA#03 (Light/Dark Theme) aus Kap. 2 verweist.

---

## Bekannte Probleme

### Problem 1 – Grammatikfehler §5.2.1
Im Text steht „Es stellt und initialisiert die globale Provider und Konfigurationen bereit".
→ Korrigiere auf: „Es stellt globale Provider und Konfigurationen für alle untergeordneten Komponenten bereit."

### Problem 2 – „dass heißt" statt „das heißt" (§5.3.5)
Im Text steht „dass heißt ein ungültiges Token soll sofort zur Abmeldung führen".
→ Korrigiere auf: „das heißt, ein ungültiges Token führt sofort zur Abmeldung."

### Problem 3 – Doppeltes „wird" (§5.3.3)
Im Text steht „Der Token wird aus dem Store entfernt wird und leitet den Nutzer".
→ Korrigiere auf: „Das Token wird aus dem Store entfernt und die Anwendung leitet Nutzende beim nächsten Render automatisch zum Login-Screen weiter."

### Problem 4 – „Nutzer" statt „Nutzende" (§5.2, §5.3, §5.5)
An mehreren Stellen steht „Nutzer" oder „den Nutzer".
→ Ersetze durch „Nutzende" überall im Kapitel.

### Problem 5 – Fehlender Punkt/Komma (§5.4)
Im Text steht „für statische Referenzdaten, deren Inhalt sich zur Laufzeit nicht verändert wird \texttt{staleTime: Infinity} gesetzt" ohne Satzzeichen nach „verändert".
→ Ergänze ein Komma: „…nicht verändert, wird \texttt{staleTime: Infinity} gesetzt."

### Problem 6 – Wertende Formulierung (§5.5.1)
Im Text steht „Diese klare Trennung trägt zur besseren Wartbarkeit der Codebasis bei."
→ Korrigiere auf: „Diese Trennung erhöht die Wartbarkeit der Codebasis."

### Problem 7 – Fehlender `\subsection` für Query-Hooks (§5.4)
Im Fließtext wird ein Abschnitt zu Query-Hooks beschrieben, aber es fehlt möglicherweise der zugehörige `\subsection{Query-Hooks}`-Befehl.
→ Prüfe und ergänze auf Anfrage.

---

## Begriffe & Quellen

### Einheitliche Begriffe in diesem Kapitel

| Falsch | Richtig |
|---|---|
| Nutzer, den Nutzer | `Nutzende` |
| Tierbesitzer | `Tierhalter` |
| cross-platform | `plattformübergreifend` |

### Verwendete Quellen

Entnimm alle konkreten Inhalte immer aus dem aktuellen `.tex`-Text. Die Cite-Keys dienen zur Orientierung:

| Cite-Key | Inhalt |
|---|---|
| `\cite{expo-modals}` | Expo — Modal Screens |
| `\cite{expo-router}` | Expo Router |
| `\cite{expo-service}` | Expo Secure Store — iOS Keychain / Android Keystore |

---

## Grenzen dieses Kapitels

Füge folgende Inhalte **nicht** in Kapitel 5 ein — sie gehören in andere Kapitel:

- Technologiebegründungen → Kap. 4
- Architekturentscheidungen → Kap. 3
- Evaluationsergebnisse → Kap. 6
- Anforderungsdefinitionen (FA#, NFA#) → Kap. 2

Der Scope ist explizit auf die **Tierhalter-Rolle** beschränkt. FA#06 und FA#07 (Tierarztpraxis-Rolle) wurden nicht implementiert — erwähne das nicht erneut hier, da es bereits in Kap. 2 und Kap. 6 dokumentiert ist.

Umfang: S. 49–60 (ca. 12 Seiten).

---

## DSR-Prüfung

Prüfe bei jeder Überarbeitung, ob folgende DSR-Kriterien erfüllt sind:

- Das Kapitel ist klar der DSR-Phase **Build** zuzuordnen: Die Konzeption aus Kap. 3 wird konkret umgesetzt.
- Der Scope (nur Tierhalter-Rolle) ist transparent und wird im Einleitungsabsatz benannt.
- Code-Listings sind nicht selbsterklärend — jedes Listing muss im Fließtext eingeführt und erklärt werden.
- Implementierungsentscheidungen (z.B. `onSettled` statt `onSuccess` beim Logout) müssen kurz begründet werden — das stärkt die wissenschaftliche Nachvollziehbarkeit.
- Verweise auf Anhang-Abbildungen müssen korrekt gesetzt sein, da die Screenshots die einzige visuelle Dokumentation der implementierten Screens sind.