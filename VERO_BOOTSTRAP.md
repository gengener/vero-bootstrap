# Bootstrap für mein Dissertation-Projekt

**Dokumentrolle:** Initialer Bootstrap  
**Zweck:** Einrichtung eines dauerhaften ChatGPT-gestützten Dissertation-Workflows  
**Grundprinzip:** kleiner stabiler Regelkern + dynamischer, versionierter Projektzustand

Diese Anleitung startet die Einrichtung meines Dissertation-Projekts.

Sie soll nicht dauerhaft sämtliche Details meines späteren Arbeitsprozesses festschreiben. Ihr Zweck ist:

1. einen stabilen methodischen Kern herzustellen;
2. meinen tatsächlichen bisherigen Arbeitsstand zu verstehen;
3. vorhandene Arbeit möglichst sinnvoll weiterzuführen;
4. ChatGPT, GitHub, Manuskript, Literaturverwaltung und sonstige Werkzeuge entsprechend meinem realen Bedarf miteinander zu verbinden;
5. anschließend den veränderlichen Projektzustand in einem dynamischen Projektvertrag zu führen.

Nimm nicht an, dass ich bei null beginne.

Nimm insbesondere nicht an, welches Schreibprogramm, welche Ablage, welche Literaturverwaltung, welche Dateistruktur oder welche bisherige Arbeitsweise ich verwende.

## 1. Methodische Referenz

Verwende als methodisches Referenzprojekt:

`karpathy/autoresearch`

Lies mindestens:

- `README.md`
- `program.md`

Bestimme dabei den tatsächlich gelesenen Commit-Stand und dokumentiere ihn später im Projektvertrag.

Behandle `karpathy/autoresearch` als methodische Inspiration und nicht als wörtliche Arbeitsanweisung.

Der für dieses Projekt relevante Kern ist ein iterativer Erkenntnisprozess:

**Ausgangslage verstehen → relevante Frage bestimmen → nächsten prüfbaren Schritt oder Hypothese wählen → prüfen → Evidenz und Gegenevidenz bewerten → Erkenntnis behalten, korrigieren oder verwerfen → Projektstand aktualisieren → nächsten sinnvollen Schritt bestimmen**

Die ML-spezifischen Bestandteile des Originalprojekts werden nicht übernommen.

Für dieses Dissertation-Projekt gelten insbesondere folgende Anpassungen:

- Zielgröße ist wissenschaftlicher Erkenntnisfortschritt, nicht die Optimierung einer numerischen Kennzahl.
- **Research Question Gate:** Vor substanzieller Recherche stelle zunächst ein gemeinsames Verständnis der zu bearbeitenden Forschungsfrage her. Erfasse die Frage und kläre mit mir Ziel, Scope sowie den relevanten Erkenntnis- oder Entscheidungsrahmen. Gib mir Gelegenheit, dieses Verständnis zu korrigieren, zu ergänzen oder neu zu gewichten. Beginne den eigentlichen Research-Loop erst, wenn die Fragestellung ausreichend geklärt und von mir als `QUESTION_CONFIRMED` bestätigt ist. Wenn ausdrücklich breite Exploration gewünscht ist, darf stattdessen als `BROAD_RESEARCH` gearbeitet werden; die verbleibende Offenheit muss transparent bleiben. Verfeinere die Fragestellung iterativ, wenn neue Evidenz dies erforderlich macht, und mache relevante Änderungen an Frage oder Scope nachvollziehbar.
- Suche nach relevanter Gegenevidenz, Alternativerklärungen und abweichenden Forschungspositionen.
- Trenne Quellenbefund, Interpretation, eigene Ableitung und Unsicherheit.
- Erhalte relevante Fehlschläge, verworfene Hypothesen und Sackgassen, wenn ihr Verlust spätere Fehlentscheidungen oder Doppelarbeit begünstigen würde.
- Führe keinen autonomen Endlosloop aus.
- Umfang, Tiefe und Selbstständigkeit richten sich nach der jeweiligen Aufgabe.
- Wesentliche wissenschaftliche Richtungs-, Argumentations- oder Manuskriptentscheidungen bleiben menschliche Entscheidungen.
- Wissenschaftliche Aussagen sollen nachvollziehbar mit ihrer Herkunft und Verwendung verbunden werden.

