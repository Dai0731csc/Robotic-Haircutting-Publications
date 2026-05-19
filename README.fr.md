# Coupe de cheveux robotique

Langues : [English](README.md) | [中文](README.zh.md) | [Suomi](README.fi.md) | [Deutsch](README.de.md) | Français

Ce dépôt sert principalement de vue d'ensemble de type encyclopédique sur la coupe de cheveux robotique. Il rassemble des éléments de contexte, d'histoire, de sécurité, de défis, de directions de recherche et de références. Les publications pertinentes rassemblées dans ce dépôt sont listées à la fin.

## Vue d'ensemble

La coupe de cheveux robotique désigne l'utilisation de systèmes robotiques pour assister ou réaliser entièrement des opérations de coupe de cheveux. Le terme peut englober la tonte, le rasage, le coiffage et d'autres tâches de soin apparentées. Les plateformes robotiques conçues pour ces tâches sont généralement appelées robots de coupe de cheveux.

Ce domaine se situe à l'intersection de la robotique, de la vision par ordinateur, de la planification du mouvement, de la manipulation robotique, de l'interaction humain-robot, de la communication, de l'infographie, de la réalité virtuelle, de l'intelligence artificielle et de l'haptique.

Contrairement aux tondeuses électriques ordinaires ou aux outils de coiffure manipulés à la main, les systèmes robotiques de coupe de cheveux nécessitent des capacités de perception, de planification et de contrôle permettant à un robot de positionner un outil de coupe ou de soin par rapport à la tête humaine et aux cheveux. Cette tâche est techniquement difficile parce que les cheveux sont déformables, varient fortement d'une personne à l'autre et doivent être manipulés à proximité de régions anatomiques sensibles telles que les oreilles, les yeux, le cuir chevelu et le visage.

Les systèmes vont de plateformes téléopérées à des concepts plus autonomes. En 2025, aucun robot de coupe de cheveux entièrement commercial n'était largement déployé, mais les prototypes de recherche et les travaux de synthèse suggèrent une trajectoire plausible vers la commercialisation.

## Histoire

### Premiers dispositifs automatiques de coupe de cheveux

