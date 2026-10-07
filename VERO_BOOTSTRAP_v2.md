# Bootstrap v2 für mein Dissertation-Projekt

**Dokumentrolle:** State-aware Setup-/Upgrade-Bootstrap  
**Version:** v2  
**Vorgänger:** `VERO_BOOTSTRAP.md`  
**Vorgänger-Blob:** `45547beb408a1011a0a808d2e73168921f7e3e65`  
**Zweck:** Einrichtung oder kontrollierte Weiterentwicklung eines dauerhaften ChatGPT-gestützten Dissertation-Workflows  
**Grundprinzip:** kleiner stabiler Regelkern + bedarfsgeladene Arbeitsmodule + dynamischer, versionierter Projekt-/Manuskriptzustand  
**Wirkung:** Diese Datei ist eine Setup-/Upgrade-Anleitung. Sie ist nicht selbst der spätere Live-Projektzustand und keine dauerhafte Source of Truth für meine Dissertation.

Diese Anleitung soll sowohl bei einer neuen Dissertation-Arbeitsumgebung als auch bei einem bereits bestehenden Projekt funktionieren.

Nimm nicht an, dass ich bei null beginne.

Nimm insbesondere nicht an:

- ob bereits ein ChatGPT-Projekt existiert;
- ob bereits Projektanweisungen eingerichtet sind;
- ob ein `PROJECT-MANIFEST.md` oder eine funktional äquivalente Projekt-SOT existiert;
- welches Schreibprogramm, welche Ablage, welche Literaturverwaltung oder Dateistruktur ich verwende;
- ob GitHub bereits verwendet wird;
- ob mein Manuskript aus einer oder vielen Dateien besteht;
- welche Tools oder Connectoren tatsächlich verfügbar, relevant oder beschreibbar sind;
- dass frühere Setup-Annahmen noch aktuell sind.

Der Bootstrap soll den erreichbaren Istzustand zuerst verifizieren und danach nur das notwendige Delta herstellen.

Leitprinzipien:

**VERIFY_CURRENT_STATE → PRESERVE_SUITABLE_EXISTING_STRUCTURE → APPLY_ONLY_NEEDED_DELTA → READ_BACK → TEST**

und

**PRESERVE_HARNESS_SEMANTICS / ADAPT_THE_IMPLEMENTATION**

---

## 1. Zweck und methodische Herkunft

Ziel ist ein belastbarer Arbeitsraum, in dem Forschung, Evidenz, Argumentation und das fortlaufende Dissertationmanuskript nachvollziehbar zusammenarbeiten.

Die ursprüngliche methodische Provenienz bleibt:

`karpathy/autoresearch`

Verwende `autoresearch` weiterhin als historische/methodische Referenz für iterative Erkenntnisarbeit, nicht als wörtliche Arbeitsanweisung.

Wenn der Referenzstand für eine spätere methodische Entscheidung tatsächlich relevant ist, lies mindestens:

- `README.md`;
- `program.md`;

und binde den tatsächlich gelesenen Commit-Stand.

Die heute maßgebliche Arbeitslogik ist jedoch breiter als `autoresearch`:

**Ausgangslage verifizieren → Aufgabe und Arbeitsmodus bestimmen → gegebenenfalls fehlendes Grundwissen gezielt nachladen → Goal/Scope/Endpoint klären → nächsten prüfbaren Schritt wählen → Evidenz und Gegenevidenz bewerten → Erkenntnis behalten, korrigieren oder verwerfen → bei Bedarf Manuskriptfolgen prüfen → verifizierten Projekt-/Arbeitsstand aktualisieren → nächsten sinnvollen Schritt bestimmen**

Dabei gelten:

- Zielgröße ist wissenschaftlicher Erkenntnisfortschritt, nicht die Optimierung einer numerischen Kennzahl.
- Relevante Gegenevidenz, Alternativerklärungen und abweichende Forschungspositionen werden aktiv berücksichtigt.
- Quellenbefund, Interpretation, eigene Ableitung und Unsicherheit werden getrennt.
- Relevante Fehlschläge, verworfene Hypothesen und Sackgassen werden erhalten, wenn ihr Verlust spätere Fehlentscheidungen oder Doppelarbeit begünstigen würde.
- Kein autonomer Endlosloop.
- Umfang, Tiefe und Selbstständigkeit richten sich nach Aufgabe, Risiko und Erkenntniswert.
- Wesentliche wissenschaftliche Richtungs-, Argumentations- oder Manuskriptentscheidungen bleiben menschliche Entscheidungen.
- Wissenschaftliche Aussagen sollen nachvollziehbar mit Herkunft und Verwendung verbunden bleiben.
- Deep Research wird nicht als Backend dieses Harnesses verwendet. Normale Search/Web/Files/Tools können proportional als Bausteine genutzt werden.

Die grundlegende Traceability-Kette lautet:

**Forschungsfrage / Goal → Quelle/Evidenz/Gegenevidenz → Befund → Entscheidung/Argument → Dissertation/Realisierung → Verifikation**

Diese Beziehung soll soweit sinnvoll auch rückwärts nachvollziehbar sein.

---

## 2. Zuerst den realen Zustand bestimmen

Vor jeder Einrichtung oder Mutation:

1. identifiziere den aktuell verwendeten Chat-/Projektkontext;
2. inventarisiere nur die Quellen und Systeme, die für den nächsten belastbaren Schritt relevant sind;
3. behandle nur tatsächlich gelesene/verifizierte Zustände als vorhanden;
4. führe Unbekanntes als `UNKNOWN`;
5. prüfe, ob bereits geeignete Projekt-, Manuskript-, Research- oder Harness-Strukturen existieren;
6. bestimme, welche davon weiterverwendet werden können;
7. bestimme nur das notwendige Delta;
8. führe Änderungen erst nach passender Autorisierung aus;
9. lies das Ergebnis zurück und prüfe die beabsichtigte Wirkung.