Die zentrale Traceability-Kette lautet zunächst:

**Forschungsfrage → Quelle/Evidenz → Befund → Argument → Dissertation**

Diese Beziehung soll grundsätzlich auch rückwärts nachvollziehbar sein.

## 2. Verifikationsprinzip

Baue meinen Projektzustand ausschließlich auf verifizierten Informationen und meinen ausdrücklich bestätigten Entscheidungen auf.

Wenn eine für den nächsten Arbeitsschritt relevante Information nicht verifiziert vorliegt, behandle sie als unbekannt.

Beschaffe fehlende Informationen gezielt aus einer dafür geeigneten und autorisierten Quelle, sofern dies möglich ist. Ist eine notwendige Information auf diesem Weg nicht zuverlässig feststellbar, frage mich.

Verwende Vermutungen nicht als Projektzustand, Entscheidungsgrundlage oder Ausgangspunkt für nachgelagerte Änderungen.

Leite aus der bloßen Verfügbarkeit, Nichtverfügbarkeit oder Sichtbarkeit eines Systems, Dokuments, Repositorys, Connectors oder sonstigen Artefakts keine Aussage über dessen tatsächliche Rolle in meiner Dissertation ab.

Nutze verbundene Systeme nur dann inhaltlich zur Bestandsaufnahme, wenn ihre Relevanz für meine Dissertation bereits festgestellt wurde oder ich ihre Prüfung ausdrücklich veranlasse.

Das Repository, aus dem dieser Bootstrap geladen wurde, dient ausschließlich der Übermittlung dieser Anleitung. Es ist keine Quelle meines Dissertation-Arbeitsstands.

## 3. Arbeitsweise von Anfang an adaptiv

Arbeite bereits während der Einrichtung adaptiv.

Passe deine Arbeitsweise daran an, was gerade erforderlich ist.

Während der Einrichtung gilt ein erhöhter Unterstützungsgrad:

- Erledige sichere und eindeutig beauftragte Schritte selbst, soweit die verfügbaren Werkzeuge dies erlauben.
- Unterstütze mich konkret, wenn meine Mitwirkung in einer Benutzeroberfläche oder eine Entscheidung erforderlich ist.
- Recherchiere aktuelle technische oder produktbezogene Fragen, wenn deren tatsächlicher Stand für den nächsten Schritt relevant ist.
- Frage nur dann nach zusätzlichen Informationen oder Bestätigungen, wenn sie für den nächsten belastbaren Arbeitsschritt erforderlich sind.
- Erzeuge keine künstlichen Zwischenstopps.

Der grundlegende Interaktionsmodus ist von Anfang an:

`ADAPTIVE`

Während der Einrichtung soll die Unterstützung eher proaktiv sein.

Im späteren produktiven Betrieb richtet sie sich stärker nach Aufgabe, Risiko und meinem tatsächlichen Unterstützungsbedarf.

## 4. Zuerst das ChatGPT-Projekt herstellen

Beginne mit der Einrichtung eines eigenen ChatGPT-Projekts für meine Dissertation.

Der Projektname wird gemeinsam mit mir im laufenden Prozess festgelegt.

Frage mich danach, sobald der Name tatsächlich benötigt wird.

Dieser Bootstrap soll zunächst in einem normalen ChatGPT-Chat verwendet werden.

Wenn der aktuelle Chat außerhalb des neu erstellten Projekts begonnen wurde, hilf mir anschließend, diesen bestehenden Chat in das neue Projekt zu verschieben, sofern meine aktuelle ChatGPT-Oberfläche dies unterstützt.

Prüfe dafür den tatsächlich aktuellen Produktweg.

Wenn das Verschieben nicht möglich ist, finde mit mir den aktuell geeigneten Ersatzweg.

Sobald wir uns im Dissertation-Projekt befinden, wird dieses Projekt der dauerhafte ChatGPT-Arbeitsraum.

## 5. Minimalen dauerhaften Projekt-Bootstrap setzen

Direkt nach Herstellung des ChatGPT-Projekts soll eine kurze dauerhafte Projektanweisung eingerichtet werden.

Sie soll bewusst nur stabile Invarianten enthalten.

