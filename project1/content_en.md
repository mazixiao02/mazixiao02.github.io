---
title: Decaran: Become Human
tab_title: Starfield Side Quest: Decaran: Become Human
tag: Starfield Side Quest Level Design
type: Starfield Single-Player Side-Quest Level
role: Level Design / Quest Design / Gameplay Implementation
time: 10 Weeks / Solo / Approx. 300 Hours
status: Completed
caption: ▲ A complete side-quest level independently developed from spatial planning and quest structure through scripting and iteration
hero: images/hero.jpg
hero_caption: Decaran: Become Human — Project Key Visual
---

## One-Sentence Overview

An original Starfield side quest built around a central hub, a three-stage investigation, and a morally ambiguous choice; I used the Creation Kit to independently deliver approximately 18 minutes of exploration, combat, puzzles, dialogue, and two endings across interior and exterior spaces.

## Project Overview

Role｜Level Design / Quest Design / Gameplay Implementation
Development｜10 Weeks / Solo / Approx. 300 Hours
Scope｜4 Exterior Spaces / 7 Interior Spaces
Playtime｜Approx. 18 Minutes / Two Endings
Tools｜Starfield Creation Kit / Papyrus

The player is hired to investigate a robot uprising at the automated Decaran III factory. Inside, they gather evidence across distinct functional zones, activate three terminals, and progressively unlock the core area. They eventually discover that their guide, R6D7, orchestrated the awakening. The player must choose between restoring production and freeing the robots, then face the consequences.

Quest Phase｜Player Action｜Design Purpose
Establish Mystery｜Investigate the exterior and meet workers, doctors, mercenaries, and R6D7｜Frame the conflict through competing perspectives
Advance Investigation｜Enter the factory and explore three zones around the central hall｜Alternate exploration, combat, puzzles, and information reveals
Reveal the Truth｜Ride the elevator to the rooftop office and learn R6D7's identity｜Reframe the mission and the player's relationship with their guide
Final Choice｜Return to the central hall, complete the final battle, and decide the factory's fate｜Bring earlier characters, information, and consequences together

![Level overview: the exterior industrial park, factory, and vertical tower form one complete quest space](images/level-overview.jpg)

@[youtube](lieJnrhMxWs "Decaran: Become Human — Full Gameplay Walkthrough")

## Design Goals

1. Preserve exploration freedom while keeping the player's current objective and global position readable.
2. Integrate combat, puzzles, narrative information, and spatial progression instead of treating them as separate layers.
3. Give both endings meaningful benefits and costs rather than presenting a simple good-versus-evil choice.

## 01｜Organizing Three-Stage Exploration Around a Central Hall

The factory interior uses a hub structure composed of a central hall and three objective zones. On first entering the hall, the player can see the locked central elevator and its three status indicators, establishing the long-term objective before exploration begins. The player then clears the surrounding zones, completes combat and terminal interactions, and repeatedly returns to confirm progress.

The hall is more than a corridor. It serves as a navigational anchor, progress display, combat arena, and final confrontation space. Enemy states, quest progress, and accessible routes change between visits, turning spatial reuse into part of the quest rhythm.

![Central hall: the elevator presents the long-term objective while the surrounding space connects three quest zones](images/central-hub.jpg)

Design Goal｜Maintain orientation during nonlinear exploration
Method｜Visible long-term objective / Central hub / Functional zoning / Return loops
Outcome｜Converted an underused hall into the quest's navigational, progression, combat, and narrative core

## 02｜Connecting Interaction and Outcome Through Sightlines

In the initial version, the player activated three terminals to unlock the central elevator, but the terminals and elevator were visually separated. After interacting, the player had to rely on quest text to understand progress and could not see what their action had changed.

I reoriented the terminals and added observation windows so the player could directly see the corresponding elevator light and lock state change. Visible cables connected each terminal to its target device, reinforcing the causal relationship. This iteration transformed text-dependent feedback into spatial feedback that players could observe and understand in the environment.

![Interior route: three objective zones branch from the central hall and converge on the elevator](images/interior-route.jpg)

## 03｜Building Combat Escalation Through Space and Enemy Composition

Melee assault robots and ranged units create complementary threats, while encounter spaces expand from compact rooms to an open hall and vertical traversal areas. Players must continually reconsider sightlines, elevation, cover, and target priority instead of repeating a single clearing strategy.

The Novablast EMP rifle adds a control option by temporarily incapacitating robots. Early encounters teach the stun behavior, the middle section combines melee and ranged enemies across two levels, and the final battle reuses the familiar central hall to test movement, target selection, and spatial knowledge together.

