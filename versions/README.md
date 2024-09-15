# Aranara MIDI Players
*Scratch-Based MIDI Player that is named Aranara because of my interest in Genshin Impact. This has nothing to do with programs that play MIDIs in any Genshin Impact instruments!*

**Please consider checking [rules and guidelines](https://daniferous.github.io/aranara-midi-player-sb3/guidelines) before reading below!**

## Disclaimer:
*Note: This page will be replaced with a WIP site that should make it easy on the eyes!*
[Click here to check the new page!](https://daniferous.github.io/aranara-midi-player-sb3/main/index.html)

# Versions 
See Bottom for Modded Variants

## Aranara MIDI Renderer Toolkit 1.2
*Fork of AMP 2.3.8. Contains advanced features, such as selective audio channel rendering and customizable color palettes.*
- [Aranara MIDI Renderer Toolkit 1.2.html](https://daniferous.github.io/aranara-midi-player-sb3/amrt/Aranara%20MIDI%20Renderer%20Toolkit%201.2.html)

## 2.3.8
*Added a setting to control audio velocity threshold. This mutes notes that are at or under this value.*
- [Aranara MIDI Player Release 2.3.8](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%202.3.8.html)

## 2.3.7
*Fixed a bug where Program Change does not work as intended for Ch 16.*

## 2.3.4
*Fixed bug where having more than multiple songs would cause choosing menu options to load/delete songs*

## 2.3.3
*Revamped Aranara MIDI Format!*
### Please Note!
A crucial update has been made to the Aranara MIDI Format. Thus, any future Aranara MIDI Format Projects will require any new Aranara MIDIs made with the updated Modded MIDIParser Converter Tool!

## 2.3.2
*Added PFA Color Mode*
*Fixed a bug in deleting songs*
Note: There is a known bug wherein regardless of tracks, channel colors will remain the same if using PFA Color Mode. (MIDITrail-like) This has been fixed in 2.3.3.

## 2.2.0
*New Audio System Test - First Public Release of 2.X*
- [Aranara MIDI Player Release 2.2.2](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%202.2.2.html)

## 2.1.0
*New Color System Test*

## 2.0.0
*New Keyboard Overlay Test*

## Aranara MIDI Lite V0.3.5
*Intended to be lightweight, revamped version of R1.5.5. Block Ct: 1280*
- [Aranara MIDI Player Lite V0.3.5](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%20Lite%20v0.3.5.html)
- [Aranara MIDI Player Lite V0.3.5 Fancy](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%20Lite%20v0.3.5%20-%20Fancy.html) 
*Contains slightly more blocks but is more similar to PFA. Block Ct: 1305*

## R1.5.5
*Minor Bug Fixes*
- [Aranara MIDI Player Release 1.5.5](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%20R1.5.5.html)

## R1.5.4
*Implemented the Boba Branch and merged it with the main branch. Identical to the latest Boba Update (B1.2)*
- [Aranara MIDI Player Release 1.5.4](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%20R1.5.4.html)

## R1.5.3
- [Aranara MIDI Player Release 1.5.3](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%20R1.5.3.html)
- [Aranara MIDI Player Release 1.5.3 Widescreen](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%20R1.5.3W.html)

## R1.5.3 - Boba Branch
*The Boba Branch is an experimental branch where only the audio events and visual data are used during playback, at the cost of not having a notecount...*

## R1.4.0
*Private Development Branch, not really used for R1.5.X*

## R1.3.2
- [Aranara MIDI Player Release 1.3.2](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%20R1.3.2.html)
- [Aranara MIDI Player Release 1.3.2 Widescreen](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%20R1.3.2W.html)

# Aranara MIDI Format Versions
## Main Structure

Structure is as follows:
```
[Data Type][Data Value/s]*
*Variable Length Data Values are concluded with a separator, "|".
```
Data Type can be as follows:
```
0 - 7: First digit of note pitch, which ranges from 00 to 7F.
8 - B: Reserved, Unused
C: Control Change, Unused
D: Program Change
E: Tempo Change
F: Track Header
```
Data Values depend on the Data Type:
1. Note Events
```
[Pitch - 2 chars][Velocity - 2 chars][Channel - 1 char][Tick - Variable][Separator][Length - Variable][Separator]
```
2. Program Change
```
[Patch Value - 2 chars][Channel - 1 char][Tick - Variable][Separator]
```
3. Tempo Change
```
[Microseconds per Beat - Variable][Separator][Tick - Variable][Separator]
```
4. Track Header
```
[Track Value - Variable][Separator]
```
## Versions
- 1.2
```diff
+ Added Header "[Aranara]█"
+ Support for Older Aranara Format MIDIs still allowed
- Fixed Bug which caused Channel 16 events to be parsed as Channel 1 Events
- Older Aranara Format MIDIs will still need to be reconverted using the updated conversion tool.
```
- 1.1
```diff
+ Added MIDI Resolution (Typically stored as 768 ticks per half note, or 384 ticks per quarter note)
+ Added Support for Program Change
```
- 1.0
Initial Version of Aranara MIDI Format


[Return to Main Page](https://daniferous.github.io/aranara-midi-player-sb3)