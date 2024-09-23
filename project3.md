## Projekt 3: **BaSyx Editor-Plugin**

Das BaSyx-Ökosystem kann derzeit keine neue Verwaltungsschale erzeugen oder Teilmodelle in einer Verwaltungsschale hinzufügen. Hierzu gibt es bereits [Anforderungen im Ticket-System](https://github.com/eclipse-basyx/basyx-applications/issues/240) des [BaSyx-GUI-Projekts](https://github.com/eclipse-basyx/basyx-applications/tree/main/aas-gui), welche als Anforderungsgrundlage verwendet werden sollen. Das Projekt [AAS-Manager](https://github.com/rwth-iat/aas_manager) ist ebenfalls in Betracht zu ziehen.

![image](https://github.com/user-attachments/assets/34d6e4bf-d1eb-443f-98cb-9d3f75068bf2)

Für das vorliegende Projekt soll für das BaSyx-UI das AAS-Editor-Plugin erweitert werden. Im Plugin sollen folgende Anwendungsfälle unterstützt werden:

![image](https://github.com/user-attachments/assets/34d49de1-2085-4f38-bab5-d259854c344c)

1. AAS erzeugen: Die AAS-Zusammenstellung soll auswählbar sein. Die Optionen betreffen im wesentliche die Zusammenstellung der Teilmodelle, die die AAS mindestens enthalten soll. Zur Auswahl bereitstehende vordefinierte Zusammenstellungen (z.B. LS-AAS) sollen nicht hartcodiert, sondern in einer JSON-Konfigurationsdatei zum Plugin hinterlegt werden. 
2. Submodell zu AAS hinzufügen.
3. Der Submodell-Baum soll angezeigt werden können. Inhaltlich noch nicht vollständig befüllte Submodelle oder Attribute sollen optisch hervorgehoben werden (z.B. rot markiert).
4. Externe Modell-Dateien sollen zur AAS hinzugefügt werden können. Nach einer Plausibilitätsprüfung soll eine [definitionsgemäße Verlinkung](C://Users/Markus%20Rentschler/Downloads/IDTA_02026-1-0_Submodel_ProvisionOf3DModels.pdf) mit MimeType der ausgewählten Datei in der Verwaltungsschale erfolgen.
5. Beim Laden einer KBL- oder VEC-Datei soll diese inhaltlich analysiert und die Nameplate-Informationen sowie relevante Technischen Daten (z.B. Gewicht, Features des Leitungssatzes) extrahiert und in ein AAS-Submodel „[General Technical Data](https://github.com/admin-shell-io/submodel-templates/tree/main/published/Technical_Data/1/2)“ überführt werden können.
6. Komponenten-Stammdaten von einem Zulieferer sollen als AAS-Typ1 (AASX-Datei) oder als AAS-Typ2 über das Netzwerk importiert werden können.
7. Attribute in Submodellen sollen editierbar sein.

**Folgende Teilaufgaben müssen im Wesentlichen bearbeitet werden:**

1. Einarbeitung: Den [AASX-Explorer](https://github.com/eclipse-aaspe/package-explorer/releases) installieren und eine BaySyx-Infrastruktur [aufsetzen](https://basyx.org/get-started/introduction). Hierzu die vorhandenen Tutorials anwenden, bewerten und identifizierte Lücken in den Tutorials verbessern.
2. Forken der benötigten [Basyx-Repositories](https://github.com/eclipse-basyx/basyx-aas-web-ui).
3. Lokale Buildchain einrichten und beherrschen lernen: Änderungen vornehmen, Build-Prozess anstossen, sind die Änderungen sichtbar im lokalen Livesystem?
4. Analyse des [BaSyx-UIs](https://wiki.basyx.org/en/latest/content/user_documentation/basyx_components/web_ui/index.html), Definition eines Usability-Konzeptes und Workflows für die Editor-Anwendungsfälle.
5. Implementierung und Test der Funktionalitäten
6. Erstellung und Verlinkung einer strukturierten Online-Benutzerdokumentation (z.B. mit [ReadTheDocs](https://app.readthedocs.org/))
7. Hosting der Funktionalität
8. Akzeptanzfindung für die erstellte Lösung im Open-Source-Projekt herbeiführen
