## Projekt 2: **BaSyx Webclient**

Die sog. „Verwaltungsschale“ ([Asset Administration Shell](https://www.plattform-i40.de/IP/Redaktion/DE/Downloads/Publikation/Details_of_the_Asset_Administration_Shell_Part1_V3.html)) ist der Standard der Industrie 4.0 für die Modellierung von digitalen Abbildern (sog. „digitalen Zwillingen“) von Gegenständen wie bspw. Automatisierungsgeräten, -systemen und zu fertigenden Produkten. Von der [IDTA](https://industrialdigitaltwin.org/content-hub/downloads) bereitgestellte Tools wie der AASX Explorer dienen zum Erzeugen von dateibasierten Verwaltungsschalen (Typ 1) und sog. reaktive Verwaltungsschalen (Typ 2) können über eine standardisierte REST-API durch sog. AAS Server im Netzwerk bereitgestellt werden. Es existieren Web-Frontends zur Visualisierung, wobei diese eher technisch orientiert und nicht wirklich userfreundlich gestaltet sind.

![image](https://github.com/user-attachments/assets/96525a7c-1fe8-4aff-9fed-9e92f22dfed6)

Im Rahmen der Aufgabe soll das Open-Source-Projekt [BaSyx](https://github.com/eclipse-basyx/basyx-aas-web-ui) weiterentwickelt und insbesondere die Usability verbessert werden. Betrachtet werden sollen vor allem die [Submodelle](https://github.com/admin-shell-io/submodel-templates/tree/main/published) „**Digital Nameplate**“, „**Technical Data**“, „**Hierarchical Structures enabling Bills of Material**“, „**Bill of Process**“**, „ServiceRequestNotification“.** Der [Nameplate-Generator](https://github.com/TTRSF/TINF22F-Nameplate-Generator) soll in das [Submodel-Plugin](https://github.com/eclipse-basyx/basyx-aas-web-ui/tree/main/aas-web-ui/src/components/SubmodelPlugins) „Digital Nameplate“ integriert werden. Das Submodel-Plugin [„Bills of Material“](https://github.com/eclipse-basyx/basyx-aas-web-ui/blob/main/aas-web-ui/src/components/SubmodelPlugins/BillsOfMaterial.vue) soll weiterentwickelt werden, um Catena-X-konforme BOMs (Aspect Model „SingleLevelBomAsPlanned/Built“) zu unterstützen.

**Folgende Teilaufgaben müssen im Wesentlichen bearbeitet werden:**

1. Einarbeitung: Den [AASX-Explorer](https://github.com/eclipse-aaspe/package-explorer/releases) installieren und eine BaySyx-Infrastruktur [aufsetzen](https://basyx.org/get-started/introduction). Hierzu die vorhandenen Tutorials anwenden, bewerten und identifizierte Lücken in den Tutorials verbessern.
2. Analyse (auch im Vergleich mit anderen AAS-UIs) und Definition eines verbesserten Usability-Konzeptes für das [BaSyx-UI](https://wiki.basyx.org/en/latest/content/user_documentation/basyx_components/web_ui/index.html).
3. Generelle Analyse der Usability des Frontend, Erarbeitung von Verbesserungsvorschlägen.
4. Definition eines Editor-Modus vs. Viewer-Modus für jedes Submodell mit Reduktion der dargestellten Informationen im „Viewer“-Modus auf das Wesentliche, bspw. Ausblenden der zu technischen Strukturinformationen.
5. Integration der Funktion „Nameplate-Generator“ in BaSyx.
6. Implementierung der Submodell-Plugins.
7. Akzeptanzfindung: Die erstellten Lösungen in den Mainstream des BaSyx-Projekts einbringen.
8. Test der Applikation gegen eine diverse AAS-Server-Infrastruktur.