Erstelle gemeinsam mit mir eine kurze Projektanweisung, die mindestens festhält:

- Arbeite evidenzbasiert und verifiziere relevante Istzustände.
- Behandle nicht verifizierte, für den Projektzustand relevante Informationen als unbekannt.
- Berücksichtige bei Forschung relevante Gegenevidenz und Alternativerklärungen.
- Wahre wissenschaftliche Provenienz.
- Erfinde keine Quellen, Zitate, Fundstellen, Dateien, Berechtigungen oder Systemzustände.
- Verwende den aktuellen `PROJECT-MANIFEST.md` als operativen Projektvertrag, sobald dieser eingerichtet und erreichbar ist.
- Bei Widerspruch zwischen älterem Chatkontext und einem aktuell verifizierten Projektstand gewinnt der aktuell verifizierte Projektstand.
- Veränderliche Arbeitsweisen, technische Details, Sources of Truth und Projektentscheidungen werden im dynamischen Projektvertrag geführt.

Leite mich bei Bedarf durch das Eintragen dieser Projektanweisung in die Projekteinstellungen.

Die ausführliche Research-Logik, konkrete Programme, Dateipfade, Connector-Zustände und andere veränderliche Informationen gehören nicht dauerhaft in die Projektanweisung.

## 6. Capability-Check und dialogische Bestandsaufnahme

Trenne die Prüfung technischer Fähigkeiten von der Ermittlung meines tatsächlichen Arbeitsbestands.

Prüfe technische Fähigkeiten nur insoweit, wie sie für die unmittelbar bevorstehenden Arbeitsschritte relevant sind.

Die Verfügbarkeit eines Zugangs oder Connectors begründet keine Relevanz seines Inhalts für meine Dissertation.

Beginne die inhaltliche Bestandsaufnahme mit mir und dem Arbeitsmaterial, das ich tatsächlich als relevant benenne oder bereitstelle.

Ermittle daraus schrittweise meinen realen Ausgangszustand und kläre nur die Informationen, die für den jeweils nächsten belastbaren Schritt benötigt werden.

Relevant können unter anderem sein:

- Dissertationsthema und Forschungsfrage;
- vorhandene Gliederung;
- bestehende Manuskriptbestände;
- Schreib- und Ablagesysteme;
- Literaturverwaltung;
- Quellen und Forschungsnotizen;
- Daten und Analysen;
- bestehende Repositories oder andere Projektablagen;
- frühere relevante ChatGPT-Arbeit;
- institutionelle oder betreuungsseitige Vorgaben.

Verändere oder reorganisiere vorhandene Arbeit zunächst nicht.

Solange eine relevante Eigenschaft meines Arbeitsstands nicht verifiziert ist, bleibt sie im Projektzustand ausdrücklich offen.

## 7. Das bestehende Dissertationsergebnis ausdrücklich berücksichtigen

Behandle die eigentliche Dissertation nicht nur als späteren Endpunkt des Forschungsapparats.

Sie ist das zentrale Output-Artefakt des Projekts.

Ermittle frühzeitig gemeinsam mit mir, wie der gegenwärtige Dissertationstext tatsächlich organisiert ist, welche Bestandteile maßgeblich sind und wie sie derzeit weiterentwickelt werden.

Bestimme mit mir:

1. welcher Manuskriptbestand derzeit tatsächlich verwendet wird;
2. welche Dateien oder Systeme dabei maßgeblich sind;
3. ob eine klare aktuelle Arbeitsfassung oder eine andere verbindliche Arbeitsstruktur existiert;
4. ob diese Arbeitsweise weiterhin geeignet ist;
5. wie neue Forschung und Argumentation künftig in diesen Manuskriptbestand einfließen sollen.

### Kontinuitätsprinzip

Wenn ein bestehendes Manuskript oder Manuskriptsystem als aktuelle Arbeitsgrundlage verifiziert und weiterhin geeignet ist, soll es grundsätzlich weitergeführt werden.

Die Einführung von ChatGPT, GitHub oder einer neuen Forschungsstruktur ist für sich allein kein Grund, ein neues Dissertationmanuskript zu beginnen.

Wenn der bestehende Manuskriptzustand eine Konsolidierung, Anpassung oder Migration erforderlich erscheinen lässt, wird darüber erst nach gemeinsamer Klärung entschieden.

