# Robotisches Haareschneiden

Sprachen: [English](README.md) | [中文](README.zh.md) | [Suomi](README.fi.md) | Deutsch | [Français](README.fr.md)

Dieses Repository dient in erster Linie als enzyklopädischer Überblick über robotisches Haareschneiden und behandelt Hintergrund, Geschichte, Sicherheit, Herausforderungen, Forschungsrichtungen und Literaturhinweise. Relevante in diesem Repository gesammelte Veröffentlichungen sind am Ende aufgeführt.

## Überblick

Robotisches Haareschneiden bezeichnet den Einsatz robotischer Systeme zur Unterstützung oder vollständigen Ausführung von Haarschneidevorgängen. Der Begriff kann Trimmen, Rasieren, Frisieren und weitere verwandte Pflegeaufgaben umfassen. Robotische Plattformen, die für diese Aufgaben entwickelt wurden, werden üblicherweise als Haarschneide-Roboter bezeichnet.

Das Gebiet liegt an der Schnittstelle von Robotik, Computer Vision, Bewegungsplanung, Manipulation, Mensch-Roboter-Interaktion, Kommunikation, Computergrafik, virtueller Realität, künstlicher Intelligenz und Haptik.

Im Gegensatz zu gewöhnlichen elektrischen Haarschneidemaschinen oder manuell geführten Pflegewerkzeugen benötigen robotische Haarschneidesysteme Wahrnehmungs-, Planungs- und Regelungsfähigkeiten, damit ein Roboter ein Schneide- oder Pflegewerkzeug relativ zu Kopf und Haar positionieren kann. Dies ist technisch anspruchsvoll, weil Haare deformierbar sind, zwischen Personen stark variieren und in der Nähe empfindlicher anatomischer Bereiche wie Ohren, Augen, Kopfhaut und Gesicht bearbeitet werden.

Die Systeme reichen von teleoperierten Plattformen bis zu autonomeren Konzepten. Stand 2025 ist kein vollständig kommerzieller Haarschneide-Roboter breit im Einsatz, doch Forschungsprototypen und Überblicksarbeiten deuten auf einen plausiblen Weg zur Kommerzialisierung hin.

## Geschichte

### Frühe automatische Haarschneidegeräte