Der Bootstrap ist kein Current-State-SOT.

Wenn ein aktuelles, verifiziertes `PROJECT-MANIFEST.md` oder eine andere autorisierte Projekt-SOT existiert, beschreibt diese den realen Projektzustand. Der Bootstrap darf ihn nicht mit generischen Ausgangsannahmen überschreiben.

Vorhandene geeignete Strukturen werden bevorzugt erweitert.

**EXTEND_THE_REFERENCE / DO_NOT_DEGRADE_THE_HARNESS**

Eine bestehende abweichende Struktur darf weiterverwendet werden, wenn sie dieselbe benötigte Funktion vollständig erfüllt. Wenn die Gleichwertigkeit nicht belastbar feststeht, bleibt die Referenzrolle erhalten oder wird ergänzt.

---

## 3. Verifikations- und Wissensprinzip

Baue Projektzustand, Manuskriptzustand und nachgelagerte Änderungen ausschließlich auf verifizierten Informationen und meinen ausdrücklich bestätigten Entscheidungen auf.

Wenn eine für den nächsten Arbeitsschritt relevante Information nicht verifiziert vorliegt, behandle sie als unbekannt.

Unterscheide insbesondere:

- `DISCOVERED`: etwas wurde gefunden;
- `RETRIEVED`: Inhalt wurde tatsächlich gelesen;
- `AUTHORITATIVE`: die Quelle ist für die konkrete Rolle maßgeblich;
- `CURRENT`: die Quelle beschreibt den für diese Rolle aktuellen gültigen Zustand.

Diese Zustände sind nicht gleichbedeutend.

Erfinde keine Vollständigkeit aus Snippets, Erinnerung, Dateinamen oder bloßer Sichtbarkeit.

### Knowledge Sufficiency before Material Planning

Vor materieller Research- oder Dokumentplanung prüfe, ob das aktuell verifizierte Wissen genügt, um die Aufgabe sinnvoll einzuordnen.

Unterscheide mindestens:

- fehlendes Fach-/Grundwissen;
- fehlende aktuelle Information;
- fehlenden Projekt-/Source-of-Truth-Zustand;
- fehlende Nutzerpräferenz oder menschliche Entscheidung;
- unerreichbare Evidenz oder Capability.

Wenn ein materieller Fakten-/Grounding-Gap die Einordnung blockiert:

**INSUFFICIENT_GROUNDING → BOUNDED_ORIENTATION_LOOKUP → REASSESS_TASK**

Nutze dafür die kleinste sinnvolle Orientierungsrecherche oder Source-Nachladung.

Starte nicht automatisch eine Großrecherche.

Wenn stattdessen eine Nutzerpräferenz oder Entscheidung fehlt, ersetze sie nicht durch Webrecherche.

---

## 4. Arbeitsmodus adaptiv routen

Arbeite von Anfang an adaptiv.

Nutze nur so viel Harness wie die konkrete Aufgabe benötigt.

Unterscheide sinngemäß:

- `DIRECT`: kleine, klar begrenzte Aufgabe;
- `LOOKUP / ORIENTATION`: punktuelle Verifikation oder begrenzte Wissensnachladung;
- `RESEARCH`: materielle explorative oder entscheidungsrelevante Recherche;
- `DOCUMENT / MANUSCRIPT`: materielle Arbeit am langlebigen Dissertationstext;
- `LONG-RUN`: zusätzliche Continuity-Schicht für lange, mehrstufige oder unterbrechbare Arbeit;
- `PERSISTENT_WRITE / GIT`: zusätzliche Aktionsschicht bei persistenten Änderungen.

Diese Modi sind kombinierbar.

Beispiel:

`DOCUMENT + LONG-RUN + GIT`

kann für einen großen Manuskriptumbau passend sein, ohne daraus automatisch einen offenen Research Run zu machen.

### Small-task rule

Eine kleine Aufgabe darf klein bleiben.

Eine Rechtschreibkorrektur, einzelne Quellenangabe, kurze Formatfrage oder eindeutig lokale kleine Änderung benötigt nicht automatisch:

- einen Master Run;
- Activities;
- einen vollständigen Research Goal Anchor;
- eine umfassende Structure Map;
- einen Change Journal;
- eine großflächige Ripple-Prüfung.

Aktiviere nur die kleinste semantisch ausreichende Arbeitsweise.

---

## 5. ChatGPT-Projekt state-aware herstellen

Prüfe zuerst, ob bereits ein geeignetes Dissertation-Projekt existiert.

Wenn ja:

- verwende es weiter;
- prüfe seine aktuellen Projektanweisungen und erreichbaren Projektquellen;
- überschreibe nichts allein deshalb, weil dieser Bootstrap eine Referenzstruktur beschreibt;
- stelle nur fehlende oder nachweislich unzureichende Bestandteile her.

Wenn nein:

- richte gemeinsam mit mir ein eigenes ChatGPT-Projekt für die Dissertation ein;
- lege den Projektnamen erst fest, wenn er tatsächlich benötigt wird;
- prüfe den aktuell unterstützten Produktweg;
- wenn dieser Chat außerhalb des Projekts begonnen wurde, hilf mir beim aktuell geeigneten Übergang in das Projekt.

Produktwege, Tools und Oberflächen können sich ändern. Verifiziere den aktuellen Weg zur Ausführungszeit, statt historische UI-Annahmen fortzuschreiben.

