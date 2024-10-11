## Projekt 1: **BaSyx Security-Plugin**

Folgende Dokumente definieren bislang das Thema „Security für Verwaltungsschalen“:

- [Security der Verwaltungsschale](https://www.plattform-i40.de/PI40/Redaktion/DE/Downloads/Publikation/security-der-verwaltungsschale.html) (02/2018)
- [Zugriffssteuerung für Industrie 4.0-Komponenten zur Anwendung von Herstellern, Betreibern und Integratoren](https://www.plattform-i40.de/PI40/Redaktion/DE/Downloads/Publikation/zugriffssteuerung-industrie40-komponenten.html) (12/2018)
- [Sicherer Downloadservice](https://www.plattform-i40.de/PI40/Redaktion/EN/Downloads/Publikation/secure_downloadservice.html) (12/2020)
- [Details of the Asset Administration Shell Part 1, Chapter 6, ABAC & RBAC](https://www.plattform-i40.de/PI40/Redaktion/DE/Downloads/Publikation/Details_of_the_Asset_Administration_Shell_Part1_V3.html) (05/2022)

In „[Details of the Administration Shell](https://admin-shell-io.github.io/aas-specs-antora/IDTA-01003-a/v3.0/index.html)“ war bis V30RC02 ein Security-Konzept für sowohl RBAC als auch ABAC enthalten. Hierfür exisitert auch eine prototypische AAS-Server-Implementierung (https://v3.admin-shell-io.com/), siehe Abbildung 18,  jedoch keine Benutzeroberfläche, um Zugriffsrichtlinien für AAS-Elemente zu konfigurieren.

![image](https://github.com/user-attachments/assets/4eee8263-d331-442b-b0d3-95a7a1e74f57)

Derzeit wird das AAS-Security-Konzept in der IDTA komplett überarbeitet und soll durch eine neue Spezifikation „Security“ ersetzt werden. Hierfür werden in der IDTA-Arbeitsgruppe vier Varianten diskutiert:

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

![image](https://github.com/user-attachments/assets/96419526-2e05-47d6-9083-47ed9e4c08a9)

**Folgende Teilaufgaben müssen im Wesentlichen bearbeitet werden:**

1. Einarbeitung in [Keycloak](https://www.keycloak.org/), [XACML](https://en.wikipedia.org/wiki/XACML), [ODRL](https://en.wikipedia.org/wiki/ODRL).
2. Einarbeitung in [BaSyx](https://eclipse.dev/basyx). Dazu eine BaySyx-Infrastruktur [aufsetzen](https://basyx.org/get-started/introduction). Die vorhandenen Tutorials anwenden, qualitativ bewerten und identifizierte Lücken in den Tutorials verbessern.
3. Forken der benötigten [Basyx-Repositories](https://github.com/eclipse-basyx/basyx-applications/tree/main/aas-gui).
4. Lokale Buildchain einrichten und beherrschen lernen: Änderungen vornehmen, Build-Prozess anstossen, sind die Änderungen sichtbar im lokalen Livesystem?
5. Analyse des [BaSyx-UIs](https://wiki.basyx.org/en/latest/content/user_documentation/basyx_components/web_ui/index.html), Definition eines Usability-Konzeptes und Workflows für die Security-Anwendungsfälle.
6. Implementierung und Test der Plugin-Funktionalitäten (Benutzeroberflächen, Import/Export der Policy-Dateien)
7. Erstellung und Verlinkung einer strukturierten Online-Benutzerdokumentation (z.B. mit [ReadTheDocs](https://app.readthedocs.org/))
8. Hosting der Funktionalität
9. Akzeptanzfindung für die erstellte Lösung im Open-Source-Projekt herbeiführen