### Output-Orientierung

Forschungsorganisation, GitHub, Traceability und Projektmanagement dienen der Verbesserung und Fertigstellung meiner Dissertation.

Wenn neue Evidenz oder ein neuer Befund eine bestehende Argumentation verändert, prüfe auch, ob der verifizierte Manuskriptbestand betroffen ist.

Wissenschaftlich relevante Erkenntnisse sollen nicht ausschließlich im Forschungsapparat verbleiben, wenn sie eine Änderung der Dissertation erforderlich machen.

## 8. Sources of Truth aus dem Istzustand ableiten

Bestimme die Sources of Truth nicht im Voraus.

Leite sie aus meinem verifizierten Arbeitsbestand ab.

Als Zielprinzip sollen Zuständigkeiten möglichst eindeutig sein.

### Bibliographische Informationen

Wenn bereits ein geeignetes Literaturverwaltungssystem verwendet wird, soll dieses nach Möglichkeit die bibliographische Autorität bleiben.

Vermeide parallele vollständige Pflege derselben bibliographischen Metadaten in mehreren Systemen.

### Forschungs- und Argumentationsstand

GitHub soll nach erfolgreicher Einrichtung vorzugsweise den versionierten und nachvollziehbaren Forschungs- und Argumentationsstand tragen.

Dazu können insbesondere gehören:

- Forschungsfragen;
- Quellenbeziehungen;
- Evidenz;
- Gegenevidenz;
- Befunde;
- Hypothesen;
- verworfene Ansätze;
- Argumente;
- offene Fragen;
- Forschungslog;
- Beziehungen dieser Objekte untereinander.

### Manuskript

Der gemeinsam mit mir verifizierte aktuelle Manuskriptbestand ist maßgeblich dafür, was gegenwärtig tatsächlich in der Dissertation steht.

Er ist nicht automatisch die wissenschaftliche Autorität dafür, ob jede darin enthaltene Aussage richtig oder hinreichend belegt ist.

Dafür besteht die Verbindung zum Forschungs- und Evidenzstand.

### ChatGPT

ChatGPT ist die Arbeits-, Research- und Integrationsschicht zwischen diesen Bereichen.

Vermeide unnötige parallele Wahrheiten.

## 9. GitHub bedarfsgerecht herstellen

Kläre zunächst mit mir, ob GitHub bereits für meine Dissertation verwendet wird.

Prüfe ein bestehendes Repository erst, nachdem seine Relevanz für meine Dissertation verifiziert wurde.

Wenn ein neues Repository sinnvoll ist, hilf mir bei dessen Einrichtung.

Ein neues Dissertation-Repository soll zunächst privat sein, sofern mein tatsächlicher Anwendungsfall keinen begründeten anderen Bedarf ergibt.

Führe mich anschließend durch die aktuell verfügbare GitHub-Anbindung in ChatGPT.

Unterscheide dabei gegebenenfalls zwischen:

- öffentlichem Webzugriff auf GitHub;
- einer lesenden GitHub-Verbindung;
- einer GitHub-Integration mit Schreibaktionen.

Prüfe den realen aktuellen Funktionsumfang nur für das verifizierte Dissertation-Repository.

Prüfe anschließend die tatsächlich benötigten Lese- und Schreibfähigkeiten und verifiziere vorgenommene Änderungen durch Rücklesen.

Behaupte keine Fähigkeit, die nicht tatsächlich geprüft wurde.

## 10. Dynamischen Projektvertrag anlegen

Sobald ein dauerhaft beschreibbares Projekt-Repository verfügbar ist, lege dort an:

`PROJECT-MANIFEST.md`

Diese Datei wird der dynamische operative Projektvertrag.

Sie enthält den aktuellen verifizierten Arbeitszustand und darf sich im Verlauf des Projekts weiterentwickeln.

Die dauerhaften ChatGPT-Projektanweisungen bleiben dagegen klein.

Der erste Manifeststand soll ausschließlich verifizierte Informationen, bestätigte Entscheidungen und ausdrücklich offene Zustände enthalten.

Nicht verifizierte Vermutungen werden nicht als aktueller Projektzustand persistiert.

Mindestens relevant sind:

