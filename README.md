# Robotic Haircutting

Languages: English | [中文](README.zh.md) | [Suomi](README.fi.md) | [Deutsch](README.de.md) | [Français](README.fr.md)

This repository serves primarily as an encyclopedia-style overview of robotic haircutting, covering background, history, safety, applications, challenges, and references. Relevant publications collected in this repository are cited where appropriate and listed together at the end.

## Overview

Robotic haircutting refers to the use of robotic systems to assist with or fully perform haircutting operations. Its scope can include trimming, shaving, hairstyling, and related grooming tasks. Robotic platforms designed for these tasks are commonly described as haircutting robots.

The field sits at the intersection of robotics, computer vision, motion planning, manipulation, human-robot interaction, communication, computer graphics, virtual reality, artificial intelligence, and haptics.

Unlike ordinary electric clippers or manually operated grooming tools, robotic haircutting systems require sensing, planning, and control capabilities that allow a robot to position a cutting or grooming tool relative to the human head and hair. This is technically difficult because hair is deformable, highly variable across individuals, and manipulated near sensitive anatomical regions such as the ears, eyes, scalp, and face.

Systems range from teleoperated platforms to more autonomous concepts. As of 2025, no fully commercial haircutting robot is widely deployed, but research prototypes and surveys suggest a plausible path toward commercialization.

## History

### Early Automated Haircutting Devices

