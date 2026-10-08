# Robotisches Haareschneiden

Sprachen: [English](../README.md) | [中文](README.zh.md) | [Suomi](README.fi.md) | Deutsch | [Français](README.fr.md)

Dieses Repository bietet einen enzyklopädischen Überblick über robotisches Haareschneiden. Es behandelt Hintergrund, Geschichte, Sicherheitsaspekte, Anwendungen, technische Herausforderungen und zentrale Referenzen. Relevante Veröffentlichungen werden im Text zitiert und am Ende dieses Dokuments gesammelt. Eine allgemeine Einführung in das Projekt ist außerdem in den [Haircutting Robot Introduction Slides](../haircutting_robot_introduction.pdf) verfügbar, die Motivation, bisherige Forschung, technische Anforderungen, Sicherheit, unterstützende Technologien und den Ausblick behandeln.

## Überblick

Robotisches Haareschneiden bezeichnet den Einsatz robotischer Systeme zur Unterstützung oder Ausführung von Haarschneideaufgaben. Dazu gehören Trimmen, Rasieren, Frisieren und weitere verwandte Pflegeaufgaben. Robotische Plattformen, die für diese Aufgaben entwickelt wurden, werden üblicherweise als Haarschneide-Roboter bezeichnet.

Das Gebiet liegt an der Schnittstelle von Robotik, Computer Vision, Bewegungsplanung, Manipulation, Mensch-Roboter-Interaktion, Kommunikation, Computergrafik, virtueller Realität, künstlicher Intelligenz und Haptik.

Im Gegensatz zu gewöhnlichen elektrischen Haarschneidemaschinen oder manuell geführten Pflegewerkzeugen benötigen robotische Haarschneidesysteme Wahrnehmungs-, Planungs- und Regelungsfähigkeiten, damit ein Roboter ein Schneide- oder Pflegewerkzeug relativ zu Kopf und Haar positionieren kann. Das ist technisch anspruchsvoll, weil Haare deformierbar sind, zwischen Personen stark variieren und in der Nähe empfindlicher anatomischer Bereiche wie Ohren, Augen, Kopfhaut und Gesicht bearbeitet werden.

Die heute diskutierten Systeme reichen von teleoperierten Plattformen bis zu autonomeren Konzepten. In der hier gesammelten Literatur von 2025 wird kein vollständig kommerzieller Haarschneide-Roboter als breit eingesetzt beschrieben, doch Forschungsprototypen und Überblicksarbeiten deuten auf einen plausiblen Weg zur Kommerzialisierung hin.

## Geschichte

### Frühe automatische Haarschneidegeräte

