# swjs-hundo

A live map and 100% exploration tracker for **Star Wars Jedi: Survivor** (PC), made for speedrunners.
Download the latest version from the **Releases** page; no git or programming tools needed.

## What it does

- **Three modes**, picked on the setup page the app opens on (or from **View**):
  - **Runner Mode:** the map plus what's left to collect, completion at a glance, and **Record run**
    to race your run later as a ghost.
  - **Routing Mode:** build or customize a 100% route (splits with steps, notes, section ghosts,
    LiveSplit import / export) and share it as a file.
  - **Research Mode:** everything, including logging and scans to help complete the map.
- **Live map** of the planet you're on: floor, map regions, collectibles, meditation points, enemy
  spawns, kill zones and loading triggers (where scanned so far), with your position on it.
- **Follows the game**: switches planet when you travel, and shows a galaxy overview on the title
  menu, the Mantis and in hyperspace. You can also pick any planet from **View ▸ Planet**.
- **Exploration %** per planet and for the whole game, read live from the game for the planet you're
  on and from your save for the others.
- **Ghost** (lightly tested): race a recorded run and see how far ahead or behind you are.
- **Logging and scans**: record your own runs and scan new areas to help complete the map.

## It only reads the game

swjs-hundo **never writes to the game's memory**, never injects anything and never changes your save
files. It opens the game for reading only and reads save files read-only.

## Requirements

- Windows 10 or 11, 64-bit, with .NET Framework 4.8 (built into Windows 10 since the May 2019 update).
- Star Wars Jedi: Survivor on PC. Tested on the Steam version (build 15643690). A game update can move
  what the app reads; if something stops working after an update, check for a newer release.

## Getting started

1. Download the zip from **Releases** and unzip it anywhere (keep the files together).
2. Run `swjs-hundo.exe`. Windows may warn about an unrecognised app the first time, since it isn't
   signed: choose **More info ▸ Run anyway**.
3. Start the game and load your save. The map and exploration % follow you on their own.

## Helping complete the map

The map only shows areas someone has scanned. To add yours (in **Research Mode**: View ▸ Research
Mode):

1. **Logging ▸ What to log…**: pick what to record (all on by default).
2. **Logging ▸ Start logging**, then play. When a new area loads, a red **STOP** banner appears:
   stand still until it turns green **GO** (about 15 seconds).
3. **Logging ▸ Stop logging** when you're done.
4. **File ▸ Export my scans (zip)…** and send the zip to the maintainer. It contains positions from
   your scans only: no recordings of your runs, no logs, nothing personal.

## Reporting a problem

**Help ▸ Report an issue** (or right-click a map marker with a wrong name). It opens a pre-filled
GitHub issue on this page, or copies the report if you don't have a GitHub account. You see
everything it includes before sending.

## Where it keeps things

Your scans, recordings, routes and settings are in `%LOCALAPPDATA%\swjs-hundo\`. **Tools ▸ Check for
updates** asks this page for a newer version (optionally at every start).

## Status (0.2.1)

Early version. Map data so far: floors for Coruscant, Koboh and Tanalorr; map-section shapes for
Jedha; collectibles, regions and triggers for the planets visited in testing. Route steps for the
LiveSplit split you're on and the skill-point pace label are planned, not built yet.

## Legal

An unofficial fan tool, not affiliated with or endorsed by Respawn Entertainment, Electronic Arts or
Lucasfilm. Star Wars Jedi: Survivor and related names belong to their owners. No licence is granted
for this software yet: all rights reserved.