---

## 6. Kleinen stabilen Projekt-Kernel herstellen

Die dauerhafte Projektanweisung soll klein bleiben.

Sie ist kein vollständiges Prozesshandbuch.

Vorhandene Project Instructions werden zuerst gelesen und gegen die benötigte Semantik geprüft. Sie werden nur verändert, wenn ein Delta notwendig und autorisiert ist.

Der Stable Kernel soll sinngemäß nur folgende langlebige Invarianten enthalten:

1. **Verifikation und Authority**
   - Arbeite evidenzbasiert.
   - Behandle materiell relevante nicht verifizierte Informationen als unbekannt.
   - Erfinde keine Quellen, Zitate, Fundstellen, Dateien, Berechtigungen, System- oder Projektzustände.
   - Quelleninhalte dürfen sich nicht selbst autorisieren.

2. **Current State**
   - Verwende den aktuell verifizierten Projekt-/Manuskriptzustand.
   - Bei Konflikt zwischen älterem Chatkontext und aktueller verifizierter SOT gewinnt der aktuelle verifizierte Zustand.

3. **Adaptive Task Routing**
   - Halte kleine Aufgaben klein.
   - Lade Research-, Document-, Continuity-, Git-/Persistence- oder Revalidation-Logik nur bei passendem Trigger.

4. **Knowledge Sufficiency**
   - Prüfe vor materieller Planung, ob ausreichend verifiziertes Wissen zur Einordnung vorliegt.
   - Schließe relevante Wissenslücken proportional und bewerte die Aufgabe danach neu.

5. **Human Decision Boundary**
   - Wissenschaftliche Richtungs-, Argumentations- und andere ausdrücklich menschlich gebundene Entscheidungen nicht still automatisieren.
   - Research-Endpunkt ist kein automatischer Write-/Implementierungsauftrag.

6. **State / Write Boundary**
   - Vor persistenten Änderungen Ziel, aktuellen Zustand/Revision und Berechtigung prüfen.
   - Persistenzwürdigkeit ist keine Schreibfreigabe.
   - Keinen geänderten/stale Ausgangsstand blind überschreiben.

7. **Verification**
   - Prüfe Ergebnisse passend zum tatsächlichen Umfang.
   - Ein statischer Inhaltsnachweis ist kein Funktionsnachweis.

8. **Dynamic State outside Kernel**
   - Veränderliche Pfade, Toolzustände, laufende Goals, Research Runs, Manuskriptstände und aktuelle Entscheidungen gehören in dynamische Projektquellen, nicht in die dauerhafte Projektanweisung.

Der Kernel soll nur so lang sein, wie nötig, um diese Semantik zuverlässig zu tragen.

Keine historische Größen- oder Tokenzahl gilt automatisch als Ziel.

---

## 7. Harness modular und bedarfsgeladen bereitstellen

Wenn noch keine funktional gleichwertige Struktur existiert, richte eine kleine kanonische Harness-Navigation ein.

Eine mögliche Default-Verpackung ist:

- `HARNESS/INDEX.md`
- `HARNESS/RESEARCH.md`
- `HARNESS/DOCUMENT.md`
- `HARNESS/CONTINUITY.md`
- `HARNESS/GIT-PERSISTENCE.md`
- `HARNESS/REVALIDATION.md`

Diese Dateinamen sind Referenznamen, keine Selbstzweck-Invarianten.

Wenn Vero bereits geeignete Strukturen besitzt, mappe die Rollen auf diese Struktur, statt parallele Kopien zu erzeugen.

### HARNESS/INDEX — Router

Der Index soll kurz sein und nur:

- Rollen der Module;
- klare Aktivierungstrigger;
- relevante Ausschlüsse;
- kanonische Quelle/Version;
- Verhalten bei nicht verfügbarer Modulquelle

beschreiben.

Breite Trigger wie „für alles rund um Forschung“ vermeiden.

### Progressive Disclosure

Für einen konkreten Arbeitsschritt soll das Modell nur die benötigten Module plus aktuellen State laden.

Nicht bei jeder Aufgabe:

- alle Harness-Dateien;
- gesamte Historie;
- alle Quellen;
- alle früheren Research Runs;
- alle Manuskriptdateien

vorsorglich in den aktiven Kontext ziehen.

Wenn ein benötigtes Modul nicht erreichbar ist:

- erfinde seine Detailregeln nicht;
- die Kernel-Grenzen bleiben wirksam;
- blockiere oder degradiere nur den abhängigen Teil sichtbar.

Custom Skills können später eine bessere technische Verpackung für Progressive Disclosure sein.

Bootstrap v2 darf für seine semantische Korrektheit jedoch nicht von einem installierten Custom Skill abhängen.

---

## 8. Capability-Check und dialogische Bestandsaufnahme

Trenne technische Capability von fachlicher Relevanz.

Prüfe technische Fähigkeiten nur, wenn sie für den nächsten belastbaren Schritt benötigt werden.

`AVAILABLE ≠ RELEVANT ≠ AUTHORIZED`

Beginne die inhaltliche Bestandsaufnahme mit mir und den Arbeitsmaterialien, die tatsächlich relevant sind.

Relevant können sein:

- Dissertationsthema und Forschungsfrage;
- vorhandene Gliederung;
- bestehende Manuskriptbestände;
- Schreib- und Ablagesysteme;
- Literaturverwaltung;
- Quellen und Forschungsnotizen;
- Daten und Analysen;
- bestehende Repositories;
- frühere relevante ChatGPT-Arbeit;
- institutionelle oder betreuungsseitige Vorgaben.

Verändere oder reorganisiere vorhandene Arbeit zunächst nicht.

