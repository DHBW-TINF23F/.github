## Projekt 4: **Mnestix Webclient**

Die sog. „Verwaltungsschale“ ([Asset Administration Shell](https://www.plattform-i40.de/IP/Redaktion/DE/Downloads/Publikation/Details_of_the_Asset_Administration_Shell_Part1_V3.html)) ist der Standard der Industrie 4.0 für die Modellierung von digitalen Abbildern (sog. „digitalen Zwillingen“) von Gegenständen wie bspw. Automatisierungsgeräten, -systemen und zu fertigenden Produkten. Von der [IDTA](https://industrialdigitaltwin.org/content-hub/downloads) bereitgestellte Tools wie der AASX Explorer \[3\] dienen zum Erzeugen von dateibasierten Verwaltungsschalen (Typ 1) und sog. reaktive Verwaltungsschalen (Typ 2) können über eine standardisierte REST-API durch sog. AAS Server im Netzwerk bereitgestellt werden. Es existieren Web-Frontends zur Visualisierung, wobei diese eher technisch orientiert und nicht wirklich userfreundlich gestaltet sind.

![image](https://github.com/user-attachments/assets/99e5aab6-019f-4977-8b44-f53fdb0b71e5)

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
