---
title: Hamsterballin’
tab_title: UE5 Multiplayer Racing: Hamsterballin’
tag: Unreal Engine 5
type: 3D / Local Multiplayer / Racing / Mario Kart-like
role: Final Level / Cableway System / Camera Design
time: 12 Weeks / 42-Person Team
status: Steam Store Page Live
status_url: https://store.steampowered.com/app/4319370/Hamsterballin/
status_link: View Steam Store Page
caption: ▲ Iterating on navigation, route choice, and spectacle within a high-speed racing experience
hero: images/hero.jpg
hero_caption: Hamsterballin’ — Gacha Galaxy Final Level Key Visual
---

## One-Sentence Overview

Hamsterballin' is a UE5 local multiplayer racing game. On a 42-person team, I worked on the final track, the cableway shortcut system, and camera design, continuously iterating on navigation, route choice, and spectacle during high-speed racing.

## Project Overview

Hamsterballin’ is a local multiplayer racing game in which players control rolling and bouncing hamster balls and compete across tracks filled with obstacles, shortcuts, and three-dimensional terrain. The project was developed in SMU Guildhall's Team Game Project II course by a 42-person team over 12 weeks and is coming soon to Steam.

## My Work

### 1. Final Level: Gacha Galaxy

I believe that a great racing track should be linked together by a series of powerful “memorable moments.” In Mario Kart, for example, players may not remember every turn or every detail, but they remember the whirlpool of quicksand on a desert track or the giant eel on an underwater track. When designing a track, I first imagine these memorable moments, plan the rhythm of their appearances, and use ordinary sections to connect those peak experiences naturally.

As the primary owner of the final level, I led its thematic concept, track-layout design, and cross-disciplinary collaboration with programmers and artists, moving the level from concept to final implementation.

#### 1. Establishing the Level's Core Concept

Once the project entered level production, we needed to complete a full track within a short schedule. I quickly established our design goal: a massive central landmark that would serve as both a navigation marker and a memory anchor. I proposed building the track around a giant robot.

However, because the development schedule was short and the art team had limited bandwidth, I discussed the idea with the team leader and quickly changed the central object to a gacha machine. The revision preserved the central-landmark concept while significantly reducing art-production costs. It ultimately created the spatial structure of “racing around the gacha machine—passing through the gacha machine—entering its interior and returning to the start.”

#### 2. Leading the Design of the Core Area

After defining the overall layout, I designed the track's start, finish, and the gacha-machine area at the center of the level.

To let the track pass through the gacha machine, we wrapped a “Saturn ring” around the spherical section at its top, allowing the track to split into two paths there. This is also where the name Gacha Galaxy came from.

Because the gacha machine simultaneously served as a navigation aid, visual focal point, and expression of the level's theme, I worked extensively with the art team. We continuously adjusted model scale, track connections, and player sightlines so that the visual presentation would support navigation and the racing experience.

#### 3. Driving Iteration on the Core Gameplay

Across multiple playtests, we found that after entering the gacha machine, players had to travel through three consecutive spiral tubes to return to the upper level. This design had three problems:
• It was repetitive and offered little room for player input.
• Players easily lost their sense of direction.
• Prolonged rotation caused 3D motion sickness for some players.

The team's initial plan was simply to reduce the sequence to one spiral tube. I believed that this did not address the core issue, because players still had almost no decisions or meaningful input after entering the tube and would simply keep driving forward.

I therefore proposed replacing the entire section with the Cableway system. This solution eliminated the repetitive route and created new experiential value:
• Fixed cameras strengthened players' spatial orientation.
• High-speed racing briefly shifted into a moment of spectacle.
• A close-up view of the giant gacha machine further reinforced the level's central memory point.

The team adopted the proposal and completed its implementation.

#### 4. Project Outcome

The level was successfully completed, shipped with the game, and became the game's final level.

### 2. Cableway System and Camera Design

Beginning in the project's POCT phase, I independently proposed, designed, and implemented the Cableway system as a level shortcut. I was responsible for shortcut planning, interaction logic, and the player's camera presentation. During Cableway travel, the camera showcases scenery, previews upcoming routes, and reinforces orientation, allowing the system to function simultaneously as a shortcut, navigation tool, and cinematic sequence.