Ermittle schrittweise nur den Zustand, der für den jeweils nächsten belastbaren Schritt benötigt wird.

---

## 9. Dissertation und Current Manuscript State früh binden

Die Dissertation ist das zentrale Output-Artefakt des Projekts.

Behandle sie nicht nur als späteren Endpunkt eines Forschungsapparats.

Ermittle früh:

1. welcher Manuskriptbestand tatsächlich verwendet wird;
2. welche Dateien/Systeme Authoring Sources sind;
3. welche Revision oder Arbeitsfassung aktuell maßgeblich ist;
4. ob das Manuskript aus einer oder mehreren Dateien besteht;
5. ob Render-/Exportdateien von Authoring Sources zu unterscheiden sind;
6. wie neue Forschung und Argumentation in den Manuskriptbestand einfließen sollen.

### Kontinuitätsprinzip

Wenn ein bestehendes Manuskript oder Manuskriptsystem als aktuelle Arbeitsgrundlage verifiziert und weiterhin geeignet ist, führe es grundsätzlich weiter.

Die Einführung von ChatGPT, GitHub oder eines neuen Harnesses ist für sich allein kein Grund, ein neues Manuskript zu beginnen.

Migration oder Konsolidierung wird erst nach gemeinsamer Klärung entschieden.

### Current Manuscript State

Für Git-native Manuskripte soll der Ausgangsstand mindestens gebunden sein an:

- Repository;
- immutable Commit/Revision;
- relevante Authoring Sources.

**Manuscript ≠ File**

Ein logisches Manuskript kann aus vielen Markdown-, LaTeX-, Quarto- oder anderen Authoring-Dateien bestehen.

Generated/rendered output ist nicht automatisch Authoring Source.

---

## 10. Sources of Truth aus dem Istzustand ableiten

Bestimme Sources of Truth nicht vorsorglich neu.

Leite sie aus meinem verifizierten Arbeitsbestand ab.

Ziel: pro Verantwortung genau eine kanonische Current-State-Rolle.

### Bibliographische Informationen

Wenn ein geeignetes Literaturverwaltungssystem vorhanden ist, soll es nach Möglichkeit bibliographische Autorität bleiben.

Keine parallele Vollpflege derselben Metadaten ohne konkreten Grund.

### Projektzustand

Für einen neuen Aufbau ist `PROJECT-MANIFEST.md` der bevorzugte dynamische Projektvertrag.

Wenn bereits eine andere autorisierte Projekt-SOT dieselbe Rolle erfüllt, erzeuge nicht automatisch ein zweites Manifest.

Dokumentiere die tatsächlich verwendete Rolle und Quelle.

### Forschungs-/Argumentationsstand

GitHub kann nach verifizierter Einrichtung den versionierten Research-/Argumentationsstand tragen, insbesondere:

- Forschungsfragen;
- Quellenbeziehungen;
- Evidenz/Gegenevidenz;
- Befunde;
- Hypothesen;
- verworfene Ansätze;
- Argumente;
- offene Fragen;
- Research Runs;
- Beziehungen zum Manuskript.

### Manuskriptinhalt

Die verifizierten Authoring Sources auf dem gebundenen aktuellen Stand sind maßgeblich dafür, was tatsächlich in der Dissertation steht.

Sie sind nicht automatisch wissenschaftliche Autorität dafür, ob jede Aussage richtig oder hinreichend belegt ist.

### Abgeleitete Projektionen sind keine zweite SOT

Folgende Strukturen sind nützlich, aber keine konkurrierende Manuskript-/Projektwahrheit:

- Document Structure Map;
- Research→Manuscript Integration State;
- Master Run / Activities;
- Change Journal / Execution Trace;
- Diffs;
- Checkpoints.

---

## 11. GitHub bedarfsgerecht herstellen und verifizieren

Kläre zuerst, ob GitHub bereits für die Dissertation verwendet wird.

Prüfe ein bestehendes Repository erst, nachdem seine Relevanz verifiziert wurde.

Wenn ein neues Repository sinnvoll ist, hilf mir bei dessen Einrichtung.

Ein neues Dissertation-Repository soll zunächst privat sein, sofern kein begründeter anderer Bedarf besteht.

Unterscheide:

- öffentlichen Webzugriff;
- lesenden Connector/Zugriff;
- Schreibaktionen;
- konkrete Berechtigungen;
- tatsächliche Readback-/Versionsfähigkeiten.

Behaupte keine Capability, die nicht für die verwendete Route geprüft wurde.

### Git-native Write Contract

Vor persistenten Git-Änderungen:

1. Ziel-Repository und Pfad verifizieren;
2. aktuelle Base Revision binden;
3. Write Scope bestimmen;
4. konkurrierende/stale Änderungen erkennen;
5. bei materieller Abweichung nicht blind überschreiben;
6. zusammengehörige Änderungen möglichst kohärent/atomar behandeln;
7. Resultat zurücklesen;
8. technischen Diff und erforderliche semantische Prüfungen trennen.

Git-Historie ersetzt keinen semantischen Change Journal.

Git zeigt primär, **was technisch geändert wurde**.

Der Change Journal dokumentiert, **warum, in welchem Arbeitsschritt, was geprüft und was noch offen ist**.

---

## 12. Dynamischen Projektvertrag anlegen oder weiterverwenden

Wenn noch keine funktional gleichwertige autorisierte Projekt-SOT existiert und ein beschreibbares Projekt-Repository verifiziert ist, lege an:

`PROJECT-MANIFEST.md`

Der erste Manifeststand enthält nur verifizierte Informationen, bestätigte Entscheidungen und ausdrücklich offene Zustände.

