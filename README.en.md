# BlockSlayer

[中文](README.zh.md) · [English](README.en.md) · [Español](README.es.md) · [Project home](README.md)

**INNNX. · A Flutter prototype combining block clearing with slime combat**

BlockSlayer starts with spatial planning: drag differently shaped pieces onto a board, fill rows or columns and clear them. The current prototype adds slime health, attacks powered by line clears and enemy turns counted by successful placements. Choosing where to place a piece affects both the board's available space and the combat rhythm.

## HOME preview and navigation

<a href="screenshots/home.png"><img src="screenshots/home.png" width="320" alt="Existing BlockSlayer English home showing Classic Mode, Time Attack and settings" /></a>

This is the existing authentic home screenshot. It still displays BLOCK CRUSH and English button labels. Chinese and Spanish home interfaces have not been confirmed; those documentation pages explain this same real interface in their own languages.

| Home element | Meaning and behavior |
| --- | --- |
| BLOCK CRUSH | The retained application name. The public showcase uses BlockSlayer; existing internal naming is not yet unified. |
| CLASSIC MODE | Place blocks, clear lines and earn points. The round ends when none of the remaining pieces can fit. |
| TIME ATTACK | The current implementation starts at 120 seconds. Each successful placement adds 2 seconds and each cleared line adds 5 seconds. |
| BEST | A locally stored high score for the corresponding mode. |
| Gear icon | Settings for sound effects and the Neon, Wood or Jewel theme. |

## Core loop: place, clear and preserve space

1. Open Classic Mode or Time Attack.
2. Drag a candidate piece onto the 8×8 board. It must stay within the board and cannot overlap occupied cells.
3. Complete a row or column to clear it, gain points and free space.
4. Each set supplies three candidate pieces. A new set appears after all three are used. Plan both immediate clears and room for future shapes.
5. Classic Mode ends when no remaining piece can be placed. Time Attack also runs against a countdown.

## Scoring and time

The current implementation adds 10 points for each occupied cell in an accepted piece. Line bonuses use “cleared lines × 100 × consecutive-clear count.” A placement without a clear resets that count. In Time Attack, placing and clearing extend the timer, combining quick decisions with board planning. These are current implementation values, which may change during balancing.

## Slime combat prototype

The prototype enemy starts with 100 HP. Clearing one line deals 10 damage, two lines deal 25, and three or more deal 45. Combat feedback links the clearing cells to the enemy panel, making line clears part of an attack rather than only a score event.

By default, an enemy turn triggers after every five successful piece placements. Failed drops do not advance the counter. A warning state appears one placement before the attack. Defeating the slime stops its turns. The implementation also includes slime board hazards and attack feedback, so combat can affect the board layout.

These details come from a read-only inspection of the private implementation. They were not runtime-tested in this update. The earlier gameplay image below does not include the later combat panel and does not establish validation of the current combat interface.

## Existing gameplay image

<a href="screenshots/game.png"><img src="screenshots/game.png" width="320" alt="Early BlockSlayer block gameplay image without the later slime combat panel" /></a>

## Visuals, audio and local records

The home uses a gradient background, glowing title and mode cards. Settings include Neon, Wood and Jewel themes and a sound-effects switch. Local storage supports high scores and related preferences. Screenshot and sharing dependencies exist, but the complete sharing flow has not been revalidated here.

## Technology, origin and status

Flutter, Dart, Provider, SharedPreferences, flutter_animate and audioplayers. The public material presents a prototype, not a verified finished release.

The original local README credited Md Rounaq Ali's `block-crush-game` project. The interface and internal identifiers retain Block Crush / block_blast names. This showcase does not attribute all upstream work to INNNX. The exact upstream URL, license, asset permissions and modification scope still need verification. The original README's store-release, performance and license claims are not adopted here.

## Playing and public scope

No installer is currently public. Redistribution permissions and actual installation, launch and core gameplay must be checked before offering a playable build. This repository contains documentation and images; source code, signing materials and development configuration remain private. GitHub's automatic Source code archive is not a playable game.

[Playable release guide](docs/PLAYABLE-RELEASE.md)