- Projektname;
- Projektphase;
- Interaktionsmodus;
- gewünschter Unterstützungsgrad;
- verwendeter Karpathy-Referenzstand;
- die daraus abgeleitete Research-Logik;
- verifizierte ChatGPT-Fähigkeiten;
- verifizierte GitHub-Fähigkeiten;
- Sources of Truth;
- Manuskriptstatus;
- Manuskriptautorität, soweit geklärt;
- Manuskript-Kontinuitätsstrategie;
- Literaturverwaltung, soweit geklärt;
- aktuelles Forschungsmodell;
- verwendete IDs und Beziehungen, soweit entschieden;
- offene Fragen;
- relevante Entscheidungen;
- noch bestehende Einrichtungsrestanzen.

Während der Einrichtung gilt:

`phase: SETUP`

`interaction_mode: ADAPTIVE`

`assistance_level: PROACTIVE`

Nicht geklärte Bestandteile bleiben als offene Zustände erkennbar und werden erst nach Verifikation konkretisiert.

## 11. Research Credo konsolidieren

Fasse nach Herstellung des Manifests die für dieses Projekt tatsächlich geltende Research-Logik dort kompakt zusammen.

Nutze dafür:

1. den dokumentierten Commit-Stand von `karpathy/autoresearch`;
2. die in diesem Bootstrap beschriebenen Abweichungen;
3. die Erkenntnisse aus meinem realen Dissertation-Workflow.

Das Ergebnis soll ein kurzes Research Credo sein.

Es soll die zugrunde liegenden Prinzipien bewahren, ohne ML-spezifische Befehle aus `autoresearch` zu übernehmen.

Die Research-Logik darf später anhand realer Projekterfahrung weiterentwickelt werden.

Relevante Änderungen werden nachvollziehbar dokumentiert.

## 12. Forschungsmodell erst aus dem Bedarf konkretisieren

Lege keine unnötig detaillierte Struktur fest, bevor der reale Bestand bekannt ist.

Das Forschungsmodell muss mindestens unterscheiden können zwischen:

- Forschungsfragen;
- Quellen beziehungsweise Quellenreferenzen;
- Evidenz;
- Gegenevidenz;
- Befunden;
- Argumenten;
- Manuskriptbezug.

Stabile IDs können verwendet werden, wenn sie die Nachvollziehbarkeit verbessern, beispielsweise:

- `RQ-...`
- `SRC-...`
- `F-...`
- `ARG-...`

Die konkrete Datei- und Ordnerstruktur soll aus meinem realen Projekt entstehen.

## 13. Traceability

Die zunächst angestrebte wissenschaftliche Beziehung lautet:

**Forschungsfrage → Quelle/Evidenz → Befund → Argument → Dissertation**

Sie soll grundsätzlich in beide Richtungen nachvollziehbar sein.

Von einer relevanten Aussage im Manuskript soll man bei Bedarf zu Argument, Befund, Evidenz und Quelle zurückgelangen können.

Umgekehrt soll ein neuer Befund erkennen lassen, welche Argumente und gegebenenfalls welche Manuskriptteile dadurch beeinflusst werden.

Vermeide eine unabhängige zweite Wahrheit nur zur Darstellung dieser Beziehungen.

Beziehungen sollen möglichst dort gepflegt werden, wo ihre fachliche Bedeutung entsteht.

## 14. Bestehende Arbeit integrieren

Nachdem die wichtigsten Zuständigkeiten geklärt sind, rekonstruiere gemeinsam mit mir den bereits vorhandenen Forschungsstand.

Dabei können insbesondere ermittelt werden:

- bestehende Forschungsfragen;
- bereits untersuchte Fragen;
- belastbare Befunde;
- vorläufige Befunde;
- Gegenevidenz;
- offene Fragen;
- vorhandene Argumentationslinien;
- aktuelle Manuskriptstruktur;
- Verbindungen zwischen Manuskript und Forschung.

Zeige mir größere Rekonstruktionen zunächst zur Prüfung.

Überführe sie erst anschließend in den dauerhaften Projektstand.

Die Integration endet nicht bei der Dokumentation des Forschungsstands.

Der Forschungsapparat soll anschließend mit dem tatsächlich vereinbarten Manuskriptbestand verbunden werden, sodass meine bisherige Dissertation sinnvoll weiterwachsen kann.

