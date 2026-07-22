---
title: Ghost Ship
tab_title: 星空支线关卡：幽灵船
tag: Starfield Side Quest Level Design
type: 星空单人支线任务关卡设计
role: 关卡设计 / 剧情设计 / 环境叙事 / Gameplay 实现
time: 8 周 / 单人
status: 已完成 · Scrum 敏捷开发
caption: ▲ 通过环境叙事、多区域探索与解谜战斗营造废弃豪华星际邮轮的沉浸式冒险体验
hero: cover.jpg
hero_caption: 《Ghost Ship（幽灵船）》项目封面
---

## 一句话介绍

基于《Starfield》Creation Kit 独立设计并开发恐怖探索向单人任务关卡，通过环境叙事、多区域探索与解谜战斗，营造废弃豪华星际邮轮的沉浸式冒险体验。

## 游戏介绍

《星空（Starfield）》是 Bethesda Game Studios 开发的开放世界科幻 RPG。本项目基于官方 Creation Kit 制作，为游戏新增了一条可独立游玩的原创支线任务。

## 关卡介绍

《Ghost Ship（幽灵船）》是基于《星空（Starfield）》设计的一张单人支线任务关卡。玩家为调查失踪人员登上一艘失联的豪华星际邮轮，在探索过程中逐步恢复飞船供电、破解封锁区域、收集关键物资，并通过环境叙事揭开整艘飞船覆灭的真相，最终在货舱与未知生物展开决战。关卡融合探索、战斗、潜行、解谜与环境叙事，营造出类似《异形：隔离（Alien: Isolation）》的悬疑恐怖体验。

## 我的工作

### 1. 整体关卡设计（Level Layout & Progression）

负责整体关卡流程设计，将舰桥、客舱、船员区、活动区、货舱等多个功能区域串联为完整探索路线，通过供电恢复、钥匙收集、电池解谜等机制逐步解锁新区域，构建层层递进的探索节奏。

### 2. 环境叙事与氛围设计（Environmental Storytelling）

围绕废弃豪华星际邮轮设计整体世界观，通过尸体摆放、终端日志、场景细节、光照变化及空间破坏等环境叙事元素，引导玩家逐步推理事件真相，并营造《Alien》式悬疑恐怖氛围。

### 3. 探索、解谜与战斗设计（Gameplay Design）

设计恢复供电、钥匙探索、电池收集、通风管潜入、秘密房间等探索与解谜玩法，并配置 Xenogrub、Terrormorph 等敌人，使探索、解谜与战斗交替推进，持续提升关卡张力。

### 4. 关卡节奏设计（Pacing Design）

通过黑暗失重开场、供电恢复、自由探索、狭窄追逐、资源管理及最终 Boss 战等阶段，构建由探索逐步升级至高潮战斗的完整体验节奏。

## 时间线

阶段｜时间｜工作内容
Level Design Pitch｜2026.05.26｜完成关卡 Pitch，确定主题、美术风格、核心玩法、剧情框架与整体关卡流程。
Level Design Document｜2026.06.01｜完成 LDD，明确空间布局、探索流程、解谜机制、战斗配置及环境叙事设计。
Whitebox｜2026.06.08｜完成白盒搭建，验证空间布局、玩家流程、探索节奏与导航设计。
Initial Gameplay｜2026.06.22｜完成核心 Gameplay，实现探索、解谜、战斗、环境叙事及任务流程，并开展 Playtest。
Gameplay Complete｜2026.07.06｜完成全部关卡内容开发，持续根据测试反馈优化 Flow、战斗体验、恐怖氛围与环境叙事。
Aesthetics｜2026.07.13｜完成场景美术、灯光、材质与环境布置，强化豪华邮轮废墟的视觉表现与沉浸感。
RTM｜2026.07.19｜完成 Bug 修复、最终优化与项目交付。

## 测试迭代

问题｜解决方案｜结果
即使是恐怖关卡，没有武器对玩家来说也很难受，尤其是在《星空》中。｜在早期给玩家配备“电磁枪”武器。｜玩家在游戏早期获得短暂麻痹敌人的能力，在拥有对抗手段的同时，依然无法完全杀死敌人，没有削弱恐惧感。
船员区域过于空旷，动线不佳。｜对区域进行分割，在中心放置会议桌，周围设置一圈走廊，并在外层设置独立房间。｜形成复杂的回环结构，优化动线。
存档点设置在最终 Boss 战房间内部，导致无限死亡。｜在最终 Boss 战房间外放置安全屋。｜解决死档问题。

## 项目总结

### 项目亮点（What Went Well）

• 打造不同区域风格截然不同的星际邮轮关卡。
• 创造独特的恐怖游戏体验。
• 成功重用区域与路线。

### 优化方向（Even Better If）

• 作为邮轮，关卡规模可以适当增大，结构适当复杂化。
• 适当增加环境叙事内容。
• 优化室内空间路线大小，以适应大型怪物的移动路径。
• 增大 Boss 战区域，丰富单场战斗体验。

### 项目收获（What I Learned）

• 总结“将现实建筑化作关卡设计”的经验。

具体经验包括：

1. 获取现实参考：例如，邮轮关卡参考迪士尼邮轮官网平面图。
2. 适当简化结构：邮轮关卡不需要现实中的二十层大邮轮。
3. 优化游戏尺寸：优化房间层高、走廊宽度，以适应游戏人物大小与镜头风格；例如，第三人称镜头往往需要更大的室内空间。
4. 优化动线：现实建筑往往以安全、人流为准则设计动线，而关卡设计需要考虑心流、视线等因素。

## 附录

[查看 Ghost Ship 关卡设计文档（PDF）](pdfs/Ma _DFSI_LDD_01.pdf)
[查看 Ghost Ship RTM ReadMe（PDF）](pdfs/Ma_DFSI_ReadMe_ RTM.pdf)

![Figure 49：舰桥区域](images/bridgearea.jpg)

![Figure 50：船员区域 1](images/crewarea1.jpg)

![Figure 51：船员区域 2](images/crewarea2.jpg)

![Figure 52：船员区域 3](images/crewarea3.jpg)

![Figure 53：餐厅区域](images/diningarea.jpg)

![Figure 54：大厅区域](images/hallarea.jpg)

![Figure 55：厨房区域](images/kitchenarea.jpg)

![Figure 56：乘客区域 1](images/passengerarea1.jpg)

![Figure 57：乘客区域 2](images/passengerarea2.jpg)

![Figure 58：乘客区域 3](images/passengerarea3.jpg)

![Figure 59：乘客区域 4](images/passengerarea4.jpg)
