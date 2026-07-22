---
title: Hamsterballin’
tab_title: UE5 Multiplayer Racing: Hamsterballin’
tag: Unreal Engine 5
type: 3D / Local Multiplayer / Racing / Mario Kart–Like
role: Final Level / Cableway System / Camera Design
time: 12 Weeks / 42-Person Team
status: Steam Store Page Public
status_url: https://store.steampowered.com/app/4319370/Hamsterballin/
status_link: View on Steam
caption: ▲ Iterative improvements to navigation, route choice, and spectacle during high-speed racing
hero: images/hero.jpg
hero_caption: Key art for Gacha Galaxy, the final level of Hamsterballin’
---

## One-Sentence Overview

Hamsterballin’ is a UE5 local multiplayer racing game. On a 42-person team, I designed the final track, the cableway shortcut system, and its camera work, iterating continuously to improve navigation, route choice, and spectacle during high-speed racing.

## Project Overview

Hamsterballin’ is a local multiplayer racing game in which players control rolling, bouncing hamster balls and compete across tracks filled with obstacles, shortcuts, and layered terrain. Developed for SMU Guildhall’s Team Game Project II course, the game was completed by a 42-person team over 12 weeks and is scheduled for release on Steam.

## My Work

### 1. Final Level: Gacha Galaxy

I believe a great racing track should be connected by a sequence of powerful “memorable moments.” In Mario Kart, for example, players may not remember every corner or detail, but they remember the quicksand vortex in the desert track or the giant eel in the underwater track. When designing a course, I first envision moments like these, establish the rhythm at which they appear, and use standard track sections to connect those peaks naturally.

![Figure 1: Presentation slide explaining my “memorable moments” design approach](images/figure-01-memory-point-ppt.jpg)

As the primary designer responsible for the final level, I led its thematic concept, track-layout design, and cross-disciplinary collaboration with programming and art, carrying the level from concept through final implementation.

#### 1.1 Establishing the Core Level Concept

When the project entered level production, we needed to complete an entire track within a short development window. I quickly established the design goal: a massive central landmark that could act as both a navigation cue and a memorable spatial anchor. My initial proposal was to build the track around a giant robot.

![Figure 2: Initial level design](images/figure-02-initial-level-design.jpg)

However, given the short schedule and limited art resources, I discussed the concept with the team lead and quickly revised the centerpiece into a gacha machine. This change preserved the central-landmark concept while significantly reducing the art-production cost. It ultimately produced the level’s overall spatial structure: race around the gacha machine, pass through it, then enter its interior to return to the starting point.

![Figure 3: Opening section of the track](images/figure-03-track-start.jpg)

#### 1.2 Leading the Design of the Core Areas

After establishing the overall layout, I designed the starting area, finish line, and the gacha-machine zone at the center of the level.

To route the track through the gacha machine, we wrapped a “Saturn ring” around the spherical section at its top, allowing the track to split into two routes at this location. This idea also gave the level its name, Gacha Galaxy.

![Figure 4: Racing through the gacha machine](images/figure-04-through-gacha-machine.jpg)

As the central structure of the level, the gacha machine had to serve navigation, visual focus, and thematic communication simultaneously. I collaborated extensively with the art team, continually adjusting the model’s scale, style, track connections, and player sightlines so the visual presentation would support navigation and the racing experience.

#### 1.3 Driving Iteration on the Core Gameplay

Across multiple playtests, we found that after entering the gacha machine, players had to climb back upward through three consecutive spiral tubes. This design created three problems:
• The route was repetitive and offered little room for player input.
• Players easily lost their sense of direction.
• Sustained rotation caused 3D motion sickness for some players.

The team initially planned to reduce the sequence to a single spiral tube. I believed this did not address the underlying issue: once inside the tube, players had almost no decisions or meaningful actions and simply continued driving forward.

I therefore proposed replacing the entire section with the Cableway system. The solution eliminated the repetitive route and introduced new experiential value:
• It briefly shifted the pace from high-speed racing to scenic spectacle.
• It brought players close to the giant gacha machine, further reinforcing the level’s central memorable moment.

The team adopted the proposal and completed its implementation.

![Figure 5: Cableway inside the gacha machine](images/figure-05-interior-cableway.jpg)

#### 1.4 Project Outcome

The level was completed successfully, shipped with the game, and became the game’s final track.

![Figure 6: Final level view 1](images/figure-06-final-level-01.jpg)

![Figure 7: Final level view 2](images/figure-07-final-level-02.jpg)

### 2. Cableway System and Camera Design

Beginning in the project’s POCT phase, I independently proposed, designed, and implemented the Cableway system as a track shortcut. I was responsible for shortcut planning, interaction logic, and the player-camera sequences. While the player travels along a cableway, the camera presents the environment, previews upcoming routes, and reinforces orientation, allowing the system to function simultaneously as a shortcut, navigation tool, and cinematic presentation device.

During the POCT technical-validation phase, I drew inspiration from games such as Ballance and Splatoon and attempted to prototype a high-speed cableway system. Because our racing game was built entirely around physics simulation, however, the cableway could not reliably constrain the player, so I had to abandon the first version.

![Figure 8: Cableway in Splatoon](images/figure-08-splatoon-cableway.jpg)

![Figure 9: POCT cableway demonstration](images/figure-09-poct-cableway-demo.gif)