As early as the POCT phase, I drew inspiration from games including Balance and Splatoon and experimented with a high-speed Cableway system during early gameplay exploration. Because our racing game was built entirely around physics simulation, however, the Cableway could not constrain the player and the idea had to be set aside.

During the POCG phase, I still did not want to abandon the direction. Further experimentation showed that three or four cables could enclose the player's hamster ball and constrain it perfectly through physics alone. The result was highly enjoyable and had strong presentation potential. From then on, the mechanic became one of the project's primary gameplay systems and was intended for use as a track shortcut.

During full production, I naturally continued working with the art and programming teams to develop the Cableway system, and I designed every Cableway in the final level. The one I am proudest of appears near the beginning of the track, as the player is about to cross the “Saturn ring” above the gacha machine. I extended the Cableway far out from the track and curved it back in the opposite direction, forming a graceful arc. The player first moves away from the track and then cuts back toward its center at high speed. The camera pulls far back and uses a zoom lens, allowing the player to feel the speed while taking in the entire track organized around the gacha machine.

Late in development, I was asked to optimize every Cableway camera across every level. Even with little time remaining, and even though the team told me I could decline if the workload was too heavy, I accepted the task.

The camera system behind the Cableways was, frankly, extremely rudimentary. On a Cableway, a dedicated camera takes control from the player's third-person follow camera and always obeys two rules:
1. It always faces the player.
2. Its movement percentage along the camera track always equals the player's movement percentage along the Cableway.

This made camera configuration extremely difficult. There was no precise control, so each camera had to be placed manually through experience and repeated adjustment.

I quickly embedded myself with the other two level-design teams, communicated with them about their needs, adapted to their workflows, and ultimately completed the configuration and optimization of 11 Cableway cameras across three levels.

@[youtube](NM2TgDevFbo "Cableway System and Camera Design Showcase")

![Level 1 Cableways 1–2: route layout and sightline guidance](images/level1cableway1&2.jpg)

![Level 1 Cableways 3–4: continuous camera movement and environment presentation](images/level1cableway3&4.jpg)

![Level 2 Cableway 1: shortcut entrance and route connection](images/level2cableway1.jpg)

![Level 2 Cableway 2: previewing scenery during transport](images/level2cableway2.jpg)

![Level 3 Cableway 1: elevated route and spatial guidance](images/level3cableway1.jpg)

![Level 3 Cableway 2: camera composition and presentation of key targets](images/level3cableway2.jpg)

![Level 3 Cableways 3–4: continuous route pacing and environmental presentation](images/level3cableway3&4.jpg)

![Level 3 Cableway 5: Cableway exit and reconnection with the main track](images/level3cableway5.jpg)

## Timeline

Phase｜Date｜Goal｜Work
POCT｜｜｜
POCG｜｜｜
Prototype｜｜｜
Vertical Slice｜｜｜
Alpha｜｜｜
Beta｜｜｜
Launch｜｜｜

## Playtesting and Iteration

Feedback｜Analysis｜Solution

## Project Retrospective

What Went Well
• Completed the design, production, and iteration of the final level, Gacha Galaxy.
• Configured all Cableway cameras, improving navigation and presentation during high-speed movement.
• Collaborated effectively with the programming, art, and design teams, and the project successfully launched on Steam.

Even Better If
• The Cableway camera system was too rudimentary. I should have continued following up with the programming team and requested further improvements to this important system.
• Some shortcut routes had poorly balanced risk and reward in early versions and required multiple rounds of playtesting to adjust.
• During high-speed racing, some camera transitions interfered with the player's ability to read the route ahead, requiring continued refinement of camera angle and timing.
• Because multiplayer racing depends heavily on player behavior, some design problems could only be identified through extensive multiplayer testing.
• Begin multiplayer playtesting earlier and validate route design during the graybox stage.
• Add more routes with meaningful strategic differences to improve replayability.
• Enrich the final lap with more dynamic events and visual feedback to further strengthen the climax of the ending.

What I Learned
• Summarize flow-design experience from a racing project
• Summarize experience in cinematic presentation
• Summarize my level-design philosophy
• Testing and iteration
• A large-team, cross-disciplinary collaboration pipeline

## Attachments