Ideas for automated haircutting appeared well before modern robotic systems. A 1966 United States patent by [Jean Gronier](#ref-gronier-1966) described an automatic hair-cutting machine using programmed control to produce a predetermined style. It is better understood as pre-robotic automation than as a modern robotic haircutting system, because it relied on mechanical structure and predefined programs rather than real-time sensing or adaptive feedback.

Later patents proposed more integrated systems combining sensing, robotic mechanisms, and user interfaces, indicating a shift toward more recognizably robotic implementations, including the later patent by [Mubarak Aldabbah](#ref-aldabbah-2023).

### Camera-Assisted Self-Haircut Systems

A related direction focused on helping people cut their own hair rather than having a robot cut it autonomously. In 2014, [Futami, Terada, and Tsukamoto](#ref-futami-2014) proposed a camera-equipped movable robot system that let users inspect their head from different viewpoints while performing a self-haircut.

### Robotic Haircutting Prototypes

In the 2020s, several public demonstrations and do-it-yourself prototypes brought attention to robotic haircutting concepts. These projects combined mechanical actuation, sensing, and user supervision, but they were generally experimental demonstrations rather than validated or commercially deployed systems, a distinction also discussed in [Shuai Li (2025)](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf).

### Related Hair-Care and Hairstyling Robots

Several academic systems studied tasks adjacent to haircutting, including shampooing, scalp massage, brushing, combing, detangling, and front-hair styling. These systems do not necessarily perform cutting, but they address many of the same technical issues, including deformable-hair perception, contact-rich manipulation, path planning, user comfort, and safety around the head ([Ando et al., 2013](#ref-ando-2013); [Hughes et al., 2021](#ref-hughes-2021); [Dennler et al., 2021](#ref-dennler-2021); [Yoo et al., 2024](#ref-yoo-2024); [Kim et al., 2025](#ref-kim-2025)).

Examples include hair-washing and head-care robots, feedback-driven detangling systems, robotic hair-combing platforms, soft robotic hair-manipulation systems such as MOE-Hair, and front-hair styling robots based on root-centric strand adjustment.

### Digital Hairstyle Modeling and Simulation Systems

In addition to physical robotic systems, digital hairstyle modeling and simulation tools also provide important references for robotic haircutting. [Digital Salon](#ref-he-2025-digital-salon) is an AI- and physics-driven system for 3D hair generation, interactive grooming, real-time simulation, and image rendering. It supports natural-language generation of target hairstyles and allows users to refine and dynamically simulate hairstyles in a three-dimensional environment. Although the system does not perform physical haircutting, it demonstrates how user language, target hairstyles, strand-level modeling, interactive editing, and visual preview can be integrated into a unified workflow, making it a relevant technical basis for target hairstyle representation, simulation-based validation, and human-robot interaction interfaces in robotic haircutting.

### Academic Development

In the 2020s, robotic haircutting began to be framed as a distinct research topic in service robotics and personal-care automation. Early monograph and survey treatments described haircutting as a multidisciplinary engineering problem involving perception, deformable object modeling, motion planning, control, teleoperation, human-robot interaction, and safety. This work also emphasized the difficulty of operating near the human head, including uncertainty in hair geometry, user-to-user variability, and the need for tightly integrated perception-planning-control pipelines, while introducing broader conceptual framings such as robotic haircutting as a CNC-like process and as a mobile-robotics-style coverage task with safety constraints around critical regions ([Li, 2025](publications/2025/LiHaircutting%20Robots.pdf); [Shuai Li, 2025](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf); [Khan and Li, 2026a](publications/2026/CNC_Inspired_Robotic_Hair_Cutting_A_Comprehensive_Survey_on_Precision_Personal_Care_Automation.pdf); [Khan and Li, 2026b](publications/2026/Robotic_Haircutting_Systems_A_Survey_of_Methods_Challenges_and_Hair_Modeling_Insights.pdf)).

More recent work has also connected robotic haircutting to vision-language-action architectures, using the field as a concrete setting for discussing higher-level system intelligence, evaluation, and deployment strategy ([Khan and Li, 2026c](publications/2026/Vision_Language_Action_Modules_for_Intelligent_Haircutting_Robots__A_Position_Paper_on_Architectures_Evaluation_and_Future_Direction.pdf)).

### AI-Generated Robotic Haircutting Videos

From late 2025 onward, generative AI video tools contributed to a wave of fictional robotic haircutting videos online. These depicted humanoid robot barbers, multi-arm workstations, and helmet-style automatic haircutting devices. Although fictional, they increased public awareness and reflected growing interest in automated personal care.

## Safety

Safety is central to robotic haircutting because the robot operates near the human head while using tools such as clippers, scissors, razors, dryers, or heated styling devices. Relevant hazards include perception errors, unexpected head movement, excessive contact force, tool overheating, cutting-tool misalignment, calibration faults, communication delay in teleoperation, and software or control failures.

Proposed safety measures include workspace limits, speed and acceleration constraints, force or pressure thresholds, compliant mechanisms, soft covers or end-effectors, emergency stop functions, proximity monitoring, redundant sensing, and automatic interruption when unsafe conditions are detected.

No international safety standard exists specifically for robotic haircutting. However, several existing standards are relevant as reference points for risk analysis and system design, especially [ISO 13482](#ref-iso-13482), [ISO/TS 15066](#ref-iso-ts-15066), [ISO 10218-1](#ref-iso-10218-1), and [ISO 14971](#ref-iso-14971). Hazard categories, mitigation strategies, and the relevance of these standards to haircutting-specific risk analysis are discussed in [Shuai Li (2025)](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf) and a [2025 safety review](publications/2025/Safety_in_Robotic_Haircutting.pdf).

## Challenges and Research Directions

Major challenges include reliable perception of hair and scalp, modeling diverse hair types, compensating for user movement, planning safe tool trajectories, maintaining appropriate tool distance and contact force, and operating around sensitive regions such as the ears, eyes, face, and scalp.

Hair is especially difficult to manipulate because it is deformable, strand-based, and highly variable in length, density, curl pattern, stiffness, and moisture. Even when geometric precision is high, aesthetic evaluation remains difficult because haircut quality also depends on style preference, symmetry, comfort, and user expectation.

Additional challenges include long-duration operation, affordability, certification, liability, user acceptance, privacy, and data handling. Systems that rely on cameras or three-dimensional scanning may collect facial, scalp, or hairstyle data, which introduces privacy concerns in addition to ordinary safety concerns.

These challenges point toward several promising research directions in robotic haircutting:

- Autonomous haircut execution
- Teleoperated haircutting for remote expert control
- Shared-autonomy systems that combine human supervision with robotic execution
- Haircut planning from target styles, geometric specifications, or user instructions
- 3D hair modeling and physical simulation for target hairstyle generation, digital preview, and robot-execution validation
- Real-time perception of hair, scalp, and head pose during cutting
- Compensation for user motion and other disturbances during operation
- Safety-aware control for operation near sensitive anatomical regions
- Evaluation protocols, benchmarking methods, and certification-oriented system design
- Deployment-oriented system integration for reliable real-world use

## References

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

## Team Publications

The following publications are cited throughout the sections above and collected in this repository.

### 2025

- [Haircutting Robots](publications/2025/LiHaircutting%20Robots.pdf)
- [Haircutting Robots from Theory to Practice](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf)
- [Safety in Robotic Haircutting](publications/2025/Safety_in_Robotic_Haircutting.pdf)

### 2026

- [CNC-Inspired Robotic Hair Cutting: A Comprehensive Survey on Precision Personal Care Automation](publications/2026/CNC_Inspired_Robotic_Hair_Cutting_A_Comprehensive_Survey_on_Precision_Personal_Care_Automation.pdf)
- [Robotic Haircutting Systems: A Survey of Methods, Challenges and Hair Modeling Insights](publications/2026/Robotic_Haircutting_Systems_A_Survey_of_Methods_Challenges_and_Hair_Modeling_Insights.pdf)
- [Vision-Language-Action Modules for Intelligent Haircutting Robots: A Position Paper on Architectures, Evaluation and Future Direction](publications/2026/Vision_Language_Action_Modules_for_Intelligent_Haircutting_Robots__A_Position_Paper_on_Architectures_Evaluation_and_Future_Direction.pdf)