Ideen zum automatischen Haareschneiden entstanden lange vor modernen robotischen Systemen. Ein US-Patent von [Jean Gronier](#ref-gronier-1966) aus dem Jahr 1966 beschrieb eine automatische Haarschneidemaschine, die mithilfe programmierter Steuerung eine vorgegebene Frisur erzeugen sollte. Es lässt sich besser als vorrobotische Automatisierung denn als modernes robotisches Haarschneidesystem verstehen, da es auf mechanischer Struktur und vorgegebenen Programmen beruhte und nicht auf Echtzeitwahrnehmung oder adaptivem Feedback.

Spätere Patente schlugen integriertere Systeme vor, die Wahrnehmung, robotische Mechanismen und Benutzerschnittstellen kombinierten. Das spiegelt einen Übergang zu deutlicher robotisch geprägten Umsetzungen wider, darunter auch das spätere Patent von [Mubarak Aldabbah](#ref-aldabbah-2023).

### Kameragestützte Selbsthaarschnitt-Systeme

Eine verwandte Forschungslinie konzentrierte sich darauf, Menschen beim eigenen Haareschneiden zu unterstützen, anstatt den Schnitt autonom durch einen Roboter ausführen zu lassen. 2014 stellten [Futami, Terada und Tsukamoto](#ref-futami-2014) ein robotisches System mit beweglicher Kamera vor, das Nutzern während des Selbsthaarschnitts unterschiedliche Blickwinkel auf den eigenen Kopf ermöglichte.

### Robotische Haarschneide-Prototypen

In den 2020er Jahren lenkten mehrere öffentliche Demonstrationen und Do-it-yourself-Prototypen Aufmerksamkeit auf Konzepte des robotischen Haareschneidens. Diese Projekte kombinierten mechanische Aktuation, Sensorik und menschliche Aufsicht, blieben jedoch experimentelle Demonstrationen statt validierter oder kommerziell eingesetzter Systeme. Dieselbe Unterscheidung wird auch in [Shuai Li (2025)](../publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf) betont.

### Verwandte Haarpflege- und Frisierroboter

Mehrere akademische Systeme haben dem Haareschneiden benachbarte Aufgaben wie Haarewaschen, Kopfhautmassage, Bürsten, Kämmen, Entwirren und das Stylen des vorderen Haarbereichs untersucht. Obwohl diese Systeme nicht unbedingt Haare schneiden, behandeln sie viele derselben technischen Fragen, darunter die Wahrnehmung deformierbarer Haare, kontaktreiche Manipulation, Pfadplanung, Nutzerkomfort und Sicherheit in Kopfnähe ([Ando et al., 2013](#ref-ando-2013); [Hughes et al., 2021](#ref-hughes-2021); [Dennler et al., 2021](#ref-dennler-2021); [Yoo et al., 2024](#ref-yoo-2024); [Kim et al., 2025](#ref-kim-2025)).

Beispiele sind Haarwasch- und Kopfpflege-Roboter, feedbackgesteuerte Entwirrsysteme, robotische Kämmsysteme, weiche Haarmanipulationssysteme wie MOE-Hair sowie Front-Hair-Styling-Systeme auf Basis wurzelzentrierter Stranganpassung.

### Digitale Frisurenmodellierungs- und Simulationssysteme

Neben physischen Robotersystemen liefern auch digitale Werkzeuge zur Frisurenmodellierung und -simulation wichtige Bezugspunkte für robotisches Haareschneiden. [Digital Salon](#ref-he-2025-digital-salon) ist ein KI- und physikbasiertes System für die 3D-Haargenerierung, interaktive Pflege, Echtzeitsimulation und Bildrendering. Es unterstützt die Erzeugung von Zielfrisuren mittels natürlicher Sprache und ermöglicht es Nutzern, Frisuren in einer dreidimensionalen Umgebung zu verfeinern und zu simulieren. Obwohl das System selbst kein reales Haareschneiden ausführt, zeigt es, wie Nutzersprache, die Spezifikation von Zielfrisuren, strangbasierte Modellierung, interaktive Bearbeitung und visuelle Vorschau in einem einheitlichen Workflow zusammengeführt werden können. Dadurch ist es für Zielfrisurenrepräsentation, simulationsbasierte Validierung und Mensch-Roboter-Interaktionsschnittstellen im robotischen Haareschneiden relevant.

### Akademische Entwicklung

In den 2020er Jahren begann sich robotisches Haareschneiden als eigenes Forschungsthema in der Servicerobotik und persönlichen Pflegeautomatisierung herauszubilden. Frühe Monografien und Überblicksarbeiten beschrieben Haareschneiden als multidisziplinäres Ingenieurproblem, das Wahrnehmung, Modellierung deformierbarer Objekte, Bewegungsplanung, Regelung, Teleoperation, Mensch-Roboter-Interaktion und Sicherheit umfasst. Diese Arbeiten betonten zudem die Schwierigkeit des Arbeitens in Kopfnähe, einschließlich Unsicherheit in der Haargeometrie, Unterschiede zwischen Nutzern und des Bedarfs an eng integrierten Wahrnehmungs-Planungs-Regelungs-Pipelines. Gleichzeitig führten sie breitere konzeptionelle Perspektiven ein, etwa robotisches Haareschneiden als CNC-ähnlichen Prozess oder als Mobile-Robotics-artige Abdeckungsaufgabe mit Sicherheitsbeschränkungen in kritischen Bereichen ([Li, 2025](../publications/2025/Haircutting_Robots.pdf); [Shuai Li, 2025](../publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf); [Khan und Li, 2026a](../publications/2026/CNC_Inspired_Robotic_Hair_Cutting_A_Comprehensive_Survey_on_Precision_Personal_Care_Automation.pdf); [Khan und Li, 2026b](../publications/2026/Robotic_Haircutting_Systems_A_Survey_of_Methods_Challenges_and_Hair_Modeling_Insights.pdf)).

Ein neu in *International Journal of Systems Science* veröffentlichter Artikel entwickelt diese Mobile-Robotics-Perspektive auf Haareschneide-Roboter weiter ([Huang, Khan und Li, 2026](https://doi.org/10.1080/00207721.2026.2687894)).

Neuere Arbeiten verknüpfen robotisches Haareschneiden außerdem mit Vision-Language-Action-Architekturen und verwenden das Feld als konkreten Rahmen zur Diskussion höherer Systemintelligenz, Evaluation und Einsatzstrategien ([Khan und Li, 2026c](../publications/2026/Vision_Language_Action_Modules_for_Intelligent_Haircutting_Robots__A_Position_Paper_on_Architectures_Evaluation_and_Future_Direction.pdf)).

### KI-generierte Videos zum robotischen Haareschneiden

Seit Ende 2025 haben generative KI-Videowerkzeuge zu einer Welle fiktiver Videos über robotisches Haareschneiden im Internet beigetragen. Diese Videos zeigten humanoide Roboter-Friseure, Multiarm-Arbeitsstationen und helmartige automatische Haarschneidegeräte. Obwohl die Inhalte fiktiv waren, steigerten sie die öffentliche Aufmerksamkeit und spiegelten das wachsende Interesse an automatisierter Körperpflege wider.

## Sicherheit

Sicherheit ist beim robotischen Haareschneiden zentral, weil der Roboter in Kopfnähe arbeitet und dabei Werkzeuge wie Clipper, Scheren, Rasierer, Trockner oder beheizte Stylingwerkzeuge verwendet. Relevante Gefahren sind Wahrnehmungsfehler, unerwartete Kopfbewegungen, übermäßige Kontaktkräfte, Werkzeugüberhitzung, Fehlpositionierung des Schneidwerkzeugs, Kalibrierfehler, Kommunikationsverzögerungen bei Teleoperation sowie Software- oder Regelungsfehler.

Vorgeschlagene Sicherheitsmaßnahmen umfassen Arbeitsraumbeschränkungen, Geschwindigkeits- und Beschleunigungsgrenzen, Kraft- oder Druckschwellen, nachgiebige Mechanismen, weiche Abdeckungen oder Endeffektoren, Not-Aus-Funktionen, Nahbereichsüberwachung, redundante Sensorik und automatische Unterbrechung bei erkannten Gefahrensituationen.

Für robotisches Haareschneiden existiert kein eigener internationaler Sicherheitsstandard. Mehrere bestehende Standards bieten jedoch nützliche Referenzpunkte für Risikoanalyse und Systemgestaltung, insbesondere [ISO 13482](#ref-iso-13482), [ISO/TS 15066](#ref-iso-ts-15066), [ISO 10218-1](#ref-iso-10218-1) und [ISO 14971](#ref-iso-14971). Gefahrenkategorien, Minderungsstrategien und die Bedeutung dieser Standards für eine haarschneidespezifische Risikoanalyse werden in [Shuai Li (2025)](../publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf) sowie in einem [Sicherheitsüberblick von 2026](https://doi.org/10.1002/rob.70305) behandelt.

## Herausforderungen und Forschungsrichtungen

Zu den zentralen Herausforderungen gehören die zuverlässige Wahrnehmung von Haar und Kopfhaut, die Modellierung vielfältiger Haartypen, die Kompensation von Nutzerbewegungen, die Planung sicherer Werkzeugtrajektorien, die Aufrechterhaltung angemessener Werkzeugabstände und Kontaktkräfte sowie das Arbeiten in der Nähe empfindlicher Bereiche wie Ohren, Augen, Gesicht und Kopfhaut.

Haare sind besonders schwer zu handhaben, weil sie deformierbar, strangbasiert und hinsichtlich Länge, Dichte, Lockenmuster, Steifigkeit und Feuchtigkeit stark variabel sind. Selbst bei hoher geometrischer Präzision bleibt die ästhetische Bewertung schwierig, weil die Qualität eines Haarschnitts auch von Stilpräferenzen, Symmetrie, Komfort und Nutzererwartungen abhängt.

Weitere Herausforderungen sind Langzeitbetrieb, Erschwinglichkeit, Zertifizierung, Haftung, Nutzerakzeptanz, Privatsphäre und Datenverarbeitung. Systeme, die Kameras oder dreidimensionale Scans verwenden, können Gesichts-, Kopfhaut- oder Frisurdaten erfassen und damit zusätzlich zu allgemeinen Sicherheitsfragen auch Datenschutzprobleme aufwerfen.

Diese Herausforderungen weisen auf mehrere vielversprechende Forschungsrichtungen im robotischen Haareschneiden hin:

- Autonome Ausführung von Haarschnitten
- Teleoperiertes Haareschneiden für entfernte Expertensteuerung
- Shared-Autonomy-Systeme, die menschliche Aufsicht mit robotischer Ausführung verbinden
- Haarschnittplanung auf Basis von Zielfrisuren, geometrischen Spezifikationen oder Nutzeranweisungen
- 3D-Haarmodellierung und physikalische Simulation für Zielfrisurengenerierung, digitale Vorschau und Validierung robotischer Ausführung
- Echtzeitwahrnehmung von Haar, Kopfhaut und Kopfpose während des Schneidens
- Kompensation von Nutzerbewegungen und anderen Störungen während des Betriebs
- Sicherheitsbewusste Regelung für den Betrieb in der Nähe empfindlicher anatomischer Regionen
- Evaluationsprotokolle, Benchmark-Methoden und zertifizierungsorientiertes Systemdesign
- Einsatzorientierte Systemintegration für einen zuverlässigen Betrieb in realen Anwendungen

## Laufende Arbeit

Zusätzlich zu den hier gesammelten Veröffentlichungen entwickelt das Team hinter diesem Repository über das folgende öffentliche Projekt ein ferngesteuertes teleoperiertes Haareschneide-Robotersystem:

- [Client_RHCR](https://github.com/Dai0731csc/Client_RHCR): ein clientseitiges System für ferngesteuertes teleoperiertes robotisches Haareschneiden. Es unterstützt browserbasierte Wahrnehmung, Kalibrierung, Kommunikation und Raw-Pose-Streaming. Beiträge von Forschenden und Entwicklern, die sich für dieses Thema interessieren, sind willkommen.

### Teleoperationsdemonstrationen

| Normalbetrieb [\[9\]](#team-publication-9) | Rebase-Betrieb [\[9\]](#team-publication-9) |
| --- | --- |
| ![Demo der normalen Teleoperation](../ongoing-work/media/teleoperation/Normal.gif) | ![Demo der Rebase-Teleoperation](../ongoing-work/media/teleoperation/Rebase.gif) |

| Sicherheits-Governor [\[8\]](#team-publication-8) | Not-Aus [\[9\]](#team-publication-9) |
| --- | --- |
| ![Demo des Sicherheits-Governors bei der Teleoperation](../ongoing-work/media/teleoperation/Safety_governor.gif) | ![Demo des Not-Aus bei der Teleoperation](../ongoing-work/media/teleoperation/Emergency_stop.gif) |

Weitere laufende Arbeiten dieses Teams sind in [../ongoing-work/README.md](../ongoing-work/README.md) organisiert.

## Bildung und Training

Neben Forschungsarbeiten und Implementierungsprojekten sammelt dieses Repository auch Lehr- und Trainingsmaterialien zum robotischen Haareschneiden. Diese Ressourcen sind in [../education/README.md](../education/README.md) organisiert.

- [Capstone Weekly Planning 2026](../education/Capstone%20Weekly%20Planning_2026.pdf): ein Kursprojekt-Planungsdokument für studentisches Training und Projektbeteiligung.

## Fragen und Antworten (Q&A)

Neben der Übersicht oben sammelt dieses Repository Frage-und-Antwort-Materialien zum robotischen Haareschneiden im Verzeichnis [../Q&A/](../Q&A/).

Die Materialien fassen Antworten von Studierenden und Teilnehmenden auf einen Projektfragebogen zusammen und enthalten kurze Hintergrundnotizen des Forschungsteams. Behandelte Themen sind unter anderem:

- Kommerzialisierungsaussichten und Einführungszeitpläne
- KI- und Wahrnehmungsunterstützung beim robotischen Haareschneiden
- mechanische Struktur, Werkzeuge und Sicherheitsmechanismen
- Steuerung, Bewegungsplanung und Trajektoriengenerierung
- Marktpotenzial, Nutzervertrauen und Modelle geteilter Autonomie
- weitere offene Fragen und Folgediskussion

- [Q & A about haircutting robots](../Q&A/Q%20%26%20A%20about%20haircutting%20robots.pdf): gesammelte Fragen und Antworten zu den genannten Themen.

## Verwandte Projekte und Werkzeuge

Relevante Referenzprojekte und Werkzeuge sind nach Kategorien in [../related-projects/README.md](../related-projects/README.md) organisiert. Dieses Verzeichnis dient als erweiterbare Referenz für technische Grundlagen im breiteren Forschungsumfeld des robotischen Haareschneidens.

## Literaturhinweise

- <a id="ref-gronier-1966"></a>Jean Gronier. *Automatic hair-cutting machine having programmed control means for cutting hair in a predetermined style*. US Patent 3241562A, 1966. [[link](https://patents.google.com/patent/US3241562A/en)]
- <a id="ref-aldabbah-2023"></a>Mubarak Aldabbah. *Automatic hair cutter robot*. WO Patent 2023080812A1, 2023. [[link](https://patents.google.com/patent/WO2023080812A1/en)]
- <a id="ref-futami-2014"></a>Kyosuke Futami, Tsutomu Terada, and Masahiko Tsukamoto. *A System for Supporting Self-Haircuts Using Camera Equipped Robot*. MoMM, 2014. [[link](https://doi.org/10.1145/2684103.2684143)]
- <a id="ref-ando-2013"></a>Takeshi Ando et al. *Biosignal-based relaxation evaluation of head-care robot*. EMBC, 2013. [[link](https://doi.org/10.1109/embc.2013.6611101)]
- <a id="ref-hughes-2021"></a>Josie Hughes et al. *Detangling hair using feedback-driven robotic brushing*. RoboSoft, 2021. [[link](https://doi.org/10.1109/RoboSoft51838.2021.9479221)]
- <a id="ref-dennler-2021"></a>Nathaniel Dennler, Eura Shin, Maja Mataric, and Stefanos Nikolaidis. *Design and Evaluation of a Hair Combing System Using a General-Purpose Robotic Arm*. IROS, 2021. [[link](https://doi.org/10.1109/IROS51168.2021.9636768)]
- <a id="ref-yoo-2024"></a>Uksang Yoo et al. *MOE-Hair: Toward Soft and Compliant Contact-rich Hair Manipulation and Care*. HRI Companion, 2024. [[link](https://doi.org/10.1145/3610978.3640682)]
- <a id="ref-kim-2025"></a>Soonhyo Kim et al. *Front Hair Styling Robot System Using Path Planning for Root-Centric Strand Adjustment*. SII, 2025. [[link](https://doi.org/10.1109/SII59315.2025.10871088)]
- <a id="ref-he-2025-digital-salon"></a>Chengan He et al. *Digital Salon: An AI and Physics-Driven Tool for 3D Hair Grooming and Simulation*. arXiv:2507.07387, 2025. [[link](https://doi.org/10.48550/arXiv.2507.07387)][[code](https://github.com/Dai0731csc/Digital-Salon)]
- <a id="ref-iso-13482"></a>ISO 13482. *Robots and robotic devices - Safety requirements for personal care robots*.
- <a id="ref-iso-ts-15066"></a>ISO/TS 15066. *Robots and robotic devices - Collaborative robots*.
- <a id="ref-iso-10218-1"></a>ISO 10218-1. *Robotics - Safety requirements for industrial robots - Part 1: Robots*.
- <a id="ref-iso-14971"></a>ISO 14971. *Medical devices - Application of risk management to medical devices*.

## Veröffentlichungen in diesem Repository

Dieses Projekt wird an der Universität Oulu von [Professor Shuai Li](https://www.oulu.fi/en/researchers/shuai-li) geleitet und konzentriert sich derzeit auf Forschung zum robotischen Haareschneiden. Die einschlägigen Veröffentlichungen wurden in den obigen Abschnitten bereits erwähnt und sind in diesem Repository gesammelt. Sie sind nachfolgend aufgeführt.

### 2025

- <a id="team-publication-1"></a>[1] S. Li, *Haircutting Robots*. Cham, Switzerland: Springer, 2025. DOI: [10.1007/978-3-031-84026-5](https://doi.org/10.1007/978-3-031-84026-5). [PDF](../publications/2025/Haircutting_Robots.pdf).
- <a id="team-publication-2"></a>[2] S. Li, "Haircutting Robots: From Theory to Practice," *Automation*, vol. 6, no. 3, article 47, 2025. DOI: [10.3390/automation6030047](https://doi.org/10.3390/automation6030047). [PDF](../publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf).

### 2026

- <a id="team-publication-3"></a>[3] A. T. Khan and S. Li, "Robotic Haircutting Systems: A Survey of Methods, Challenges, and Hair Modeling Insights," *IEEE Journal of Selected Areas in Sensors*, vol. 3, pp. 104–112, 2026. DOI: [10.1109/JSAS.2026.3654480](https://doi.org/10.1109/JSAS.2026.3654480). [PDF](../publications/2026/Robotic_Haircutting_Systems_A_Survey_of_Methods_Challenges_and_Hair_Modeling_Insights.pdf).
- <a id="team-publication-4"></a>[4] A. T. Khan and S. Li, "CNC-Inspired Robotic Hair Cutting: A Comprehensive Survey on Precision Personal Care Automation," *Journal of Artificial Intelligence for Automation*, vol. 1, no. 1, article 2, 2026. DOI: [10.53941/jaia.2026.100002](https://doi.org/10.53941/jaia.2026.100002). [PDF](../publications/2026/CNC_Inspired_Robotic_Hair_Cutting_A_Comprehensive_Survey_on_Precision_Personal_Care_Automation.pdf).
- <a id="team-publication-5"></a>[5] A. T. Khan and S. Li, "Vision-Language-Action Models for Intelligent Haircutting Robots: A Position Paper on Architectures, Evaluation, and Future Directions," ResearchGate, position paper, 2026. DOI: [10.13140/RG.2.2.30849.62563](https://doi.org/10.13140/RG.2.2.30849.62563). [PDF](../publications/2026/Vision_Language_Action_Modules_for_Intelligent_Haircutting_Robots__A_Position_Paper_on_Architectures_Evaluation_and_Future_Direction.pdf).
- <a id="team-publication-6"></a>[6] Z. Huang, A. T. Khan, and S. Li, "Haircutting robots: a mobile robotics perspective," *International Journal of Systems Science*, pp. 1–20, 2026. DOI: [10.1080/00207721.2026.2687894](https://doi.org/10.1080/00207721.2026.2687894). [PDF](../publications/2026/Haircutting%20robots%20%20a%20mobile%20robotics%20perspective.pdf).
- <a id="team-publication-7"></a>[7] Z. Huang, A. Vilkki, S. Li, and J. Röning, "Safety in Robotic Haircutting," *Journal of Field Robotics*, pp. 1–25, 2026. DOI: [10.1002/rob.70305](https://doi.org/10.1002/rob.70305). [PDF](../publications/2026/Safety_in_Robotic_Haircutting.pdf).
- <a id="team-publication-8"></a>[8] Z. Huang, A. T. Khan, A. M. Mohammed, F. Lo Regio, J.-J. Torvinen, L. Angrisani, and S. Li, "A Safety Boundary Governor for Teleoperated Robotic Haircutting," conference submission, 2026. [PDF](../publications/2026/A%20Safety%20Boundary%20Governor%20for%20Teleoperated%20Robotic%20Haircutting.pdf).
- <a id="team-publication-9"></a>[9] Z. Huang, A. Vilkki, J. Huang, B. Liao, C. Luo, L. Angrisani, and S. Li, "TeleHairing: A Teleoperation Baseline for Robotic Haircutting," *arXiv preprint*, arXiv:2610.07096, 2026. DOI: [10.48550/arXiv.2610.07096](https://doi.org/10.48550/arXiv.2610.07096). [PDF](../publications/2026/TeleHairing.pdf).
