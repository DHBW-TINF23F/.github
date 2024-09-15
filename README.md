**Informationen zur Softwaretechnik-Vorlesung TINF23F**

[1\. Verfahrensanweisungen 2](#_Toc177036411)

[1.1. Ziel 2](#_Toc177036412)

[1.2. Rahmenbedingungen 2](#_Toc177036413)

[1.3. Bewertung 2](#_Toc177036414)

[1.4. Aufgabenstellung 3](#_Toc177036415)

[1.5. Präsentationen 5](#_Toc177036416)

[1.6. Dokumentation 6](#_Toc177036417)

[1.7. FAQ 9](#_Toc177036418)

[1.8. TINF23F Teilnehmerübersicht 10](#_Toc177036419)

[2\. Projektthemen 11](#_Toc177036420)

[2.1. Mnestix Webclient 12](#_Toc177036421)

[2.2. BaSyx Webclient 13](#_Toc177036422)

[2.3. BaSyx-Editor-Plugin 15](#_Toc177036423)

[2.4. LS2AAS Service 16](#_Toc177036424)

[2.5. Nameplate Generator 17](#_Toc177036425)

[2.6. AAS-Tractus-X 18](#_Toc177036426)

[2.7. AAS Discovery GUI 19](#_Toc177036427)

[2.8. AIMC Configurator 19](#_Toc177036428)

# **Verfahrensanweisungen**

# **Ziel**

Das vorlesungsbegleitende Software-Projekt soll Ihnen erste Erfahrungen hinsichtlich des Entwurfs, der Implementierung und der Qualitätssicherung von Software in größerem Umfang und innerhalb eines Projektteams geben.

Dies umfasst die typischen Phasen Analyse, Design, Implementierung bis zum Test im abgebildeten Top-Down-Entwicklungsprozess nach einem Phasenmodell.

Es sollen die in den Vorlesungen besprochenen Techniken zur Anwendung kommen.

# **Rahmenbedingungen**

- Gruppen zu 5-7 Studenten.
- Jeder im Team hat eine oder mehrere bestimmte Rollen und die zugehörigen Aufgaben. Folgende Rollen müssen pro Team besetzt werden:
  - Projektleiter
  - Produktmanager
  - Systemarchitekt (Leitender Entwickler)
  - Testmanager
  - Technischer Redakteur
  - Jeder ist auch Entwickler
- Jeder im Team muss für mindestens ein Programmmodul oder Dokument die Verantwortung inkl. Implementierung übernehmen und dies deutlich kennzeichnen, da es als Grundlage für die individuelle Benotung herangezogen wird.
- Die Projektdokumentation soll in einem Github-Repository abgewickelt werden.
- Die Teamsitzungen mit Beschlüssen, Status und Ergebnissen müssen in einem einfach lesbaren Protokoll im Repository (z.B. fortlaufend aktualisiertes Issue im Issue-Tracker) dokumentiert werden.

# **Bewertung**

Die Note ergibt sich aus Folgender prozentualer Verteilung der Bewertung der Gruppenarbeit:

- 2/3 kollektive Leistung für die Implementierung, Entwicklungsdokumentation und Präsentation
- 1/3 individuelle Leistung des Einzelnen in seiner Rolle und für sein verantwortliches Modul bzw. Dokument. Bitte sorgen Sie dafür, dass Ihr individueller Beitrag klar identifizierbar ist, auch in den Wiki-Beiträgen im Repository!

# **Aufgabenstellung**

**Aufgabe im 3. Semester:**

**Analysephase VL-Wochen 1-6**

1. Bilden Sie Gruppen zu 5-7 Studenten und verteilen Sie Rollen wie beschrieben. Diese Gruppen bleiben für das Semester 3 und 4 bestehen.
2. Suchen Sie sich eines der ausgegebenen Projekte aus.
3. Systematisieren Sie die Anforderungen und ergänzen Sie ggf. zusätzliche Kundenanforderungen, die sich im Gespräch mit dem Auftraggeber (Dozenten) ergeben, in einem CRS.
4. Erstellen Sie einen einfachen (!) Business Case (BC), indem Sie von einer fiktiven kommerziellen Auftragsentwicklung ausgehen.
5. Erstellen Sie eine erste Projektplanung für Ihr Team. Verplanen sie maximal 180 Stunden pro Teammitglied (inklusive Administration und Dokumente schreiben).
6. Erstellen Sie CRS und BC jeweils als Word-Dokument.

Achten Sie auf die in der Vorlesung behandelten Themen Requirements Engineering und Systemanalyse. Versuchen Sie, in Ihrer Gruppe durch Reviews zu gut spezifizierten Anforderungen unter Anwendung der geeigneten Modellierungstechniken zu kommen.

**Designphase VL-Wochen 7-11**

1. Legen Sie pro Team ein GitHub-Repository mit dem Root “**TINF23F/TeamNr/ProjektName**” an, in dem Sie ab dann Ihre Projektartefakte verwalten. Legen Sie dazu jeweils eine Verzeichnisstruktur an wie in Kapitel 1.6 „Dokumentation“ beschrieben.
2. Richten Sie im Repository den Issue-Tracker für die diversen Dokumentreviews und das Team-Protokoll ein, mit jeweils einem eigenen Issue pro Dokument (d.h. CRS, BC, SRS, SAS, STP und für jedes MOD). In diesen Issues werden ggf. auch die jeweiligen Dokumentenstände angehängt.
3. Erstellen Sie im Wiki des Repositories das Pflichtenheft (SRS), in dem das System aus Black-Box-Sicht definiert und modelliert wird.
4. Erstellen Sie im Wiki des Repositories die Architekturspezifikation (SAS), modellieren Sie dort das System aus White-Box-Sicht. Leiten Sie die zu implementierenden Module daraus ab und weisen Sie diese im Projektplan als Arbeitspakete den Teammitgliedern zu. Legen Sie eine entsprechende Verzeichnisstruktur für die zugehörigen Sourcecodedateien in GitHub an.
5. Updaten Sie die Projektplanung im Repository („Projects“ in GitHub). Versuchen Sie dabei, die Aufgaben zu parallelisieren und beachten Sie Abhängigkeiten zwischen Arbeitspaketen.
6. **Die Dozenten raten dringend dazu, bereits im 3. Semester mit der Implementierung eines Prototyps zu beginnen, um das Projektrisiko im 4.Semester entsprechend zu verringern.**
7. Jedes Team präsentiert die Ergebnisse des 3.Semesters in einer 20minütigen Präsentation mit anschließender 10minütiger Verteidigung (üblicherweise im letzten Vorlesungstermin).

**Abzugeben sind am Ende des 3. Semesters zwei Tage vor dem Präsentationstermin folgende Dokumente in elektronischer Form in Ihrem GitHub-Repository:**

- CRS, BC, SRS, SAS, Projektplan
- Sitzungsprotokolle
- Präsentation

**Aufgabe bis Ende des 4. Semesters:**

1. Implementieren Sie das System, testen und integrieren Sie Ihre Module und erstellen Sie dazu die Moduldokumentation (MOD) im Repository.
2. Richten Sie im Repository den Issue-Tracker für den Systemtest ein.
3. Erstellen Sie den Systemtestplan (STP) im Repository.
4. Führen Sie den Systemtest durch und dokumentieren Sie die Ergebnisse in einem Systemtestreport (STR).
5. Finalisieren Sie alle abzugebenden Dokumente.
6. Jedes Team präsentiert seine Ergebnisse in einer 20minütigen Präsentation mit anschließender 10minütiger Verteidigung.

**Abzugeben sind eine Woche vor dem Präsentationstermin sämtliche Projektdokumente in elektronischer Form (PDF und Basisformat) in Ihrem GitHub-Repository:**

- CRS, BC, SRS, SAS, Projektplan, MODs, STP, STR, Benutzer Manual, Protokolle, Sourcen, Executable.

**Am Tag vor der Präsentation ist auch die finale Projektpräsentation bereitzustellen.**

# **Präsentationen**

**Allgemeines**

- Zeitvorgabe (möglichst genau) 20 min
- Etwa 10 min Fragen
- Sie dürfen selbst entscheiden, wer und wie viele präsentieren.
- Da Sie sehr viele Informationen in 20 Minuten darstellen müssen, überlegen Sie sich genau, was Sie sagen wollen und welche Informationen auf die Folien kommen. Planen Sie daher zur Vorbereitung der Präsentation ausreichend Zeit ein (30 min bis 1h pro Folie!).
- Faustregel für die Anzahl der Folien ist eine nichtanimierte Folie pro Minute, mit Animationen werden es entsprechend weniger Folien.

**Präsentation 1 - BC/CRS/SRS/SAS (3. Semester)**

Inhalt :

- **Teamvorstellung in der PPT mit Namen, Bild, eMail-Adresse, Matrikelnummer und Projektrolle auf der ersten Folie**. Die Dozenten benötigen das um Sie auseinanderhalten und ggf. kontaktieren zu können.
- Vorstellung des Projektes (Master Usecase)
- Darstellung des Funktionsumfangs, Beschreibung der funktionalen und nichtfunktionalen Anforderungen sowie Entscheidung darüber, ob Mandatory oder Optional.
- Business Case (1 Folie)
- Erläutern Sie Ihre Vorgehensweise und verwendete Tools.
- Zeigen Sie, wie Sie modularisiert haben und wie der daraus abgeleitete Projektplan aussieht.
- Beschreiben Sie die Systemarchitektur und die Modularisierung (Top Down)
- Zeigen Sie wesentliche Lösungsansätze aus der SAS (zum Beispiel Paketformat, Anbindung an Java, ERD …).
- Bei Bedarf können Sie auch schon Prototypen vorstellen.

**Präsentation 2 - STP/STR/Produkt Präsentation/Selbstkritik (4. Semester)**

Beispielhafter Inhalt:

- Teamvorstellung in der PPT mit Namen, Bild, eMail-Adresse, Matrikelnummer und Projektrolle (erste Folie)
- Vorstellung des Projektes (Master Usecase)
- Produktübersicht (Black-Box)
- Architekturübersicht und Module (White-Box)
- Vorgehensweise beim Testen
- Live Demo
- Fazit / Ausblick

# **Dokumentation**

**Allgemeines**

- Für die meisten Dokumente erhalten Sie Word-Vorlagen in der NextCloud. Diese geben das allgemeine Gliederungsschema vor. Bei Verwendung eigener Vorlagen und Designs sollte aber die vorgegebene Gliederung weitgehend beibehalten werden.
- Diese Vorlagen sind sehr allgemein. Es kann also sein, dass Sie nicht zu allen Punkten, die erwähnt sind, etwas zu schreiben haben.
- Ausfüllhinweise im Dokument bei Finalisierung bitte löschen.
- Als Alternative zu Word-Dokumenten wird die Verwendung des Projektwiki des Repositories (GitHub) empfohlen. Diese Dokumente müssen dann zur Abgabe als PDF extrahiert und versioniert werden.
- Erlaubte Sprachen für die Projektdokumention sind Deutsch und Englisch, für produktbegleitende Dokumente (User Manual, Readme, SRS, SAS, STP) ist Englisch verpflichtend.

**Ablage der Dokumente**

Bitte verwenden Sie für die Abgaben und im Repository (GitHub) **IMMER** folgendes Ablageschema. Denken Sie an die Versionierung der Dateien. Die Dateinamen sollen wie folgt aufgebaut sein:

**TINF23F_CRS_Team_x_0v1**,

**TINF23F_MOD_Team_x_Modulname_0v1**

CRS, BC, SRS, SAS, MODs, STP, STR, Präsentationen und MeetingMinutes (bzw. Links auf deren Position im Wiki) hier ablegen (keine weiteren Unterverzeichnisse):

**Team_x_Projektname\\PROJECT\\**

Sourcecodedateien in den entsprechenden Unterstrukturen hier ablegen:

**Team_x_Projektname\\SOURCE\\MOD_y_Modulname**

Das entwickelte ausführbare Programm zusammen mit dem MANUAL hier ablegen:

**Team_x_Projektname\\EXECUTABLE\\**

Bei der Übermittlung der Projektdateien in einem ZIP-Archiv müssen die oben geforderten Verzeichnisstrukturen enthalten sein. In jeder Übermittlung müssen auch die vorherigen bereits übermittelten Dateien miteingepackt sein, d.h. es soll immer ein vollständiger Projektordner übermittelt werden. **Das gibt Ihnen auch die Chance, ggf. noch Korrekturen bei den bereits abgegeben Dateien einzubringen. In dem Fall immer die Versionsnummer des Dokuments hochzählen.**

Es sollen am Schluss alle Dokumente aus Semester 3 und 4 enthalten sein (die neuesten Versionen der Dokumente). Alle finalen Dokumente bitte als PDF UND im Originalformat (Word, MD oder HTML). Bitte KEINE getrennten Unterverzeichnisse für PDF und Originalformat.

**Einzelne Dokumente / Items**

| **CRS** |     |
| --- | --- |
| Zweck: | Beschreibt die Kundenwünsche an das Produkt |
| Umfang: | 5 -10 Seiten |
| Vorlage: | Ja  |
| Methoden: | Strukturierte Anforderung (Schablone), Fließtext, Skizzen der Oberfläche, Use Cases, Anwendungsfälle, Geschäftsvorfälle, … |
| Inhalt: | Siehe Vorlage |
|     |     |

<table><tbody><tr><th><p><strong>BC</strong></p></th><th></th></tr><tr><td><p>Zweck:</p></td><td><p>Kurze Betrachtung der wirtschaftlichen Aspekte des Projekts</p></td></tr><tr><td></td><td><p>Max. 4 Seiten</p></td></tr><tr><td><p>Vorlage:</p></td><td><p>Nein</p></td></tr><tr><td><p>Methoden:</p></td><td><p>Voll / Teilkosten Rechnung, Verfahren zur Risikoanalyse, ...</p></td></tr><tr><td><p>Inhalt:</p></td><td><p>Kostenrechnung:</p><ul><li>Fixe Kosten und Kosten für die einzelnen Arbeitspakete/Phasen.</li></ul><p>Rentabilitätsrechnung:</p><ul><li>Wie verdiene ich Geld damit?</li></ul><p>Erste grobe Projektplanung als GANTT-Diagramm</p><ul><li>Wie kann ich das Projekt abwickeln?</li></ul></td></tr><tr><td></td><td></td></tr><tr><td></td><td></td></tr></tbody></table>

| **SRS** |     |
| --- | --- |
| Zweck: | Beschreibt den Produktumfang und fixiert das Feature-Set aus Black-Box-Sicht. |
|     | 10 -15 Seiten |
| Vorlage: | Ja  |
| Methoden: | Trackbare strukturierte Anforderungen, klar formuliert (Schablone), Skizzen der Oberfläche, Prototypen, Use Cases mit Ablaufdiagrammen, … |
| Inhalt: | Siehe Vorlage |
|     |     |

| **SAS** |     |
| --- | --- |
| Zweck: | Beschreibt die konzeptionelle Lösung des Gesamtsystems (Grey-Box, White-Box) |
|     | 5 -15 Seiten |
| Vorlage: | Ja  |
| Methoden: | Architektur-, Komponenten-, Klassen-, Kommunikations-, Ablauf- und Sequenzdiagramme, ERM, Datenmodelle, … |
| Inhalt: | Siehe Vorlage |
|     |     |

| **STP** |     |
| --- | --- |
| Zweck: | Beschreibt die Systemtestfälle und die Testplanung für den Systemtest des Gesamtsystems (Black-Box) |
|     | 5 -15 Seiten, ca. 10 ausgearbeitete Testfälle |
| Vorlage: | Ja  |
| Methoden: | Anforderungsbasiertes Testen, Äquivalenzklassenbildung, Grenzwertanalyse, Exploratives Testen, Trennung von Testanweisungen und Testdaten. |
| Inhalt: | Siehe Vorlage |
|     |     |

| **MeetingMinutes** |     |
| --- | --- |
| Zweck: | Dokumentiert Ihre Projektaktivitäten |
| Umfang: | 10 - 15 Zeilen Status pro Sitzung<br><br>1 Sitzung pro Woche |
| Vorlage: | Nein |
| Methoden: | Fortlaufend ergänztes Dokument mit Inhaltsverzeichnis, für jede Sitzung ein Unterkapitel. |
| Inhalt: | Status der Arbeiten, Probleme, Beschlüsse |
| Hinweis: | Fortlaufende Protokolle als Kapitel in einer einzelnen Datei. |

| **PM Dokument** |     |
| --- | --- |
| Zweck: | Projektplanung |
| Umfang: | Max. 5 Seiten |
| Vorlage: | Nein, empfohlen wird „Projects“ im Github |
| Methoden: | Siehe PM VL |
| Inhalt: | GANTT, PSP |
|     |     |

# **FAQ**

**F: Woher kommen die Projektvorschläge?**

A: Die Projektvorschläge wurden von den Dozenten erstellt und sind meist in deren fachlicher Anwendungsdomäne angesiedelt. Das ermöglicht zusätzlichen Wissenstransfer im Rahmen der Projektarbeit.

**F: Was soll dieses Angebot mit dem Open-Source Projekt?**

A: Um die Wertigkeit der Projektarbeit für Sie zu steigern, wird angeregt, diese im Rahmen von Open-Source-Projekten abzuhandeln. Das hat folgende Vorteile:

- Die Studenten können später in Ihrem Lebenslauf auf Mitarbeit an einem veröffentlichten Open-Source-Projekt verweisen.
- Die Dozenten können die Software von nachfolgenden Studenten-Jahrgängen weiterentwickeln lassen (siehe rechtliche Hinweise weiter unten).

Beispiel:

<http://studium.dhbw-stuttgart.de/informatik/studierendenprojekte/multicastor/>

**F: Muss ich alle auch optionalen Features implementieren?**

A: Es besteht kein Zwang, alle optionalen Requirements zu implementieren, wenn die Aufwände zu groß werden. Die optionalen Features dienen als Manövriermasse für Projektrisiken in der Umsetzungsphase.

Sie sind angehalten, eine realistische Umfangsabschätzung der Projektaufgabe durchzuführen, die der eigenen Leistungsfähigkeit im zur Verfügung stehenden Zeitrahmen entspricht**. Entstehen muss am Ende ein funktionierendes und qualitativ überzeugendes sog. „Minimum Viable Product“ (MVP).** Features, die anfangs gemeinsam in der SRS als Mandatory vereinbart wurden, dürfen nicht ohne mit dem Auftraggeber (Dozenten) abgestimmte Begründung fehlen.

**Rechtliche Hinweise**

- Die erstellte Software ist ihr geistiges Eigentum. Sie haben das Vollkommene und alleinige Nutzungsrecht.
- Die Dozenten werden den Source-Code nicht ohne ihr Einverständnis weiterverwenden.
- Bei Veröffentlichung bzw. Offenlegung (z.B. als Open-Source-Projekt im GitHub-Repository) sind sie selbst für die Formulierung entsprechender Lizenzrechte verantwortlich. Es wird die Verwendung der MIT-Lizenz empfohlen.

# **TINF23F Teilnehmerübersicht**

|     | **Nachname** | **Vorname** | **DH Mail** | **Matrikel-Nr.** | **Firma** |
| --- | --- | --- | --- | --- | --- |
| 1   |     |     |     |     |     |
| 2   |     |     |     |     |     |
| 3   |     |     |     |     |     |
| 4   |     |     |     |     |     |
| ~~5~~ |     |     |     |     |     |
| 6   |     |     |     |     |     |
| 7   |     |     |     |     |     |
| 8   |     |     |     |     |     |
| 9   |     |     |     |     |     |
| 10  |     |     |     |     |     |
| ~~11~~ |     |     |     |     |     |
| 12  |     |     |     |     |     |
| 13  |     |     |     |     |     |
| 14  |     |     |     |     |     |
| 15  |     |     |     |     |     |
| 16  |     |     |     |     |     |
| 17  |     |     |     |     |     |
| 18  |     |     |     |     |     |
| 19  |     |     |     |     |     |
| 20  |     |     |     |     |     |
| 21  |     |     |     |     |     |
| 22  |     |     |     |     |     |
| 23  |     |     |     |     |     |
| 24  |     |     |     |     |     |
| 25  |     |     |     |     |     |
| 26  |     |     |     |     |     |

Sammel-eMail: [stud-verteiler+STG-TINF23F@lehre.dhbw-stuttgart.de](mailto:stud-verteiler+STG-TINF22F@lehre.dhbw-stuttgart.de)

Kurssprecher/in: MobilNr:

NextCloud-Ablage:

GitHub-Repository-Organizer:

# **Projektthemen**

Es werden Projektthemen mit ähnlichem Schwierigkeitsgrad für 4 Teams angeboten. Bei Unstimmigkeiten unter den Teams, wer welches Projekt machen möchte, treffen die Dozenten die finale Zuweisung. Folgende Themen werden bearbeitet:

Team 1**:  Mnestix Webclient**

| **Rolle** | **Name** | **Nachname** | **eMail** | **Matrikel** |
| --- | --- | --- | --- | --- |
| Projektleiter |     |     |     |     |
| Produktmanager |     |     |     |     |
| Testmanager |     |     |     |     |
| Systemarchitekt |     |     |     |     |
| Dokumentation |     |     |     |     |
| Entwickler |     |     |     |     |

GIT-Repository:  <https://github.com/DHBW-TINF23F/Team1-Mnestix-WebClient>

Team 2**:  BaSyx Webclient**

| **Rolle** | **Name** |     | **eMail** | **Matrikel** |
| --- | --- | --- | --- | --- |
| Projektleiter |     |     |     |     |
| Produktmanager |     |     |     |     |
| Testmanager |     |     |     |     |
| Systemarchitekt |     |     |     |     |
| Dokumentation |     |     |     |     |
| Entwickler |     |     |     |     |

GIT-Repository:  <https://github.com/DHBW-TINF23F/Team2-BaSyx-WebClient>

Team 3**:  BaSyx Editor Plugin**

| **Rolle** | **Name** |     | **eMail** | **Matrikel** |
| --- | --- | --- | --- | --- |
| Projektleiter |     |     |     |     |
| Produktmanager |     |     |     |     |
| Testmanager |     |     |     |     |
| Systemarchitekt |     |     |     |     |
| Dokumentation |     |     |     |     |
| Entwickler |     |     |     |     |

GIT-Repository:  <https://github.com/DHBW-TINF23F/Team3-BaSyx-Editor-Plugin>

Team 4:  **BaSyx Security Plugin**

| **Rolle** |     | **Name** | **eMail** | **Matrikel** |
| --- | --- | --- | --- | --- |
| Projektleiter |     |     |     |     |
| Produktmanager |     |     |     |     |
| Testmanager |     |     |     |     |
| Systemarchitekt |     |     |     |     |
| Dokumentation |     |     |     |     |
| Entwickler |     |     |     |     |

GIT-Repository: <https://github.com/DHBW-TINF23F/Team4-BaSyx-Security-Plugin>

## **Mnestix Webclient**

Die sog. „Verwaltungsschale“ ([Asset Administration Shell](https://www.plattform-i40.de/IP/Redaktion/DE/Downloads/Publikation/Details_of_the_Asset_Administration_Shell_Part1_V3.html)) ist der Standard der Industrie 4.0 für die Modellierung von digitalen Abbildern (sog. „digitalen Zwillingen“) von Gegenständen wie bspw. Automatisierungsgeräten, -systemen und zu fertigenden Produkten. Von der [IDTA](https://industrialdigitaltwin.org/content-hub/downloads) bereitgestellte Tools wie der AASX Explorer \[3\] dienen zum Erzeugen von dateibasierten Verwaltungsschalen (Typ 1) und sog. reaktive Verwaltungsschalen (Typ 2) können über eine standardisierte REST-API durch sog. AAS Server im Netzwerk bereitgestellt werden. Es existieren Web-Frontends zur Visualisierung, wobei diese eher technisch orientiert und nicht wirklich userfreundlich gestaltet sind.

![Ein Bild, das Text, Screenshot, Webseite, Software enthält.

Im Rahmen der Aufgabe soll das Open-Source-Projekt [Mnestix](https://github.com/mnestix/mnestix-browser) weiterentwickelt und insbesondere die Viewer-Usability für die einzelnen [IDTA-Submodelle](https://industrialdigitaltwin.org/en/content-hub/downloads).

Betrachtet werden sollen vor allem die Submodelle „**Digital Nameplate**“, „**Technical Data**“, „**Hierarchical Structures enabling Bills of Material**“ \[4\], „**BillofProcesses**“**, „ServiceRequestNotification“.** Der [Nameplate-Generator](https://github.com/TTRSF/TINF22F-Nameplate-Generator) soll in die Anzeige des „Digital Nameplate“ integriert werden.

Folgende Teilaufgaben müssen im Wesentlichen bearbeitet werden:

1. Einarbeitung in das Thema AAS und Mnestix. Dazu den [AASX-Explorer](https://github.com/eclipse-aaspe/package-explorer/releases) installieren und ein [Mnestix-Frontend](https://github.com/mnestix/mnestix-browser) mit [BaySyx-Infrastruktur](https://basyx.org/get-started/introduction) aufsetzen. Hierzu die vorhandenen Tutorials anwenden, bewerten und identifizierte Lücken verbessern.
2. Analyse der „Concept Description“ (Asset-Reference).
3. Analyse (auch im Vergleich mit anderen AAS-UIs) und Definition eines verbesserten Usability-Konzeptes für die Anzeige von Submodellen im [Mnestix-UI](https://wiki.basyx.org/en/latest/content/user_documentation/basyx_components/web_ui/index.html)
4. Forken des [Mnestix-Repositories](https://github.com/mnestix/mnestix-browser), Änderungen vornehmen, Build-Prozess anstossen, Änderungen sichtbar?
5. Umsetzung der Usability-Verbesserungen, Integration der Funktion „Nameplate-Generator“.
6. Akzeptanzfindung: Die erstellten Lösungen in den Mainstream des Mnestix-Projekts einbringen.
7. Test der Applikation gegen eine diverse AAS-Server-Infrastruktur.

## **BaSyx Webclient**

Die sog. „Verwaltungsschale“ ([Asset Administration Shell](https://www.plattform-i40.de/IP/Redaktion/DE/Downloads/Publikation/Details_of_the_Asset_Administration_Shell_Part1_V3.html)) ist der Standard der Industrie 4.0 für die Modellierung von digitalen Abbildern (sog. „digitalen Zwillingen“) von Gegenständen wie bspw. Automatisierungsgeräten, -systemen und zu fertigenden Produkten. Von der [IDTA](https://industrialdigitaltwin.org/content-hub/downloads) bereitgestellte Tools wie der AASX Explorer dienen zum Erzeugen von dateibasierten Verwaltungsschalen (Typ 1) und sog. reaktive Verwaltungsschalen (Typ 2) können über eine standardisierte REST-API durch sog. AAS Server im Netzwerk bereitgestellt werden. Es existieren Web-Frontends zur Visualisierung, wobei diese eher technisch orientiert und nicht wirklich userfreundlich gestaltet sind.

Im Rahmen der Aufgabe soll das Open-Source-Projekt [BaSyx](https://github.com/eclipse-basyx/basyx-aas-web-ui) weiterentwickelt und insbesondere die Usability verbessert werden. Betrachtet werden sollen vor allem die [Submodelle](https://github.com/admin-shell-io/submodel-templates/tree/main/published) „**Digital Nameplate**“, „**Technical Data**“, „**Hierarchical Structures enabling Bills of Material**“, „**Bill of Process**“**, „ServiceRequestNotification“.** Der [Nameplate-Generator](https://github.com/TTRSF/TINF22F-Nameplate-Generator) soll in das [Submodel-Plugin](https://github.com/eclipse-basyx/basyx-aas-web-ui/tree/main/aas-web-ui/src/components/SubmodelPlugins) „Digital Nameplate“ integriert werden. Das Submodel-Plugin [„Bills of Material“](https://github.com/eclipse-basyx/basyx-aas-web-ui/blob/main/aas-web-ui/src/components/SubmodelPlugins/BillsOfMaterial.vue) soll weiterentwickelt werden, um Catena-X-konforme BOMs (Aspect Model „SingleLevelBomAsPlanned/Built“) zu unterstützen.

Folgende Teilaufgaben müssen im Wesentlichen bearbeitet werden:

1. Einarbeitung: Den [AASX-Explorer](https://github.com/eclipse-aaspe/package-explorer/releases) installieren und eine BaySyx-Infrastruktur [aufsetzen](https://basyx.org/get-started/introduction). Hierzu die vorhandenen Tutorials anwenden, bewerten und identifizierte Lücken in den Tutorials verbessern.
2. Analyse (auch im Vergleich mit anderen AAS-UIs) und Definition eines verbesserten Usability-Konzeptes für das [BaSyx-UI](https://wiki.basyx.org/en/latest/content/user_documentation/basyx_components/web_ui/index.html).
3. Generelle Analyse der Usability des Frontend, Erarbeitung von Verbesserungsvorschlägen.
4. Definition eines Editor-Modus vs. Viewer-Modus für jedes Submodell mit Reduktion der dargestellten Informationen im „Viewer“-Modus auf das Wesentliche, bspw. Ausblenden der zu technischen Strukturinformationen.
5. Integration der Funktion „Nameplate-Generator“ in BaSyx.
6. Implementierung der Submodell-Plugins.
7. Akzeptanzfindung: Die erstellten Lösungen in den Mainstream des BaSyx-Projekts einbringen.
8. Test der Applikation gegen eine diverse AAS-Server-Infrastruktur.

## **BaSyx Editor-Plugin**

Das BaSyx-Ökosystem kann derzeit keine neue Verwaltungsschale erzeugen oder Teilmodelle in einer Verwaltungsschale hinzufügen. Hierzu gibt es bereits [Anforderungen im Ticket-System](https://github.com/eclipse-basyx/basyx-applications/issues/240) des [BaSyx-GUI-Projekts](https://github.com/eclipse-basyx/basyx-applications/tree/main/aas-gui), welche als Anforderungsgrundlage verwendet werden sollen.

Für das vorliegende Projekt soll für das BaSyx-UI das AAS-Editor-Plugin erweitert werden. Im Plugin sollen folgende Anwendungsfälle unterstützt werden:

1. Ein Bild, das Text, Screenshot, Schrift enthält. 
2. Submodell zu AAS hinzufügen.
3. Der Submodell-Baum soll angezeigt werden können. Inhaltlich noch nicht vollständig befüllte Submodelle oder Attribute sollen optisch hervorgehoben werden (z.B. rot markiert).
4. Externe Modell-Dateien sollen zur AAS hinzugefügt werden können. Nach einer Plausibilitätsprüfung soll eine [definitionsgemäße Verlinkung](C://Users/Markus%20Rentschler/Downloads/IDTA_02026-1-0_Submodel_ProvisionOf3DModels.pdf) mit MimeType der ausgewählten Datei in der Verwaltungsschale erfolgen.
5. Beim Laden einer KBL- oder VEC-Datei soll diese inhaltlich analysiert und die Nameplate-Informationen sowie relevante Technischen Daten (z.B. Gewicht, Features des Leitungssatzes) extrahiert und in ein AAS-Submodel „[General Technical Data](https://github.com/admin-shell-io/submodel-templates/tree/main/published/Technical_Data/1/2)“ überführt werden können.
6. Komponenten-Stammdaten von einem Zulieferer sollen als AAS-Typ1 (AASX-Datei) oder als AAS-Typ2 über das Netzwerk importiert werden können.
7. Attribute in Submodellen sollen editierbar sein.

Folgende Teilaufgaben müssen im Wesentlichen bearbeitet werden:

1. Einarbeitung: Den [AASX-Explorer](https://github.com/eclipse-aaspe/package-explorer/releases) installieren und eine BaySyx-Infrastruktur [aufsetzen](https://basyx.org/get-started/introduction). Hierzu die vorhandenen Tutorials anwenden, bewerten und identifizierte Lücken in den Tutorials verbessern.
2. Forken der benötigten [Basyx-Repositories](https://github.com/eclipse-basyx/basyx-aas-web-ui).
3. Lokale Buildchain einrichten und beherrschen lernen: Änderungen vornehmen, Build-Prozess anstossen, sind die Änderungen sichtbar im lokalen Livesystem?
4. Analyse des [BaSyx-UIs](https://wiki.basyx.org/en/latest/content/user_documentation/basyx_components/web_ui/index.html), Definition eines Usability-Konzeptes und Workflows für die Editor-Anwendungsfälle.
5. Implementierung und Test der Funktionalitäten
6. Erstellung und Verlinkung einer strukturierten Online-Benutzerdokumentation (z.B. mit [ReadTheDocs](https://app.readthedocs.org/))
7. Hosting der Funktionalität
8. Akzeptanzfindung für die erstellte Lösung im Open-Source-Projekt herbeiführen

## **BaSyx Security-Plugin**

Folgende Dokumente definieren bislang das Thema „Security für Verwaltungsschalen“:

- [Security der Verwaltungsschale](https://www.plattform-i40.de/PI40/Redaktion/DE/Downloads/Publikation/security-der-verwaltungsschale.html) (02/2018)
- [Zugriffssteuerung für Industrie 4.0-Komponenten zur Anwendung von Herstellern, Betreibern und Integratoren](https://www.plattform-i40.de/PI40/Redaktion/DE/Downloads/Publikation/zugriffssteuerung-industrie40-komponenten.html) (12/2018)
- [Sicherer Downloadservice](https://www.plattform-i40.de/PI40/Redaktion/EN/Downloads/Publikation/secure_downloadservice.html) (12/2020)
- [Details of the Asset Administration Shell Part 1, Chapter 6, ABAC & RBAC](https://www.plattform-i40.de/PI40/Redaktion/DE/Downloads/Publikation/Details_of_the_Asset_Administration_Shell_Part1_V3.html) (05/2022)

In der IDTA wird derzeit an der Spezifikation „Security“ gearbeitet, wobei zunächst das rollenbasierte Modell aus „[Details of the Administration Shell](https://admin-shell-io.github.io/aas-specs-antora/IDTA-01003-a/v3.0/index.html)“ übernommen wurde, dass bis V30RC02 dort enthalten war und auf dem Konzept der „Attribute-Based Access Control“ (ABAC) basiert. Es existiert auch eine prototypische AAS-Server-Implementierung (<https://v3.admin-shell-io.com/>), siehe Abbildung, jedoch keine Benutzeroberfläche, um Zugriffsrichtlinien für AAS-Elemente zu konfigurieren.

![Ein Bild, das Text, Screenshot, Software, Computersymbol enthält.

Derzeit werden in der IDTA-Arbeitsgruppe vier Varianten diskutiert:

1. Security Meta Model
2. Security Submodel
3. External Model XACL
4. External Model ODRL, basierend auf Mechanismen, die auch CATENA-X nutzt.

Eine erste Version der neuen Security-Spezifikation wird für Sept./Oktober 2024 erwartet.

Im Gegensatz dazu ist derzeit ist in BaSyx nur eine einfache rollenbasierte Zugriffskontrolle (Role Based Access Control = RBAC) implementiert. Jeder Service (AAS Discovery, AAS-Environment, AAS Concept Description etc.) benötigt eine eigene Konfigurationsdatei, welche in JSON-Format die Rollen und Rechte spezifisch für bestimmte AAS mit IDs oder Wildcards beschreibt. Hierfür gibt es ein dediziertes [Konfigurationsdateiformat](https://wiki.basyx.org/en/latest/content/user_documentation/basyx_components/v2/aas_discovery/features/authorization.html#rbac-rule-configuration) sowie ein SDK-Beispiel namens „[BaSyxSecured](https://github.com/eclipse-basyx/basyx-java-server-sdk/tree/main/examples/BaSyxSecured)“, welches den Authorisierungs-Server [Keycloak](https://www.keycloak.org/docs/latest/server_admin/index.html) verwendet.

Es soll daher für das BaSyx-UI ein neues [Plugin](https://wiki.basyx.org/en/latest/content/user_documentation/basyx_components/web_ui/features/plugin_mechanism.html) „Security“ entwickelt werden, welches folgende Anwendungsfälle mit einer guten Benutzbarkeit unterstützt:

1. Rollen verwalten und konfigurieren.
2. Rechtezuweisungen auf AAS-, Submodell- und Attributebene (ABAC) konfigurieren.
3. Identitäten verwalten und zu Rollen zuordnen
4. Import/Export von Zugangsrichtlinien für den externen Authorisierungs-Server [Keycloak](https://www.keycloak.org/docs/latest/server_admin/index.html)

Es wird dabei von folgenden Annahmen ausgegangen:

1. Die Zugangsrichtlinien (Policies) werden vom AAS-Verantwortlichen eingerichtet
2. Ein (externer) Benutzer möchte auf eine AAS zugreifen
3. Das Identitätsmanagement wird von einem Identitätsanbieter (IdP) durchgeführt. Der IdP stellt ein Access Token zur Verfügung, das für den AAS-Server relevante Angaben enthält. Das Token (JWT, JSON Web Token) wird vom IdP signiert.
4. Der AAS-Server vertraut dem Identity Provider
5. Der Zugang zur AAS wird auf der Grundlage des Access Token und der Zugangsrichtlinien gewährt

Im Kern müssen zu dem Thema AAS-Security folgende Fragestellungen geklärt werden:

- Wo sollen die Zugangsrichtlinien (Policies) gespeichert werden?
  - Innerhalb der AAS selbst?
  - In einem separaten Policy-Repository?
- Wie können die Zugangsrichtlinien abgebildet werden?
  - Mit AAS-Elementen?
  - Mit bestehenden Sprachen wie [XACML](https://en.wikipedia.org/wiki/XACML) oder [ODRL](https://en.wikipedia.org/wiki/ODRL)?
- Wie wird die Zugangsrichtlinien-Entscheidung implementiert?
  - Mit einem Interpreter, der zum Zeitpunkt der Zugriffsentscheidung aufgerufen wird?
  - Integriert in Such- und Abfragestrukturen?

![Ein Bild, das Text, Screenshot, Software, Webseite enthält.

Folgende Teilaufgaben müssen im Wesentlichen bearbeitet werden:

1. Einarbeitung in [Keycloak](https://www.keycloak.org/), [XACML](https://en.wikipedia.org/wiki/XACML), [ODRL](https://en.wikipedia.org/wiki/ODRL).
2. Einarbeitung in [BaSyx](https://eclipse.dev/basyx). Dazu eine BaySyx-Infrastruktur [aufsetzen](https://basyx.org/get-started/introduction). Die vorhandenen Tutorials anwenden, qualitativ bewerten und identifizierte Lücken in den Tutorials verbessern.
3. Forken der benötigten [Basyx-Repositories](https://github.com/eclipse-basyx/basyx-applications/tree/main/aas-gui).
4. Lokale Buildchain einrichten und beherrschen lernen: Änderungen vornehmen, Build-Prozess anstossen, sind die Änderungen sichtbar im lokalen Livesystem?
5. Analyse des [BaSyx-UIs](https://wiki.basyx.org/en/latest/content/user_documentation/basyx_components/web_ui/index.html), Definition eines Usability-Konzeptes und Workflows für die Security-Anwendungsfälle.
6. Implementierung und Test der Plugin-Funktionalitäten (Benutzeroberflächen, Import/Export der Policy-Dateien)
7. Erstellung und Verlinkung einer strukturierten Online-Benutzerdokumentation (z.B. mit [ReadTheDocs](https://app.readthedocs.org/))
8. Hosting der Funktionalität
9. Akzeptanzfindung für die erstellte Lösung im Open-Source-Projekt herbeiführen
