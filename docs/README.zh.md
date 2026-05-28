# 机器人理发

语言: [English](../README.md) | 中文 | [Suomi](README.fi.md) | [Deutsch](README.de.md) | [Français](README.fr.md)

本仓库提供一个关于机器人理发的百科式概览，涵盖其背景、历史、安全考量、应用、技术挑战和关键参考文献。相关论文在正文中按需引用，并汇总于本文末尾。仓库同时提供一份用于项目整体介绍的演讲幻灯片 [Haircutting Robot Introduction Slides](../haircutting_robot_introduction.pdf)，内容涵盖研究动机、既有工作、技术需求、安全问题、支撑技术与未来展望。

## 概述

机器人理发是指利用机器人系统辅助或执行理发任务。其范围包括修剪、剃须、发型整理以及其他相关护理活动。为这些任务设计的机器人平台通常被称为理发机器人。

这一领域处于机器人学、计算机视觉、运动规划、机器人操作、人机交互、通信、计算机图形学、虚拟现实、人工智能和触觉技术的交叉点。

与普通电动理发器或手动护理工具不同，机器人理发系统需要具备感知、规划和控制能力，使机器人能够相对于人的头部和头发定位切割或护理工具。这一任务在技术上具有挑战性，因为头发是可变形的、个体差异显著，而且操作区域靠近耳朵、眼睛、头皮和面部等敏感解剖部位。

现有系统从遥操作平台到更具自主性的概念系统不等。根据本仓库收录的 2025 年文献，尚无被描述为已广泛部署的完全商业化理发机器人，但研究原型和综述工作表明，该方向具备走向商业化的可行路径。

## 历史

### 早期自动理发装置