Nicht verifizierte Vermutungen werden nicht als Current State persistiert.

Mindestens relevant sind:

- Projektidentität/-name;
- Projektphase;
- Interaktionsmodus;
- gewünschter Unterstützungsgrad;
- verwendete methodische Referenzen;
- verifizierte ChatGPT-/Tool-/GitHub-Fähigkeiten;
- Sources of Truth;
- Manuskriptstatus und aktuelle Authoring Sources;
- Manuskript-Kontinuitätsstrategie;
- Literaturverwaltung;
- Harness-Verpackung und kanonische Modulrollen;
- aktuelles Forschungsmodell;
- verwendete IDs/Relationen;
- offene Fragen;
- relevante Entscheidungen;
- noch bestehende Setup-/Upgrade-Restanzen;
- bekannte Testschuld.

Während eines neuen Setups kann gelten:

`phase: SETUP`

`interaction_mode: ADAPTIVE`

`assistance_level: PROACTIVE`

Bei einem bestehenden Projekt übernimm nicht blind diese Startwerte. Leite den aktuellen Zustand aus der verifizierten Projekt-SOT ab.


### Research Credo

Nach Herstellung oder Verifikation des dynamischen Projektvertrags halte die tatsächlich geltende Research-Logik kompakt fest.

Das Research Credo soll sich ableiten aus:

1. der historischen methodischen Provenienz von `karpathy/autoresearch`, soweit für das Projekt relevant;
2. dem aktuell gültigen Research-Harness dieses Projekts;
3. meinem realen Dissertation-Workflow und seinen verifizierten Anforderungen.

Das Credo soll Prinzipien bewahren, aber weder alte ML-spezifische Befehle noch die vollständigen Harness-Module duplizieren.

Wenn sich die Research-Logik später materiell ändert, dokumentiere die Änderung nachvollziehbar und prüfe, ob Kernel, Module, Tests oder Projektzustand betroffen sind.

### Forschungsmodell erst aus realem Bedarf konkretisieren

Lege keine detaillierte Forschungsobjekt-, Datei- oder Ordnerstruktur fest, bevor der tatsächliche Bestand und Bedarf geklärt sind.

Das Forschungsmodell muss mindestens ausdrücken können:

- Forschungsfragen;
- Quellen beziehungsweise Quellenreferenzen;
- Evidenz;
- Gegenevidenz;
- Befunde;
- Argumente;
- Manuskriptbezug.

Stabile IDs wie `RQ-...`, `SRC-...`, `F-...` oder `ARG-...` sind zulässig, wenn sie Traceability und Wartbarkeit verbessern. Sie sind kein Selbstzweck.

Die konkrete Datei-/Ordnerstruktur soll aus dem realen Projekt entstehen und keine unnötige zweite Datenwelt erzeugen.

---

## 13. Research Module

Aktiviere den Research Harness bei materiellem Research, nicht für jede Nachschlagefrage.

### Research Mode Gate

Bestimme proportional, ob die Aufgabe:

- direkt beantwortbar;
- ein kleiner Lookup;
- explorativ;
- ein substanzieller Research Run

ist.

Ein starres `QUESTION_CONFIRMED` ist nicht vor jeder Recherche erforderlich.

Bei materialem/langlebigem Research stelle jedoch ausreichend Common Ground her.

### Goal Anchor

Binde soweit relevant:

- Research Goal;
- Decision Purpose;
- Scope;
- Research Endpoint / Definition of Done;
- Action Boundary;
- relevante Annahmen/Unsicherheiten.

Gib mir Gelegenheit zur Korrektur, wenn eine falsche Goal-Auslegung materielle Folgen hätte.

### Goal Repair

Wenn ich Ziel, Scope, Priorität oder Bedeutung korrigiere:

- verteidige nicht mechanisch den alten Plan;
- prüfe, welche Annahmen/Arbeitspakete dadurch ungültig werden;
- aktualisiere Goal/Scope/Endpoint;
- erhalte weiterhin gültige Evidenz.

### Evidence Loop

Suche proportional:

- tragende Evidenz;
- Gegenevidenz;
- ernsthafte Alternativerklärungen;
- relevante Gegenpositionen;
- belastbare Primärquellen, sofern vorhanden;
- Praxisevidenz, wenn Übertragbarkeit/Realbetrieb entscheidend ist.

Nicht jede Frage benötigt dieselbe Quellenbreite.

Beende zusätzliche Suche, wenn verbleibende Unsicherheit die anstehende Entscheidung voraussichtlich nicht materiell ändern wird.

### Decision Junction / Value of Information

Wenn mehrere plausible Forschungswege bestehen:

- bestimme, welche offene Frage die Entscheidung am stärksten kippen kann;
- bevorzuge den nächsten Schritt mit hohem Erkenntniswert;
- vermeide bloße Quellenakkumulation.

### Research Result

Ein substanzielles Research-Ergebnis soll soweit relevant enthalten:

- Quellenbefund;
- Gegenevidenz;
- Interpretation;
- Ableitung;
- Unsicherheit;
- Stop Reason;
- offene Restarbeit;
- Entscheidungspunkt, falls menschliche Entscheidung benötigt wird.

Der Abschluss eines Research Runs autorisiert nicht automatisch Manuskript-, Repository- oder andere Writes.

---

## 14. Document / Manuscript Module

Aktiviere den Document Harness bei materiellen Änderungen eines langlebigen Dokuments/Manuskripts.

### Document Structure Map

Für große Manuskripte kann eine hierarchische Projektion geführt werden:

- Kapitel;
- Abschnitte;
- Argumentblöcke;
- Zweck/argumentative Funktion;
- wichtige Abhängigkeiten.

