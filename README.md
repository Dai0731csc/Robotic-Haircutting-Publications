# Robotic Haircutting Publications

This repository collects publications and background notes related to robotic haircutting.

## Our Team's Work

This repository highlights our team's research contributions on robotic haircutting, including foundational studies, safety-oriented work, system surveys, and forward-looking position papers.

[Jump to Publications](#publications)

Featured topics include:

- Haircutting robot foundations and theory
- Safety in robotic haircutting
- System-level surveys and technical challenges
- Vision-language-action directions for intelligent haircutting robots

## Publications

### 2025

- [Haircutting Robots from Theory to Practice](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf)
- [Li Haircutting Robots](publications/2025/LiHaircutting%20Robots.pdf)
- [Safety in Robotic Haircutting](publications/2025/Safety_in_Robotic_Haircutting.pdf)

### 2026

- [CNC-Inspired Robotic Hair Cutting: A Comprehensive Survey on Precision Personal Care Automation](publications/2026/CNC_Inspired_Robotic_Hair_Cutting_A_Comprehensive_Survey_on_Precision_Personal_Care_Automation.pdf)
- [Robotic Haircutting Systems: A Survey of Methods, Challenges and Hair Modeling Insights](publications/2026/Robotic_Haircutting_Systems_A_Survey_of_Methods_Challenges_and_Hair_Modeling_Insights.pdf)
- [Vision-Language-Action Modules for Intelligent Haircutting Robots: A Position Paper on Architectures, Evaluation and Future Direction](publications/2026/Vision_Language_Action_Modules_for_Intelligent_Haircutting_Robots__A_Position_Paper_on_Architectures_Evaluation_and_Future_Direction.pdf)

## Overview

Robotic haircutting refers to the use of robotic systems to assist with or fully perform haircutting operations. Its scope can include trimming, shaving, hairstyling, and related grooming tasks. Robotic platforms designed for these tasks are commonly described as haircutting robots.

The field sits at the intersection of robotics, computer vision, motion planning, manipulation, human-robot interaction, communication, computer graphics, virtual reality, artificial intelligence, and haptics.

Unlike ordinary electric clippers or manually operated grooming tools, robotic haircutting systems require sensing, planning, and control capabilities that allow a robot to position a cutting or grooming tool relative to the human head and hair. This is technically difficult because hair is deformable, highly variable across individuals, and manipulated near sensitive anatomical regions such as the ears, eyes, scalp, and face.

Systems range from teleoperated platforms to more autonomous concepts. As of 2025, no fully commercial haircutting robot is widely deployed, but research prototypes and surveys suggest a plausible path toward commercialization.

## History

### Early Automated Haircutting Devices

Ideas for automated haircutting appeared well before modern robotic systems. A 1966 United States patent by Jean Gronier described an automatic hair-cutting machine using programmed control to produce a predetermined style. It is better understood as pre-robotic automation than as a modern robotic haircutting system, because it relied on mechanical structure and predefined programs rather than real-time sensing or adaptive feedback.

Later patents proposed more integrated systems combining sensing, robotic mechanisms, and user interfaces, indicating a shift toward more recognizably robotic implementations.

### Camera-Assisted Self-Haircut Systems

A related direction focused on helping people cut their own hair rather than having a robot cut it autonomously. In 2014, Futami, Terada, and Tsukamoto proposed a camera-equipped movable robot system that let users inspect their head from different viewpoints while performing a self-haircut.

### Robotic Haircutting Prototypes

In the 2020s, several public demonstrations and do-it-yourself prototypes brought attention to robotic haircutting concepts. These projects combined mechanical actuation, sensing, and user supervision, but they were generally experimental demonstrations rather than validated or commercially deployed systems.

### Related Hair-Care and Hairstyling Robots

Several academic systems studied tasks adjacent to haircutting, including shampooing, scalp massage, brushing, combing, detangling, and front-hair styling. These systems do not necessarily perform cutting, but they address many of the same technical issues, including deformable-hair perception, contact-rich manipulation, path planning, user comfort, and safety around the head.

Examples include hair-washing and head-care robots, feedback-driven detangling systems, robotic hair-combing platforms, soft robotic hair-manipulation systems such as MOE-Hair, and front-hair styling robots based on root-centric strand adjustment.

### Academic Development

In the 2020s, robotic haircutting began to be framed as a distinct research topic in service robotics and personal-care automation. Early academic work, including a 2025 monograph and related review papers, treated haircutting as a multidisciplinary engineering problem involving perception, deformable object modeling, motion planning, control, teleoperation, human-robot interaction, and safety.

This body of work emphasized the difficulty of operating near the human head, including uncertainty in hair geometry, user-to-user variability, and the need for tightly integrated perception-planning-control pipelines. It also introduced broader conceptual framings, including robotic haircutting as a CNC-like process and as a mobile-robotics-style coverage task with safety constraints around critical regions.

### AI-Generated Robotic Haircutting Videos

From late 2025 onward, generative AI video tools contributed to a wave of fictional robotic haircutting videos online. These depicted humanoid robot barbers, multi-arm workstations, and helmet-style automatic haircutting devices. Although fictional, they increased public awareness and reflected growing interest in automated personal care.

## Safety

Safety is central to robotic haircutting because the robot operates near the human head while using tools such as clippers, scissors, razors, dryers, or heated styling devices. Relevant hazards include perception errors, unexpected head movement, excessive contact force, tool overheating, cutting-tool misalignment, calibration faults, communication delay in teleoperation, and software or control failures.

Proposed safety measures include workspace limits, speed and acceleration constraints, force or pressure thresholds, compliant mechanisms, soft covers or end-effectors, emergency stop functions, proximity monitoring, redundant sensing, and automatic interruption when unsafe conditions are detected.

No international safety standard exists specifically for robotic haircutting. However, several existing standards are relevant as reference points for risk analysis and system design, especially ISO 13482, ISO/TS 15066, ISO 10218-1, and ISO 14971.

## Applications

Potential applications include:

- Professional salon assistance
- Supervised self-service haircutting
- Home grooming
- Assistive grooming for elderly or disabled users
- Remote, institutional, or healthcare-related grooming services

Related hair-care robots may also support non-cutting tasks such as brushing, combing, shampooing, scalp massage, and hairstyling. Most reported applications remain experimental, proposed, or prototype-level rather than validated consumer services.

## Challenges

Major challenges include reliable perception of hair and scalp, modeling diverse hair types, compensating for user movement, planning safe tool trajectories, maintaining appropriate tool distance and contact force, and operating around sensitive regions such as the ears, eyes, face, and scalp.

Hair is especially difficult to manipulate because it is deformable, strand-based, and highly variable in length, density, curl pattern, stiffness, and moisture. Even when geometric precision is high, aesthetic evaluation remains difficult because haircut quality also depends on style preference, symmetry, comfort, and user expectation.

Additional challenges include long-duration operation, affordability, certification, liability, user acceptance, privacy, and data handling. Systems that rely on cameras or three-dimensional scanning may collect facial, scalp, or hairstyle data, which introduces privacy concerns in addition to ordinary safety concerns.

## References

- Jean Gronier. *Automatic hair-cutting machine having programmed control means for cutting hair in a predetermined style*. US Patent 3241562A, 1966.
- Mubarak Aldabbah. *Automatic hair cutter robot*. WO Patent 2023080812A1, 2023.
- Kyosuke Futami, Tsutomu Terada, and Masahiko Tsukamoto. *A System for Supporting Self-Haircuts Using Camera Equipped Robot*. MoMM, 2014.
- Takeshi Ando et al. *Biosignal-based relaxation evaluation of head-care robot*. EMBC, 2013.
- Josie Hughes et al. *Detangling hair using feedback-driven robotic brushing*. RoboSoft, 2021.
- Nathaniel Dennler, Eura Shin, Maja Mataric, and Stefanos Nikolaidis. *Design and Evaluation of a Hair Combing System Using a General-Purpose Robotic Arm*. IROS, 2021.
- Uksang Yoo et al. *MOE-Hair: Toward Soft and Compliant Contact-rich Hair Manipulation and Care*. HRI Companion, 2024.
- Soonhyo Kim et al. *Front Hair Styling Robot System Using Path Planning for Root-Centric Strand Adjustment*. SII, 2025.
- Shuai Li. [*Haircutting Robots: From Theory to Practice*](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf). Automation, 2025.
- Steven Li. [*Haircutting Robots*](publications/2025/LiHaircutting%20Robots.pdf). Springer, 2025.
- [*Safety in Robotic Haircutting*](publications/2025/Safety_in_Robotic_Haircutting.pdf).
- Ameer Tamoor Khan and Shuai Li. [*Robotic Haircutting Systems: A Survey of Methods, Challenges, and Hair Modeling Insights*](publications/2026/Robotic_Haircutting_Systems_A_Survey_of_Methods_Challenges_and_Hair_Modeling_Insights.pdf). IEEE Journal of Selected Areas in Sensors, 2026.
- Ameer Tamoor Khan and Shuai Li. [*CNC-Inspired Robotic Hair Cutting: A Comprehensive Survey on Precision Personal Care Automation*](publications/2026/CNC_Inspired_Robotic_Hair_Cutting_A_Comprehensive_Survey_on_Precision_Personal_Care_Automation.pdf). 2026.
- Ameer Tamoor Khan and Shuai Li. [*Vision-Language-Action Models for Intelligent Haircutting Robots: A Position Paper on Architectures, Evaluation, and Future Directions*](publications/2026/Vision_Language_Action_Modules_for_Intelligent_Haircutting_Robots__A_Position_Paper_on_Architectures_Evaluation_and_Future_Direction.pdf). 2026.
- ISO 13482. *Robots and robotic devices - Safety requirements for personal care robots*.
- ISO/TS 15066. *Robots and robotic devices - Collaborative robots*.
- ISO 10218-1. *Robotics - Safety requirements for industrial robots - Part 1: Robots*.
- ISO 14971. *Medical devices - Application of risk management to medical devices*.