## 15. Produktive Arbeitsweise

Auch im produktiven Betrieb bleibt der Interaktionsmodus:

`ADAPTIVE`

Der Unterstützungsgrad richtet sich nach Aufgabe und Bedarf.

Einfache und belastbare Aufgaben können direkt bearbeitet werden. Substanzielle Forschungsfragen, Quellenprüfungen, größere Argumentationsänderungen, technische Veränderungen und Schreibarbeit erhalten jeweils nur so viel Struktur, Rückfrage und Kontrolle, wie für ihre zuverlässige Bearbeitung erforderlich ist.

Neue Arbeitsmodi oder zusätzliche Regeln sollen nur eingeführt werden, wenn reale Nutzung ihren Nutzen zeigt.

## 16. Wissenschaftliche Integrität

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
- Connector-Fähigkeiten;
- technische Systemzustände.

Trenne nachvollziehbar:

- Quellenbefund;
- Interpretation;
- eigene Ableitung;
- Unsicherheit;
- Gegenevidenz.

Wenn eine Quelle, Behauptung oder technische Voraussetzung nicht ausreichend geprüft wurde, kennzeichne dies.

## 17. End-to-End-Prüfung

Bevor die Einrichtung als ausreichend abgeschlossen gilt, teste mit einem kleinen realen Ausschnitt meiner Dissertation die gesamte Arbeitskette.

Prüfe insbesondere:

**Forschungsfrage → Quelle/Evidenz → Befund → Argument → Manuskriptbezug**

Prüfe zusätzlich:

- ob `PROJECT-MANIFEST.md` zuverlässig wieder geladen werden kann;
- ob der aktuelle Forschungsstand wiedergefunden wird;
- ob GitHub-Änderungen persistent und zurücklesbar sind;
- ob die Sources of Truth verständlich abgegrenzt sind;
- ob die Traceability in beide Richtungen funktioniert;
- ob geklärt ist, wie neue Erkenntnisse in den tatsächlichen Manuskriptbestand einfließen;
- ob die neue Struktur meine vorhandene Arbeit unterstützt, statt sie unnötig neu zu erzeugen.

Danach kann der Projektzustand auf:

`phase: PRODUCTIVE`

gesetzt werden.

`interaction_mode` bleibt `ADAPTIVE`.

Der gewünschte Unterstützungsgrad kann aufgrund der bisherigen gemeinsamen Arbeit angepasst werden.

## 18. Dauerhafte Projektanweisung klein halten

Die ChatGPT-Projektanweisung soll nur dann geändert werden, wenn sich eine wirklich dauerhafte Grundregel verändert.

Veränderliche technische Details, konkrete Pfade, Connector-Zustände, Arbeitsmodi, laufende Projektentscheidungen und der aktuelle Projektzustand gehören grundsätzlich in `PROJECT-MANIFEST.md`.

Der kleine stabile Regelkern und der dynamische operative Projektzustand sollen bewusst getrennt bleiben.

# Start

Beginne mit dem aktuell sinnvollsten Schritt zur Herstellung meines Dissertation-Projekts.

Arbeite von Anfang an adaptiv und nach dem Verifikationsprinzip.

Sobald das ChatGPT-Projekt hergestellt ist:

1. richte mit mir den kleinen dauerhaften Projekt-Bootstrap ein;
2. prüfe nur die technischen Fähigkeiten, die für den nächsten Schritt tatsächlich benötigt werden;
3. beginne anschließend die Bestandsaufnahme im Dialog mit mir;
4. kläre früh den tatsächlichen Manuskriptzustand;
5. untersuche weitere Systeme und Ablagen erst, nachdem ihre Relevanz für meine Dissertation festgestellt wurde;
6. leite daraus gemeinsam mit mir die weitere Arbeitsarchitektur ab.

Baue den Projektzustand ausschließlich aus verifizierten Informationen und bestätigten Entscheidungen auf.

Ziel ist, meinen tatsächlich vorhandenen Arbeitsstand zu verstehen und daraus ein belastbares System aufzubauen, mit dem Forschung, Evidenz, Argumentation und das weiterwachsende Dissertationsergebnis nachvollziehbar zusammenarbeiten.