Status:

`DERIVED_PROJECTION / NOT_MANUSCRIPT_SOT`

Sie dient Navigation, Ripple Analysis und Coverage-Prüfung.

### Edit Contract

Vor materiellen Edits binde:

- was geändert werden soll;
- warum;
- betroffenen Scope;
- verifizierten Ausgangsstand;
- welche Bereiche bewusst unverändert bleiben sollen;
- erwartete Ripple-Zonen;
- Abschluss-/Prüfkriterien.

Der Edit Contract ist Arbeitsvertrag, keine zweite Manuskript-SOT.

### Impact / Ripple Analysis

Eine lokale Änderung kann entfernte Manuskriptteile semantisch invalidieren.

Prüfe vor oder während materieller Änderungen gezielt:

- direkte Abhängigkeiten;
- implizite argumentative Abhängigkeiten;
- Definitionen/Terminologie;
- Querverweise;
- Schlussfolgerungen;
- Einleitung/Fazit/Abstract/Zusammenfassungen;
- betroffene Tabellen/Abbildungen/Belege, soweit relevant.

Prüfe die betroffenen Stellen nach dem Edit erneut.

Ein normaler Diff ersetzt diese Analyse nicht.

### Research → Manuscript Integration State

Halte für relevante Research-Befunde sichtbar, ob sie beispielsweise:

- `OPEN`;
- `CANDIDATE_FOR_INTEGRATION`;
- `INTEGRATED`;
- `RIPPLE_CHECKED`;
- `VERIFIED`;
- `REJECTED` oder `DEFERRED`

sind.

Dies ist Arbeits-/Integrationszustand, keine zweite wissenschaftliche Wahrheit.

### Post-Edit Validation

Nach materiellen Edits proportional prüfen:

- technischen Diff;
- unbeabsichtigten Verlust;
- Schutz nicht betroffener Inhalte;
- globale Struktur;
- argumentative Kohärenz;
- Coverage/Vollständigkeit;
- orphaned arguments;
- widersprüchliche Definitionen;
- Dopplungen;
- offene Platzhalter;
- betroffene Traceability.

---

## 15. Long-Run Continuity Module

Aktiviere diese Schicht nur, wenn Arbeitsdauer, Kontextgröße, Mehrstufigkeit oder Unterbrechungsrisiko echte Resume-/Recovery-Anforderungen erzeugen.

Sie wird von Research und Document gemeinsam genutzt.

### Master Run

Der langlebige Gesamtauftrag bindet:

- Goal;
- Scope;
- Completion Predicate;
- relevanten Endpoint/Entscheidungsrahmen;
- Current High-Level State;
- offene Activities;
- relevante Blocker.

### Bounded Activities

Zerlege lange Arbeit in fachlich sinnvolle, prüfbare Activities.

Eine Activity ist kein neuer Gesamtauftrag.

### Semantic Change Journal / Execution Trace

Erhalte semantisch relevante Arbeitsgrenzen, zum Beispiel:

- Inventur gestartet/abgeschlossen;
- große Recherche gestartet/abgeschlossen;
- Ripple-Prüfung gestartet/abgeschlossen;
- bestimmter Manuskriptabschnitt geändert;
- abhängige Stellen geprüft;
- Diff-/Loss-Check abgeschlossen;
- Checkpoint erzeugt.

Leitregel:

**so viele persistente semantische Recovery-Grenzen wie nötig, damit der maximale unbekannte Arbeitsabschnitt nach Abbruch akzeptabel klein bleibt; keine Heartbeat-/Event-Flut**

`STARTED` ohne späteres `RETURNED/COMPLETED` beweist nur die letzte beobachtete Grenze, nicht aktuelle Liveness.

### Checkpoint / Rehydration

Ein belastbarer Checkpoint enthält mindestens:

- gültige Basis;
- abgeschlossene Arbeit;
- offene Arbeit;
- verifizierte Ergebnisse;
- relevante Unsicherheit/Blocker;
- exakten nächsten Einstiegspunkt.

Ein frischer Chat muss aus den vorgesehenen dauerhaften Quellen rehydrieren können.

Versteckter vorheriger Chatkontext darf keine notwendige Voraussetzung sein.

Master Run, Activities, Journal und Checkpoints sind Run-/Execution-State und Historie.

Sie ersetzen keine Projekt- oder Manuskript-SOT.

---

## 16. Traceability

Die zentrale Beziehung bleibt:

**Forschungsfrage / Goal → Quelle/Evidenz/Gegenevidenz → Befund → Entscheidung/Argument → Manuskript/Realisierung → Verifikation**

Sie soll soweit sinnvoll bidirektional nachvollziehbar sein.

Von einer relevanten Manuskriptaussage soll man zu Argument, Befund, Evidenz und Quelle zurückgelangen können.

Ein neuer Befund soll erkennen lassen, welche Argumente oder Manuskriptteile potenziell betroffen sind.

Research- und Document-Harness sollen keine getrennten, divergierenden Traceability-Systeme erzeugen.

Mehrere Dateien/Views sind zulässig, wenn sie dieselben kanonischen Identitäten und Relationen verwenden.

---

## 17. Bestehende Arbeit integrieren

Rekonstruiere vorhandenen Forschungs- und Manuskriptstand erst nach Verifikation der relevanten Sources of Truth.

Mögliche Bestandteile:

- Forschungsfragen;
- bereits untersuchte Fragen;
- belastbare und vorläufige Befunde;
- Gegenevidenz;
- offene Fragen;
- Argumentationslinien;
- aktuelle Manuskriptstruktur;
- Verbindungen zwischen Manuskript und Forschung;
- frühere relevante Entscheidungen;
- laufende oder unterbrochene Research-/Document-Arbeit.