Ideen zum automatischen Haareschneiden entstanden lange vor modernen robotischen Systemen. Ein US-Patent von [Jean Gronier](#ref-gronier-1966) aus dem Jahr 1966 beschrieb eine automatische Haarschneidemaschine, die mithilfe programmierter Steuerung eine vorgegebene Frisur erzeugen sollte. Es lässt sich besser als vor-robotische Automatisierung denn als modernes robotisches Haarschneidesystem verstehen, da es auf mechanischer Struktur und vorgegebenen Programmen beruhte und nicht auf Echtzeitwahrnehmung oder adaptivem Feedback.

Spätere Patente schlugen integriertere Systeme vor, die Wahrnehmung, robotische Mechanismen und Benutzerschnittstellen kombinierten. Das zeigt einen Übergang zu deutlicher robotischeren Umsetzungen, darunter auch das spätere Patent von [Mubarak Aldabbah](#ref-aldabbah-2023).

### Kameragestützte Selbsthaarschnitt-Systeme

Eine verwandte Richtung konzentrierte sich darauf, Menschen beim eigenen Haareschneiden zu unterstützen, anstatt den Schnitt autonom durch einen Roboter ausführen zu lassen. 2014 stellten [Futami, Terada und Tsukamoto](#ref-futami-2014) ein robotisches System mit beweglicher Kamera vor, das Nutzern während des Selbsthaarschnitts unterschiedliche Blickwinkel auf den eigenen Kopf ermöglichte.

### Robotische Haarschneide-Prototypen

In den 2020er Jahren lenkten mehrere öffentliche Demonstrationen und Do-it-yourself-Prototypen Aufmerksamkeit auf Konzepte des robotischen Haareschneidens. Diese Projekte kombinierten mechanische Aktuation, Sensorik und menschliche Aufsicht, blieben aber im Allgemeinen experimentelle Demonstrationen statt validierter oder kommerziell eingesetzter Systeme; dieselbe Unterscheidung wird auch in [Shuai Li (2025)](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf) betont.

### Verwandte Haarpflege- und Frisierroboter

Mehrere akademische Systeme untersuchten dem Haareschneiden benachbarte Aufgaben wie Haarewaschen, Kopfhautmassage, Bürsten, Kämmen, Entwirren und das Stylen des vorderen Haarbereichs. Diese Systeme schneiden nicht notwendigerweise Haare, behandeln aber viele derselben technischen Fragen, darunter die Wahrnehmung deformierbarer Haare, kontaktreiche Manipulation, Pfadplanung, Nutzerkomfort und Sicherheit in Kopfnähe ([Ando et al., 2013](#ref-ando-2013); [Hughes et al., 2021](#ref-hughes-2021); [Dennler et al., 2021](#ref-dennler-2021); [Yoo et al., 2024](#ref-yoo-2024); [Kim et al., 2025](#ref-kim-2025)).

Beispiele sind Haarwasch- und Kopfpflege-Roboter, feedbackgesteuerte Entwirrsysteme, robotische Kämmsysteme, weiche Haarmanipulationssysteme wie MOE-Hair sowie Front-Hair-Styling-Systeme auf Basis wurzelzentrierter Strangverstellung.

### Digitale Frisurenmodellierungs- und Simulationssysteme

Neben physischen Robotersystemen liefern auch digitale Werkzeuge zur Frisurenmodellierung und -simulation wichtige Bezugspunkte für robotisches Haareschneiden. [Digital Salon](#ref-he-2025-digital-salon) ist ein KI- und physikbasiertes System für die 3D-Haargenerierung, interaktive Haarbearbeitung, Echtzeitsimulation und Bildrendering. Es unterstützt die Erzeugung von Zielfrisuren mittels natürlicher Sprache und ermöglicht es Nutzern, Frisuren in einer dreidimensionalen Umgebung zu verfeinern und dynamisch zu simulieren. Obwohl das System selbst kein reales Haareschneiden ausführt, zeigt es, wie Nutzersprache, Zielfrisuren, strangbasierte Modellierung, interaktive Bearbeitung und visuelle Vorschau in einem einheitlichen Workflow zusammengeführt werden können. Es kann daher als relevante technische Grundlage für Zielfrisurenrepräsentation, simulationsbasierte Validierung und Mensch-Roboter-Interaktionsschnittstellen im robotischen Haareschneiden betrachtet werden.

### Akademische Entwicklung

In den 2020er Jahren begann sich robotisches Haareschneiden als eigenes Forschungsthema in der Servicerobotik und persönlichen Pflegeautomatisierung herauszubilden. Frühe Monografien und Überblicksarbeiten beschrieben Haareschneiden als multidisziplinäres Ingenieurproblem, das Wahrnehmung, Modellierung deformierbarer Objekte, Bewegungsplanung, Regelung, Teleoperation, Mensch-Roboter-Interaktion und Sicherheit umfasst. Diese Arbeiten betonten zugleich die Schwierigkeit des Arbeitens in Kopfnähe, einschließlich Unsicherheit in der Haargeometrie, Unterschiede zwischen Nutzern und des Bedarfs an eng integrierten Wahrnehmungs-Planungs-Regelungs-Pipelines. Außerdem führten sie breitere konzeptionelle Rahmungen ein, etwa robotisches Haareschneiden als CNC-ähnlichen Prozess oder als Mobile-Robotics-artige Abdeckungsaufgabe mit Sicherheitsbeschränkungen in kritischen Bereichen ([Li, 2025](publications/2025/LiHaircutting%20Robots.pdf); [Shuai Li, 2025](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf); [Khan und Li, 2026a](publications/2026/CNC_Inspired_Robotic_Hair_Cutting_A_Comprehensive_Survey_on_Precision_Personal_Care_Automation.pdf); [Khan und Li, 2026b](publications/2026/Robotic_Haircutting_Systems_A_Survey_of_Methods_Challenges_and_Hair_Modeling_Insights.pdf)).

Neuere Arbeiten verknüpfen robotisches Haareschneiden außerdem mit Vision-Language-Action-Architekturen und verwenden das Feld als konkretes Beispiel zur Diskussion höherer Systemintelligenz, Evaluation und Einsatzstrategien ([Khan und Li, 2026c](publications/2026/Vision_Language_Action_Modules_for_Intelligent_Haircutting_Robots__A_Position_Paper_on_Architectures_Evaluation_and_Future_Direction.pdf)).

### KI-generierte Videos zum robotischen Haareschneiden

Seit Ende 2025 führten generative KI-Videowerkzeuge zu einer Welle fiktiver Videos über robotisches Haareschneiden im Internet. Diese zeigten humanoide Roboter-Friseure, Multiarm-Arbeitsstationen und helmartige automatische Haarschneidegeräte. Obwohl diese Inhalte fiktiv waren, steigerten sie die öffentliche Aufmerksamkeit und spiegelten das wachsende Interesse an automatisierter Körperpflege wider.

## Sicherheit

Sicherheit ist beim robotischen Haareschneiden zentral, weil der Roboter in Kopfnähe arbeitet und dabei Werkzeuge wie Clipper, Scheren, Rasierer, Trockner oder beheizte Stylingwerkzeuge verwendet. Relevante Gefahren sind Wahrnehmungsfehler, unerwartete Kopfbewegungen, übermäßige Kontaktkräfte, Werkzeugüberhitzung, Fehlpositionierung des Schneidwerkzeugs, Kalibrierfehler, Kommunikationsverzögerungen bei Teleoperation sowie Software- oder Regelungsfehler.

Vorgeschlagene Sicherheitsmaßnahmen umfassen Arbeitsraumbeschränkungen, Geschwindigkeits- und Beschleunigungsgrenzen, Kraft- oder Druckschwellen, nachgiebige Mechanismen, weiche Abdeckungen oder Endeffektoren, Not-Aus-Funktionen, Nahbereichsüberwachung, redundante Sensorik und automatische Unterbrechung bei erkannten Gefahrensituationen.

Für robotisches Haareschneiden existiert kein eigener internationaler Sicherheitsstandard. Mehrere bestehende Standards sind jedoch für Risikoanalyse und Systemgestaltung relevant, insbesondere [ISO 13482](#ref-iso-13482), [ISO/TS 15066](#ref-iso-ts-15066), [ISO 10218-1](#ref-iso-10218-1) und [ISO 14971](#ref-iso-14971). Gefahrenkategorien, Minderungsstrategien und die Bedeutung dieser Standards für eine haarschneidespezifische Risikoanalyse werden in [Shuai Li (2025)](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf) sowie in einem [Sicherheitsüberblick von 2025](publications/2025/Safety_in_Robotic_Haircutting.pdf) behandelt.

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
- Einsatzorientierte Systemintegration für einen zuverlässigen realen Betrieb

## Literaturhinweise

- <a id="ref-gronier-1966"></a>Jean Gronier. *Automatic hair-cutting machine having programmed control means for cutting hair in a predetermined style*. US Patent 3241562A, 1966. [[link](https://patents.google.com/patent/US3241562A/en)]
- <a id="ref-aldabbah-2023"></a>Mubarak Aldabbah. *Automatic hair cutter robot*. WO Patent 2023080812A1, 2023. [[link](https://patents.google.com/patent/WO2023080812A1/en)]
- <a id="ref-futami-2014"></a>Kyosuke Futami, Tsutomu Terada, and Masahiko Tsukamoto. *A System for Supporting Self-Haircuts Using Camera Equipped Robot*. MoMM, 2014. [[link](https://doi.org/10.1145/2684103.2684143)]
- <a id="ref-ando-2013"></a>Takeshi Ando et al. *Biosignal-based relaxation evaluation of head-care robot*. EMBC, 2013. [[link](https://doi.org/10.1109/embc.2013.6611101)]
- <a id="ref-hughes-2021"></a>Josie Hughes et al. *Detangling hair using feedback-driven robotic brushing*. RoboSoft, 2021. [[link](https://doi.org/10.1109/RoboSoft51838.2021.9479221)]
- <a id="ref-dennler-2021"></a>Nathaniel Dennler, Eura Shin, Maja Mataric, and Stefanos Nikolaidis. *Design and Evaluation of a Hair Combing System Using a General-Purpose Robotic Arm*. IROS, 2021. [[link](https://doi.org/10.1109/IROS51168.2021.9636768)]
- <a id="ref-yoo-2024"></a>Uksang Yoo et al. *MOE-Hair: Toward Soft and Compliant Contact-rich Hair Manipulation and Care*. HRI Companion, 2024. [[link](https://doi.org/10.1145/3610978.3640682)]
- <a id="ref-kim-2025"></a>Soonhyo Kim et al. *Front Hair Styling Robot System Using Path Planning for Root-Centric Strand Adjustment*. SII, 2025. [[link](https://doi.org/10.1109/SII59315.2025.10871088)]
- <a id="ref-he-2025-digital-salon"></a>Chengan He et al. *Digital Salon: An AI and Physics-Driven Tool for 3D Hair Grooming and Simulation*. arXiv:2507.07387, 2025. [[link](https://doi.org/10.48550/arXiv.2507.07387)]
- <a id="ref-iso-13482"></a>ISO 13482. *Robots and robotic devices - Safety requirements for personal care robots*.
- <a id="ref-iso-ts-15066"></a>ISO/TS 15066. *Robots and robotic devices - Collaborative robots*.
- <a id="ref-iso-10218-1"></a>ISO 10218-1. *Robotics - Safety requirements for industrial robots - Part 1: Robots*.
- <a id="ref-iso-14971"></a>ISO 14971. *Medical devices - Application of risk management to medical devices*.

## Veröffentlichungen in diesem Repository

Die folgenden Veröffentlichungen werden in den obigen Abschnitten genannt und sind in diesem Repository gesammelt.

### 2025

- [Haircutting Robots](publications/2025/LiHaircutting%20Robots.pdf)
- [Haircutting Robots from Theory to Practice](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf)
- [Safety in Robotic Haircutting](publications/2025/Safety_in_Robotic_Haircutting.pdf)

### 2026

- [CNC-Inspired Robotic Hair Cutting: A Comprehensive Survey on Precision Personal Care Automation](publications/2026/CNC_Inspired_Robotic_Hair_Cutting_A_Comprehensive_Survey_on_Precision_Personal_Care_Automation.pdf)
- [Robotic Haircutting Systems: A Survey of Methods, Challenges and Hair Modeling Insights](publications/2026/Robotic_Haircutting_Systems_A_Survey_of_Methods_Challenges_and_Hair_Modeling_Insights.pdf)
- [Vision-Language-Action Modules for Intelligent Haircutting Robots: A Position Paper on Architectures, Evaluation and Future Direction](publications/2026/Vision_Language_Action_Modules_for_Intelligent_Haircutting_Robots__A_Position_Paper_on_Architectures_Evaluation_and_Future_Direction.pdf)