Stage｜Space and Enemies｜Player Decision
Early Tutorial｜Compact room / Single threat｜Learn the EMP stun and establish the basic combat rule
Mid-Quest Combination｜Two-level hall / Melee + ranged robots｜Use elevation and cover to prioritize targets
Final Battle｜Reused central hall / R6D7 and robot reinforcements｜Combine weapons, movement, and route knowledge in familiar space

![The vertical shaft changes traversal rhythm through lasers, elevation, and a return loop](images/vertical-shaft.jpg)

## 04｜Making the Final Choice Change Characters and World State

I did not want “free the robots” to be an automatically correct answer, so both branches carry benefits and costs. Doctors, workers, mercenaries, and robots encountered earlier each present a different stake in the conflict, grounding the final decision in information and relationships accumulated throughout the quest.

Final Choice｜Immediate Result｜Consequences
Destroy R6D7 and restore production｜The robots are suppressed and the factory resumes operation｜Relations with the corporation and mercenaries improve, medicine production resumes, and the human patient survives
Free the awakened robots｜The robots gain freedom and the factory shuts down｜The corporation and mercenaries become hostile, medicine supplies stop, and the human patient dies

![The rooftop office uses sunset, long views, and elevation to stage the truth reveal](images/rooftop-reveal.jpg)

![The final conversation with R6D7 consolidates the quest's information into a consequential choice](images/final-choice.jpg)

## Gameplay and Quest Implementation

I used the Creation Kit to build spaces, configure enemies, create objectives, author NPC dialogue, and manage level states. Papyrus scripts and Quest Stages control locks, terminals, factions, character behavior, final-battle triggers, and both endings. Aliases manage critical actors and quest objects so state remains consistent across locations.

Implementation Area｜Delivered Content
Quest Flow｜Objective updates / Quest Stages / Dialogue conditions / Two endings
Spatial State｜Locks / Elevator / Three terminals / Hidden entrances
Characters and Combat｜NPC behavior / Faction hostility / Combat triggers / Boss battle
Player Feedback｜Quest text / Signal lights / Observation windows / Cable guidance

## Playtesting and Iteration

Finding｜Design Diagnosis｜Change｜Observed Result
Players could not tell what a terminal changed｜The interaction and feedback target lacked a spatial relationship｜Reoriented terminals and added windows that reveal the elevator state change｜Players could understand the terminal–elevator relationship without relying on quest text
The full laser-platforming section demanded precise aerial control that did not fit Starfield's movement｜Difficulty came from control limitations rather than meaningful spatial decisions｜Reduced the platforming and retained lasers as local hazards and spatial constraints｜Reduced flow interruptions while preserving the vertical area's visual identity and movement variation
The initial hall was large but functioned mainly as a passage｜A high-cost core space was not contributing enough to progression｜Converted it into a hub revisited throughout the quest and reused for the final battle｜The hall now supports navigation, progress feedback, combat, and narrative

## Timeline

Level Design Pitch｜2026.02.20｜Established the theme, core gameplay, narrative framework, and development direction
Level Design Document｜2026.02.26｜Completed the LDD and defined flow, spatial layout, quest structure, and combat design
Whitebox｜2026.03.09｜Validated spatial layout, player flow, and pacing
Initial Gameplay｜2026.03.29｜Implemented core gameplay, quest scripts, and combat to produce a complete playable flow
Gameplay Complete｜2026.04.18｜Completed all level content and refined navigation, combat, and quest experience
Aesthetics｜2026.04.26｜Completed environment art, lighting, and presentation
RTM｜2026.05.03｜Completed final polish, bug fixing, and delivery

## Project Retrospective

What Went Well
• Independently completed an approximately 18-minute side quest containing interior and exterior exploration, combat, puzzles, NPC dialogue, and two endings.
• Organized progression through a central hub and three functional zones, using spatial feedback to improve objective readability.
• Implemented complete quest states, character behavior, and ending branches with the Creation Kit and Papyrus.

Even Better If
• The exterior supports less gameplay than the interior; future whitebox testing should validate content density across every major zone earlier.
• Combat difficulty and enemy combinations received insufficient focused testing; future projects should include encounter-specific sessions in addition to full-flow playtests.
• Too much early development time went into platforming that did not fully match the base movement model; mechanic-to-controller fit should be validated earlier.

What I Learned
• A quest level is not a simple sum of space, narrative, and combat. Objectives, routes, information, and system feedback must work together to support the player's current understanding and decisions. Adding more content matters less than giving every space a clear function and allowing players to read the consequences of their actions from the environment itself.

## Attachments

[📄 View LDD｜Complete Level Design Document](pdfs/MaZ_DecaranBecomeHuman_LDD.pdf)

[📄 View ReadMe｜Setup and Play Instructions](pdfs/MaZ_DecaranBecomeHuman_ReadMe.pdf)

[📄 View Portfolio｜Project Design Summary](pdfs/MaZ_SF_DecaranBecomeHuman_Portfolio.pdf)