Les idées de coupe de cheveux automatisée sont apparues bien avant les systèmes robotiques modernes. Un brevet américain obtenu en 1966 par [Jean Gronier](#ref-gronier-1966) décrivait une machine automatique de coupe de cheveux utilisant un contrôle programmé pour produire une coiffure prédéterminée. Il est plus juste de le considérer comme une automatisation pré-robotique que comme un système robotique moderne de coupe de cheveux, car il reposait sur une structure mécanique et des programmes prédéfinis plutôt que sur une perception en temps réel ou un retour adaptatif.

Des brevets ultérieurs ont proposé des systèmes plus intégrés combinant perception, mécanismes robotiques et interfaces utilisateur. Cela marque une transition vers des réalisations plus nettement robotiques, y compris le brevet ultérieur de [Mubarak Aldabbah](#ref-aldabbah-2023).

### Systèmes d'auto-coupe assistés par caméra

Une direction connexe visait à aider les personnes à se couper elles-mêmes les cheveux plutôt qu'à faire exécuter la coupe de manière autonome par un robot. En 2014, [Futami, Terada et Tsukamoto](#ref-futami-2014) ont proposé un système robotique équipé d'une caméra mobile permettant à l'utilisateur d'observer sa tête sous différents angles pendant une auto-coupe.

### Prototypes robotiques de coupe de cheveux

Dans les années 2020, plusieurs démonstrations publiques et prototypes artisanaux ont attiré l'attention sur les concepts de coupe de cheveux robotique. Ces projets combinaient actionnement mécanique, capteurs et supervision humaine, mais relevaient généralement de démonstrations expérimentales plutôt que de systèmes validés ou commercialement déployés ; cette distinction est également soulignée dans [Shuai Li (2025)](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf).

### Robots de soin capillaire et de coiffage apparentés

Plusieurs systèmes académiques ont étudié des tâches voisines de la coupe de cheveux, comme le shampooing, le massage du cuir chevelu, le brossage, le peignage, le démêlage et la mise en forme de la frange. Ces systèmes ne coupent pas nécessairement les cheveux, mais abordent nombre des mêmes questions techniques, notamment la perception de cheveux déformables, la manipulation riche en contacts, la planification de trajectoire, le confort de l'utilisateur et la sécurité à proximité de la tête ([Ando et al., 2013](#ref-ando-2013); [Hughes et al., 2021](#ref-hughes-2021); [Dennler et al., 2021](#ref-dennler-2021); [Yoo et al., 2024](#ref-yoo-2024); [Kim et al., 2025](#ref-kim-2025)).

Parmi les exemples figurent des robots de lavage et de soin de la tête, des systèmes de démêlage guidés par retour d'information, des plateformes robotiques de peignage, des systèmes souples de manipulation des cheveux comme MOE-Hair, ainsi que des robots de coiffage de l'avant des cheveux fondés sur un ajustement centré sur la racine.

### Systèmes numériques de modélisation et de simulation de coiffures

Outre les systèmes robotiques physiques, les outils numériques de modélisation et de simulation de coiffures fournissent aussi des références importantes pour la coupe de cheveux robotique. [Digital Salon](#ref-he-2025-digital-salon) est un système fondé sur l'IA et la physique pour la génération de cheveux 3D, le coiffage interactif, la simulation en temps réel et le rendu d'images. Il prend en charge la génération de coiffures cibles à partir du langage naturel et permet aux utilisateurs d'affiner et de simuler dynamiquement des coiffures dans un environnement tridimensionnel. Bien que ce système n'exécute pas de coupe réelle, il montre comment le langage utilisateur, les coiffures cibles, la modélisation au niveau des mèches, l'édition interactive et la prévisualisation visuelle peuvent être intégrés dans un flux de travail unifié. Il constitue donc une base technique pertinente pour la représentation de coiffures cibles, la validation par simulation et les interfaces d'interaction humain-robot en coupe de cheveux robotique.

### Développement académique

Dans les années 2020, la coupe de cheveux robotique a commencé à être formulée comme un sujet de recherche distinct en robotique de service et en automatisation des soins personnels. Les premières monographies et études de synthèse ont décrit la coupe de cheveux comme un problème d'ingénierie multidisciplinaire impliquant perception, modélisation d'objets déformables, planification du mouvement, contrôle, téléopération, interaction humain-robot et sécurité. Ces travaux ont également souligné la difficulté d'opérer près de la tête humaine, notamment l'incertitude sur la géométrie des cheveux, la variabilité entre utilisateurs et la nécessité de pipelines étroitement intégrés de perception-planification-contrôle. Ils ont aussi introduit des cadres conceptuels plus larges, par exemple la coupe de cheveux robotique comme un processus de type CNC ou comme une tâche de couverture inspirée de la robotique mobile avec contraintes de sécurité autour de régions critiques ([Li, 2025](publications/2025/LiHaircutting%20Robots.pdf); [Shuai Li, 2025](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf); [Khan et Li, 2026a](publications/2026/CNC_Inspired_Robotic_Hair_Cutting_A_Comprehensive_Survey_on_Precision_Personal_Care_Automation.pdf); [Khan et Li, 2026b](publications/2026/Robotic_Haircutting_Systems_A_Survey_of_Methods_Challenges_and_Hair_Modeling_Insights.pdf)).

Des travaux plus récents ont également relié la coupe de cheveux robotique aux architectures vision-langage-action, en utilisant ce domaine comme cas concret pour discuter de l'intelligence système de plus haut niveau, de l'évaluation et des stratégies de déploiement ([Khan et Li, 2026c](publications/2026/Vision_Language_Action_Modules_for_Intelligent_Haircutting_Robots__A_Position_Paper_on_Architectures_Evaluation_and_Future_Direction.pdf)).

### Vidéos de coupe de cheveux robotique générées par IA

À partir de la fin de l'année 2025, les outils vidéo génératifs d'IA ont alimenté une vague de vidéos fictives de coupe de cheveux robotique en ligne. On y voyait des coiffeurs humanoïdes, des stations multi-bras et des dispositifs automatiques de coupe sous forme de casque. Bien que fictifs, ces contenus ont accru l'attention du public et reflété l'intérêt croissant pour les soins personnels automatisés.

## Sécurité

La sécurité est un enjeu central de la coupe de cheveux robotique, car le robot opère à proximité de la tête humaine en utilisant des outils tels que des tondeuses, des ciseaux, des rasoirs, des sèche-cheveux ou des outils de coiffage chauffants. Les risques pertinents comprennent les erreurs de perception, les mouvements inattendus de la tête, les forces de contact excessives, la surchauffe de l'outil, le mauvais alignement de l'outil de coupe, les erreurs de calibration, les délais de communication en téléopération ainsi que les défaillances logicielles ou de contrôle.

Les mesures de sécurité proposées comprennent des limites d'espace de travail, des contraintes de vitesse et d'accélération, des seuils de force ou de pression, des mécanismes souples, des revêtements ou effecteurs terminaux souples, des fonctions d'arrêt d'urgence, la surveillance de proximité, une instrumentation redondante et l'interruption automatique en cas de situation dangereuse détectée.

Il n'existe pas de norme internationale spécifique à la coupe de cheveux robotique. Toutefois, plusieurs normes existantes sont pertinentes pour l'analyse des risques et la conception des systèmes, notamment [ISO 13482](#ref-iso-13482), [ISO/TS 15066](#ref-iso-ts-15066), [ISO 10218-1](#ref-iso-10218-1) et [ISO 14971](#ref-iso-14971). Les catégories de danger, les stratégies d'atténuation et la pertinence de ces normes pour une analyse des risques spécifique à la coupe de cheveux sont discutées dans [Shuai Li (2025)](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf) ainsi que dans une [synthèse sur la sécurité de 2025](publications/2025/Safety_in_Robotic_Haircutting.pdf).

## Défis et directions de recherche

Parmi les principaux défis figurent la perception fiable des cheveux et du cuir chevelu, la modélisation de types de cheveux variés, la compensation des mouvements de l'utilisateur, la planification de trajectoires d'outils sûres, le maintien d'une distance et d'une force de contact appropriées, ainsi que l'opération à proximité de régions sensibles telles que les oreilles, les yeux, le visage et le cuir chevelu.

Les cheveux sont particulièrement difficiles à manipuler parce qu'ils sont déformables, structurés en mèches et très variables en longueur, densité, motif de boucle, rigidité et humidité. Même lorsque la précision géométrique est élevée, l'évaluation esthétique reste difficile, car la qualité d'une coupe de cheveux dépend aussi des préférences de style, de la symétrie, du confort et des attentes de l'utilisateur.

D'autres défis concernent le fonctionnement de longue durée, l'abordabilité, la certification, la responsabilité, l'acceptation par les utilisateurs, la protection de la vie privée et le traitement des données. Les systèmes reposant sur des caméras ou des balayages tridimensionnels peuvent collecter des données sur le visage, le cuir chevelu ou la coiffure, ce qui ajoute des enjeux de confidentialité aux questions générales de sécurité.

Ces défis suggèrent plusieurs directions prometteuses de recherche en coupe de cheveux robotique :

- Exécution autonome de coupes de cheveux
- Coupe de cheveux téléopérée pour un contrôle expert à distance
- Systèmes d'autonomie partagée combinant supervision humaine et exécution robotique
- Planification de coupe à partir de coiffures cibles, de spécifications géométriques ou d'instructions utilisateur
- Modélisation 3D des cheveux et simulation physique pour la génération de coiffures cibles, la prévisualisation numérique et la validation de l'exécution robotique
- Perception en temps réel des cheveux, du cuir chevelu et de la pose de la tête pendant la coupe
- Compensation des mouvements de l'utilisateur et d'autres perturbations pendant l'opération
- Contrôle sensible à la sécurité pour opérer près de régions anatomiques sensibles
- Protocoles d'évaluation, méthodes de benchmark et conception orientée certification
- Intégration système orientée déploiement pour une utilisation fiable en conditions réelles

## Références

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

## Publications dans ce dépôt

Les publications suivantes sont mentionnées dans les sections ci-dessus et rassemblées dans ce dépôt.

### 2025

- [Haircutting Robots](publications/2025/LiHaircutting%20Robots.pdf)
- [Haircutting Robots from Theory to Practice](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf)
- [Safety in Robotic Haircutting](publications/2025/Safety_in_Robotic_Haircutting.pdf)

### 2026

- [CNC-Inspired Robotic Hair Cutting: A Comprehensive Survey on Precision Personal Care Automation](publications/2026/CNC_Inspired_Robotic_Hair_Cutting_A_Comprehensive_Survey_on_Precision_Personal_Care_Automation.pdf)
- [Robotic Haircutting Systems: A Survey of Methods, Challenges and Hair Modeling Insights](publications/2026/Robotic_Haircutting_Systems_A_Survey_of_Methods_Challenges_and_Hair_Modeling_Insights.pdf)
- [Vision-Language-Action Modules for Intelligent Haircutting Robots: A Position Paper on Architectures, Evaluation and Future Direction](publications/2026/Vision_Language_Action_Modules_for_Intelligent_Haircutting_Robots__A_Position_Paper_on_Architectures_Evaluation_and_Future_Direction.pdf)