During the POCG gameplay-validation phase, I was still unwilling to give up on the direction. Through further experimentation, I discovered that three to four cableways could hold the player’s hamster ball between them using physics alone. The result constrained the player perfectly while providing strong gameplay appeal and presentation potential. From that point onward, the Cableway became one of the project’s major mechanics and was intended for use as a track shortcut.

![Figure 10: POCG cableway demonstration](images/figure-10-pocg-cableway-demo.gif)

During full production, I naturally continued developing the Cableway system in collaboration with the art and programming teams, while also designing every cableway in the final level. The cableway I am most proud of appears near the beginning of the track as players approach the “Saturn ring” above the gacha machine. I extended the route far outward and added a reverse curve to create a graceful arc, sending players away from the track before cutting back toward the center at high speed. I also pulled the camera far back and used a zoom shot, allowing players to feel the speed while taking in the entire course centered on the gacha machine.

![Figure 11: Gacha-machine zoom cableway sequence](images/figure-11-gacha-zoom-cableway-showcase.gif)

Late in development, I was asked to optimize every cableway camera across all levels. Although time was limited and the team told me I could decline if the workload felt too heavy, I chose to take on the task.

The camera system behind the cableways was, admittedly, very limited. On a cableway, a dedicated cableway camera takes control from the standard third-person camera and always follows two rules:
1. It always faces the player.
2. Its progress percentage along the camera rail always equals the player’s progress percentage along the cableway.

These constraints made camera setup extremely difficult. The system offered no precise control, so every sequence had to be tuned manually through experience and repeated adjustment.

I quickly embedded myself with the other two level-design groups, communicated their needs, adapted to their workflows, and ultimately configured and polished 11 cableway camera sequences across three levels.

![Figure 12: Level 1 cableways 1 and 2](images/level1cableway1&2.jpg)

![Figure 13: Level 1 cableways 2 and 3](images/level1cableway3&4.jpg)

![Figure 14: Level 2 cableway 1](images/level2cableway1.jpg)

![Figure 15: Level 2 cableway 2](images/level2cableway2.jpg)

![Figure 16: Level 3 cableway 1](images/level3cableway1.jpg)

![Figure 17: Level 3 cableway 2](images/level3cableway2.jpg)

![Figure 18: Level 3 cableways 3 and 4](images/level3cableway3&4.jpg)

![Figure 19: Level 3 cableway 5](images/level3cableway5.jpg)

![Figure 20: Cableway presentation animation 1](images/figure-20-cableway-animation-01.gif)

![Figure 21: Cableway presentation animation 2](images/figure-21-cableway-animation-02.gif)

![Figure 22: Cableway presentation animation 3](images/figure-22-cableway-animation-03.gif)

![Figure 23: Cableway presentation animation 4](images/figure-23-cableway-animation-04.gif)

![Figure 24: Cableway presentation animation 5](images/figure-24-cableway-animation-05.gif)

![Figure 25: Cableway presentation animation 6](images/figure-25-cableway-animation-06.gif)

@[youtube](NM2TgDevFbo "Cableway System and Camera Design Demonstration")

## Timeline

Stage｜Date｜Work
POCT｜2/20/2026｜Explored early Cableway gameplay and experimented with winding routes.
POCG｜3/6/2026｜Continued exploring the Cableway system and produced playable content.
Prototype & Vertical Slice｜3/27/2026｜Built a test level, learned the PCG tools, and integrated cableways into the track.
Alpha｜4/10/2026｜Designed and built the final level.
Beta｜5/1/2026｜Configured and polished all cableway camera sequences.
Launch｜5/10/2026｜Conducted final testing and fixed track PCG and respawn points.

## Playtesting and Iteration

Problem｜Iteration｜Result
The tubes inside the gacha machine were too repetitive, and their rotation caused 3D motion sickness.｜Replaced the tubes with cableways.｜Created a distinctive spiraling presentation, removed the directionless section with no meaningful player input, and eliminated the source of 3D motion sickness.
The final stretch of the track was too short, leaving little opportunity for a late overtake and removing suspense from the ending.｜Extended the route and added a large U-shaped turn so skilled players could complete an aerial overtake.｜Created a shortcut opportunity in the final stretch and added competitiveness and excitement.
The presentation cameras received many rounds of feedback.｜Continued coordinating, tuning, and revising them.｜Completed the configuration and optimization of 11 cableway camera sequences across three levels.

## Project Retrospective

What Went Well
• Completed the design, production, and iteration of the final level, Gacha Galaxy.
• Configured every cableway camera, improving navigation and presentation during high-speed movement.
• Collaborated effectively with programming, art, and design, helping the project launch successfully on Steam.

Even Better If
• The cableway camera system was too limited. I should have continued following up with the programming team and requested stronger tools for this important system, which would have avoided a workflow dependent on slow manual tuning.
• Some shortcut routes in early versions had imbalanced risk and reward. In particular, several cableways sacrificed route length for presentation value and required multiple rounds of playtesting.
• At racing speed, some camera transitions interfered with the player’s ability to read the route ahead, requiring continued refinement of camera angles and timing.
• Because multiplayer racing depends heavily on player behavior, some design issues could only be discovered through extensive multiplayer testing.
• Multiplayer playtests should have begun earlier so the route design could be validated during the graybox stage.
• The final lap could have used richer dynamic events, visual feedback, and varied presentation to create a stronger climactic finish.

What I Learned
• Racing-line and flow design
• Camera presentation and staging
• A clearer personal philosophy of level design
• Playtesting and iteration
• Cross-disciplinary production pipelines on a large team

## Attachments

• None