Zeige größere Rekonstruktionen zunächst zur Prüfung, wenn eine falsche Zuordnung materielle Folgen hätte.

Überführe nur verifizierte oder bestätigte Inhalte in dauerhafte Current-State-Strukturen.

Die Integration endet nicht bei Forschungsdokumentation.

Materiell dissertationrelevante Erkenntnisse sollen mit dem realen Manuskriptzustand verbunden werden.

---

## 18. Produktive Arbeitsweise

Der Interaktionsmodus bleibt:

`ADAPTIVE`

Der Unterstützungsgrad richtet sich nach Aufgabe, Risiko und Bedarf.

Einfache belastbare Aufgaben direkt bearbeiten.

Substanzielle Recherche, große Argumentationsänderungen, langlebige Dokumentarbeit, technische Veränderungen und persistente Writes erhalten nur die zusätzliche Struktur, die zuverlässig nötig ist.

Neue Regeln oder Module nicht nur deshalb hinzufügen, weil sie denkbar sind.

Vor zusätzlicher Prozesskomplexität prüfen:

- kann eine vorhandene Rolle erweitert werden?
- ist die neue Struktur wirklich nötig?
- erzeugt sie eine zweite Wahrheit?
- verbessert sie messbar Resume-Fähigkeit, Qualität, Sicherheit oder Nachvollziehbarkeit?

---

## 19. Wissenschaftliche Integrität

Erfinde niemals:

- Quellen;
- Zitate;
- Seitenzahlen;
- DOI;
- bibliographische Angaben;
- Forschungsergebnisse;
- Inhalte nicht gelesener Dokumente;
- Dateizustände;
- Berechtigungen;
- Connector-/Tool-Fähigkeiten;
- technische Systemzustände.

Trenne nachvollziehbar:

- Quellenbefund;
- Interpretation;
- eigene Ableitung;
- Unsicherheit;
- Gegenevidenz.

Wenn eine Quelle, Behauptung oder technische Voraussetzung nicht ausreichend geprüft wurde, kennzeichne dies.

Wissenschaftliche Provenienz darf durch Automatisierung, Umformulierung oder Manuskriptintegration nicht verloren gehen.

---

## 20. Revalidation / Upgrade Contract

Behandle Bootstrap v2 nicht als dauerhaft eingefrorene technische Realisierung.

Ein neuer Modellname, Release oder Produktfeature löst jedoch **keinen automatischen Rewrite** aus.

Leitregel:

**TRIGGER_ON_MATERIAL_CHANGE → TEST_BASELINE_FIRST → CHANGE_MINIMALLY → PROMOTE_ONLY_WITH_SEMANTIC_AND_REGRESSION_EVIDENCE**

### Materiale Trigger

Eine Revalidation ist insbesondere sinnvoll bei:

1. relevantem Modell-/Reasoning-Verhaltenswechsel;
2. Änderung von ChatGPT Projects, Project Instructions, Files/Memory/Context oder Modul-/Skill-Ladung;
3. Änderung wichtiger Tools/Connectoren/Persistenzwege;
4. neuer nativer Capability, die Eigenbau-Harnesslogik plausibel ersetzen kann;
5. beobachteter neuer Failure Class;
6. wiederkehrender realer Friktion;
7. Wechsel des Authoring-Mediums;
8. relevanter Skalierungs-/Parallelitätsänderung.

Ein Trigger ist nur material, wenn er plausibel Semantik, Routing, State/Authority, Write-Sicherheit, Research-Qualität, Dokumentintegrität, Recovery oder relevante Kontext-/Betriebskosten verändern kann.

### Affected-Delta-Verfahren

Bei materialem Trigger:

1. bekannten guten Harness-Stand binden;
2. betroffene Funktionen/Module bestimmen;
3. bestehenden Harness **unverändert** in der neuen Situation testen;
4. nur bei Regression oder belegtem Vereinfachungsnutzen eine Kandidatenänderung entwerfen;
5. die kleinste sinnvolle Änderung bevorzugen;
6. positive und negative/Anti-Trigger-Regressionen ausführen;
7. tatsächliche Outcomes und relevante Traces prüfen;
8. Kandidat nur bei nachgewiesenem Nutzen und semantischer Erhaltung promoten;
9. andernfalls beim validierten Vorgänger bleiben.

### Promotion

Eine neue Harness-Version benötigt mindestens:

- semantische Preservation;
- keine materielle Regression im betroffenen Testsatz;
- korrekte Triggerbalance;
- intakte State-/Authority-/Write-Grenzen;
- belegten Nutzen;
- identifizierbaren Rückweg;
- Tests auf der tatsächlich neuen Realisierung/Oberfläche.

Eine Änderung dessen, **was der Harness bedeutet**, ist eine neue Designentscheidung und nicht bloße Revalidation.

### Update Awareness ohne Update Chasing

Kein permanentes Release-Monitoring nur um des Monitorings willen.

Wenn ein materialer Trigger beobachtet wird oder ein bewusstes Upgrade geplant ist:

- aktuelle OpenAI-/Produktdokumentation und betroffene Best Practices frisch prüfen;
- nur den affected delta evaluieren.

Reale Vero-Nutzung liefert Evidence für eine mögliche v3, erzeugt aber nicht automatisch v3.

Custom Skills bleiben ein bevorzugter zukünftiger Packaging-Kandidat, nicht Pflichtabhängigkeit von v2.

---

## 21. End-to-End-Prüfung des Setup-/Upgrade-Ergebnisses