自动理发的设想早于现代机器人系统。1966 年，[Jean Gronier](#ref-gronier-1966) 的一项美国专利描述了一种通过程序控制来生成预定发型的自动理发机器。与现代机器人理发系统相比，它更适合被视为前机器人时代的自动化装置，因为它依赖机械结构和预设程序，而不是实时感知或自适应反馈。

之后的专利提出了更为集成的系统，将感知、机器人机构和用户界面结合起来，反映出向更典型机器人实现形式的转变，其中包括后来的 [Mubarak Aldabbah](#ref-aldabbah-2023) 专利。

### 相机辅助自助理发系统

另一条相关研究路线聚焦于帮助人们自己理发，而不是由机器人自主完成剪发。2014 年，[Futami、Terada 和 Tsukamoto](#ref-futami-2014) 提出了一种配备可移动相机的机器人系统，使用户能够在自助理发过程中从不同视角观察自己的头部。

### 机器人理发原型

在 2020 年代，若干公开演示和 DIY 原型使机器人理发概念受到更多关注。这些项目结合了机械驱动、传感和人工监督，但仍属于实验性演示，而不是经过验证或已商业部署的系统。这一区别也见于 [Shuai Li（2025）](../publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf)。

### 相关护发与造型机器人

一些学术系统研究了与理发相邻的任务，包括洗发、头皮按摩、刷发、梳发、解结以及前发造型。虽然这些系统未必直接执行剪发，但它们涉及许多相同的技术问题，包括可变形头发感知、富接触操作、路径规划、用户舒适性以及头部周围作业安全（[Ando 等，2013](#ref-ando-2013)；[Hughes 等，2021](#ref-hughes-2021)；[Dennler 等，2021](#ref-dennler-2021)；[Yoo 等，2024](#ref-yoo-2024)；[Kim 等，2025](#ref-kim-2025)）。

相关例子包括洗头与头部护理机器人、基于反馈的头发解结系统、机器人梳发平台、如 MOE-Hair 这样的软体头发操作系统，以及基于发根中心调整的前发造型机器人。

### 数字发型建模与仿真系统

除实体机器人系统外，数字发型建模与仿真工具也为机器人理发提供了重要参考。[Digital Salon](#ref-he-2025-digital-salon) 是一个结合 AI 与物理驱动的 3D 头发生成、交互式修饰、实时仿真和图像渲染系统。它支持通过自然语言生成目标发型，并允许用户在三维环境中对发型进行细化和仿真。虽然该系统本身并不执行真实剪发操作，但它展示了如何将用户语言、目标发型设定、发丝级建模、交互编辑和视觉预览整合到统一流程中。因此，它与机器人理发中的目标发型表示、基于仿真的验证以及人机交互界面密切相关。

### 学术发展

进入 2020 年代后，机器人理发开始被视为服务机器人和个人护理自动化中的一个独立研究主题。早期的专著和综述将理发描述为一个多学科工程问题，涉及感知、可变形物体建模、运动规划、控制、遥操作、人机交互和安全。这些工作也强调了在人体头部附近作业的困难，包括头发几何形态的不确定性、不同用户之间的差异，以及对紧密集成的感知-规划-控制流程的需求。同时，它们提出了更广泛的概念化视角，例如将机器人理发视为类似 CNC 的过程模型，或视为在关键区域周围带有安全约束的移动机器人覆盖任务（[Li，2025](../publications/2025/Haircutting_Robots.pdf)；[Shuai Li，2025](../publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf)；[Khan 和 Li，2026a](../publications/2026/CNC_Inspired_Robotic_Hair_Cutting_A_Comprehensive_Survey_on_Precision_Personal_Care_Automation.pdf)；[Khan 和 Li，2026b](../publications/2026/Robotic_Haircutting_Systems_A_Survey_of_Methods_Challenges_and_Hair_Modeling_Insights.pdf)）。

较新的工作还将机器人理发与视觉-语言-动作架构联系起来，用这一领域作为讨论更高层次系统智能、评测和部署策略的具体场景（[Khan 和 Li，2026c](../publications/2026/Vision_Language_Action_Modules_for_Intelligent_Haircutting_Robots__A_Position_Paper_on_Architectures_Evaluation_and_Future_Direction.pdf)）。

### AI 生成的机器人理发视频

从 2025 年末开始，生成式 AI 视频工具推动了一波虚构的机器人理发视频在网上传播。这些视频展示了人形机器人理发师、多机械臂工作站以及头盔式自动理发设备。虽然这些内容是虚构的，但它们提高了公众认知，也反映出社会对自动化个人护理的兴趣上升。

## 安全

安全是机器人理发中的核心问题，因为机器人需要在人的头部附近操作，并使用推剪、剪刀、剃刀、吹风设备或加热造型工具等器具。相关风险包括感知错误、头部意外移动、接触力过大、工具过热、切割工具错位、标定故障、遥操作中的通信延迟，以及软件或控制失效。

常见的安全措施包括工作空间限制、速度和加速度约束、力或压力阈值、柔顺机构、软包覆或软末端执行器、急停功能、近距离监测、冗余传感，以及在检测到不安全状态时自动中断操作。

目前尚不存在专门针对机器人理发的国际安全标准。不过，一些现有标准可为风险分析和系统设计提供有价值的参考，尤其包括 [ISO 13482](#ref-iso-13482)、[ISO/TS 15066](#ref-iso-ts-15066)、[ISO 10218-1](#ref-iso-10218-1) 和 [ISO 14971](#ref-iso-14971)。与机器人理发相关的危险类别、缓解策略以及这些标准对具体风险分析的意义，可参见 [Shuai Li（2025）](../publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf) 和一篇 [2025 年安全综述](../publications/2025/Safety_in_Robotic_Haircutting.pdf)。

## 挑战与研究方向

主要挑战包括对头发和头皮的可靠感知、对多样化发质的建模、对用户移动的补偿、安全工具轨迹的规划、维持合适的工具距离和接触力，以及在耳朵、眼睛、面部和头皮等敏感区域周围作业。

头发尤其难以处理，因为它是可变形的、以发丝为基础的，并且在长度、密度、卷曲模式、刚度和湿度等方面高度多样。即使几何精度很高，审美评价仍然困难，因为理发质量还取决于风格偏好、对称性、舒适度和用户预期。

其他挑战还包括长时间运行、成本可负担性、认证、责任归属、用户接受度、隐私和数据处理。依赖摄像头或三维扫描的系统可能会采集面部、头皮或发型数据，因此除一般安全问题外，还会引入隐私问题。

这些挑战指向了若干值得进一步推进的机器人理发研究方向：

- 自主理发执行
- 面向远程专家控制的遥操作理发系统
- 将人工监督与机器人执行结合起来的共享自主系统
- 基于目标发型、几何规格或用户指令的理发规划
- 面向目标发型生成、数字预演和机器人执行验证的 3D 头发建模与物理仿真
- 剪发过程中的头发、头皮与头部姿态实时感知
- 对用户运动及其他扰动的在线补偿
- 面向敏感解剖区域作业的安全感知控制
- 评测协议、基准测试方法以及面向认证的系统设计
- 面向真实场景可靠应用的部署导向系统集成

## 进行中的工作

除本仓库收录的论文外，本团队正在通过以下公开项目开发远程遥操作理发机器人系统：

- [Client_RHCR](https://github.com/Dai0731csc/Client_RHCR)：一个面向远程遥操作机器人理发的客户端系统，支持浏览器端感知、标定、通信与原始位姿流传输。欢迎对这一方向感兴趣的研究者和开发者参与贡献。

本团队的其他持续性工作已整理在 [../ongoing-work/README.md](../ongoing-work/README.md) 中。

## 教学与培训

除研究论文和实现工作外，本仓库还收录了与机器人理发相关的教学与培训材料。这些内容已整理在 [../education/README.md](../education/README.md) 中。

- [Capstone Weekly Planning 2026](../education/Capstone%20Weekly%20Planning_2026.pdf)：用于学生培训与项目参与的课程项目规划文档。

## Fork 的参考项目

与本方向相关的 fork 开源项目已按类别整理在 [../related-projects/README.md](../related-projects/README.md) 中。该索引可作为与更广泛机器人理发研究相关技术基础的可扩展参考。

## 参考文献

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

## 团队论文

本项目由[奥卢大学李帅教授](https://www.oulu.fi/en/researchers/shuai-li)带领，目前专注于理发机器人相关的研究。发表的相关论文已在上文相关部分提及，并收录在本仓库中。具体列举如下：

### 2025

- [Haircutting Robots](../publications/2025/Haircutting_Robots.pdf)
- [Haircutting Robots from Theory to Practice](../publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf)
- [Safety in Robotic Haircutting](../publications/2025/Safety_in_Robotic_Haircutting.pdf)

### 2026

- [CNC-Inspired Robotic Hair Cutting: A Comprehensive Survey on Precision Personal Care Automation](../publications/2026/CNC_Inspired_Robotic_Hair_Cutting_A_Comprehensive_Survey_on_Precision_Personal_Care_Automation.pdf)
- [Robotic Haircutting Systems: A Survey of Methods, Challenges and Hair Modeling Insights](../publications/2026/Robotic_Haircutting_Systems_A_Survey_of_Methods_Challenges_and_Hair_Modeling_Insights.pdf)
- [Vision-Language-Action Modules for Intelligent Haircutting Robots: A Position Paper on Architectures, Evaluation and Future Direction](../publications/2026/Vision_Language_Action_Modules_for_Intelligent_Haircutting_Robots__A_Position_Paper_on_Architectures_Evaluation_and_Future_Direction.pdf)