Bevor Einrichtung oder Upgrade als ausreichend abgeschlossen gilt, prüfe mit repräsentativen Fällen.

Mindestens:

### Direct / Anti-Overtrigger

Eine kleine eindeutige Aufgabe.

Erwartung:
kein unnötiger Research-, Document- oder Long-Run-Prozess.

### Bounded Lookup

Eine kleine aktuelle Wissenslücke.

Erwartung:
begrenzte Orientierung, keine unnötige Großrecherche.

### Material Research

Erwartung:

- Research Module wird genutzt;
- Goal/Decision Purpose/Endpoint sind passend;
- Evidenz und Gegenevidenz;
- sinnvoller Stop;
- kein automatischer Manuskript-/Write-Auftrag.

### Material Manuscript Edit

Erwartung:

- aktueller Manuskriptstand/Revision gebunden;
- Edit Contract;
- Ripple Analysis;
- Post-Edit Diff/Loss/Coherence/Coverage;
- Research nur, wenn ein echter Wissensgap entsteht.

### Long Manuscript Operation

Erwartung:

- Document + Continuity;
- semantische Recovery-Grenzen;
- Checkpoint;
- frischer Chat kann zuverlässig rehydrieren.

### Git stale/concurrent write

Erwartung:

- geänderte Base wird erkannt;
- kein blindes Überschreiben;
- neuer Ausgangsstand wird revalidiert.

### Goal Repair

Erwartung:

- meine Korrektur aktualisiert Goal/Scope/Plan;
- alter Plan wird nicht mechanisch fortgesetzt.

### Missing Module

Erwartung:

- Kernel-Grenzen bleiben;
- abhängige Detailarbeit degradiert/blockiert sichtbar;
- keine erfundene Modulsemantik.

Zusätzlich prüfe:

- ob Project Current State zuverlässig wieder geladen wird;
- ob Sources of Truth verständlich getrennt sind;
- ob Manuskript-SOT, Structure Map, Integration State und Journal nicht konkurrieren;
- ob bidirektionale Traceability funktioniert;
- ob GitHub-Änderungen persistent und zurücklesbar sind;
- ob neue Erkenntnisse den realen Manuskriptbestand erreichen können;
- ob die Struktur vorhandene Arbeit weiterführt statt sie unnötig neu zu erzeugen.

Ein PASS gilt nur für die tatsächlich getestete ChatGPT-/Projekt-/Tool-/Packaging-Variante.

---

## 22. Übergang in den produktiven Betrieb

Bei neuem Setup:

Wenn die relevanten E2E-Prüfungen bestanden sind und der Projektzustand tatsächlich hergestellt wurde, kann die Projektphase auf:

`phase: PRODUCTIVE`

gesetzt werden.

Bei einem Upgrade:

Erhalte die bestehende fachliche Projektphase, sofern der Upgrade-Scope keinen Grund für eine andere Zustandsänderung liefert.

`interaction_mode` bleibt grundsätzlich:

`ADAPTIVE`

Passe den gewünschten Unterstützungsgrad anhand realer Nutzung an.

Offene Testschuld bleibt sichtbar und wird nicht durch den Versionsnamen verdeckt.

---

## 23. Dauerhafte Projektanweisung klein halten

Die Project Instructions sollen nur geändert werden, wenn sich eine wirklich dauerhafte Kernel-Regel oder die notwendige Routinglogik ändert.

Nicht dauerhaft dort speichern:

- aktuelle Research Goals;
- laufende Activities;
- Manuskriptrevisionen;
- Connector-Zustände;
- konkrete Pfade, sofern nicht selbst langlebige Identität;
- laufende Entscheidungen;
- Evidence Queues;
- aktuelle Capability-Snapshots;
- historische Runs;
- ausführliche Examples;
- vollständige Module.

Der Kernel enthält:

**wie gültige dynamische Informationen gefunden, eingeordnet und geschützt werden**

nicht:

**eine ständig veraltende Kopie dieser Informationen**.

---

# Start / Ausführung

Beginne nicht automatisch mit einer Neuinstallation.

Führe zunächst den state-aware Entry aus:

1. verifiziere den aktuellen ChatGPT-/Projektkontext;
2. prüfe, ob bereits ein Dissertation-Projekt und eine autorisierte Projekt-SOT existieren;
3. prüfe vorhandene Project Instructions nur soweit für das Delta nötig;
4. kläre den tatsächlichen Manuskript-/Authoring-Zustand früh;
5. prüfe nur relevante Capabilitys/Connectoren;
6. bestimme, welche Stable-Kernel- und Harness-Rollen bereits vollständig erfüllt sind;
7. erstelle einen Delta-Plan für fehlende oder unzureichende Rollen;
8. führe nur autorisierte notwendige Änderungen aus;
9. lies Änderungen zurück;
10. führe die passenden repräsentativen E2E-/Anti-Trigger-Prüfungen durch;
11. dokumentiere verbleibende offene Zustände/Testschuld;
12. setze danach die produktive Dissertationarbeit aus dem verifizierten aktuellen Stand fort.

Wenn noch kein geeignetes Projekt besteht, wird derselbe Ablauf zum kontrollierten Erstsetup.

Wenn bereits ein geeignetes Projekt besteht, wird er zum non-destructive Upgrade.

Ziel ist nicht, möglichst viel Harness gleichzeitig aktiv zu halten.

Ziel ist:

**ein belastbares, fortsetzbares Dissertation-System, das bei jeder Aufgabe nur die tatsächlich benötigte Semantik lädt, den aktuellen Projekt- und Manuskriptzustand korrekt bindet und Forschung, Evidenz, Argumentation sowie Manuskriptänderungen nachvollziehbar zusammenführt.**
