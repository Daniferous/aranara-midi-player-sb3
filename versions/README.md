# Aranara MIDI Players
*Scratch-Based MIDI Player that is named Aranara because of my interest in Genshin Impact. This has nothing to do with programs that play MIDIs in any Genshin Impact instruments!*

>**Please consider checking [rules and guidelines](https://daniferous.github.io/aranara-midi-player-sb3/guidelines) before reading below!**

# Faelei MIDI Render Toolkit Versions

## Release 4 (AMRT 1.6.4)
*Fork of Aranara MIDI Render Toolkit Version 1.6. May not work on all browsers but might occasionally work.*

> This version utilises a different MIDI Format (.faelei). To convert MIDIs to .faelei files, navigate to the [Faelei Branch of the Modded MIDIParser Tool here](https://github.com/Daniferous/MidiParser/tree/Faelei).

> [Faelei MIDI Render Toolkit 1.6.4](https://daniferous.github.io/aranara-midi-player-sb3/faelei/Faelei%20MIDI%20Render%20Toolkit%201.6.4.html)


# Aranara MIDI Render Toolkit Versions

## 1.6
*Fork of AMP 2.3.8. Contains advanced features, such as selective audio channel rendering and customizable color palettes. Added a setting to limit maximum audible note lengths to 1 bar. Works effectively for "normal" tempo MIDIs (or MIDIs that have tempos typically within 60~200.) The resolution setting now only impacts the visuals and not the audio.*
> [Aranara MIDI Render Toolkit 1.6.html](https://daniferous.github.io/aranara-midi-player-sb3/amrt/Aranara%20MIDI%20Render%20Toolkit%201.6.html)

## 1.5
*Added option to limit audible note lengths to a maximum of 1 beat.*

## 1.4
*Fixed Palette Bug persisting in versions prior. This does not affect the AMP series.*

# Faelei MIDI Player Versions

## Release 1.0.0 (AMP 2.3.8)
*Fork of AMP 2.3.8. May not work on all browsers but might occasionally work.*

> This version utilises a different MIDI Format (.faelei). To convert MIDIs to .faelei files, navigate to the [Faelei Branch of the Modded MIDIParser Tool here](https://github.com/Daniferous/MidiParser/tree/Faelei).

> [Faelei MIDI Player 1.0.0](https://daniferous.github.io/aranara-midi-player-sb3/faelei/Faelei%20MIDI%20Player%201.0.0.html)

# Aranara MIDI Player Versions 

## 2.3.8
*Added a setting to control audio velocity threshold. This mutes notes that are at or under this value.*
> [Aranara MIDI Player Release 2.3.8](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%202.3.8.html)

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
> [Aranara MIDI Player Release 2.2.2](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%202.2.2.html)

## 2.1.0
*New Color System Test*

## 2.0.0
*New Keyboard Overlay Test*

## Aranara MIDI Lite V0.3.5
*Intended to be lightweight, revamped version of R1.5.5. Block Ct: 1280*
> [Aranara MIDI Player Lite V0.3.5](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%20Lite%20v0.3.5.html)

> [Aranara MIDI Player Lite V0.3.5 Fancy](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%20Lite%20v0.3.5%20-%20Fancy.html) 

>*The "Fancy" edition contains slightly more blocks but is more similar in aesthetics to PFA. Block Ct: 1305*

## R1.5.5
*Minor Bug Fixes*
> [Aranara MIDI Player Release 1.5.5](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%20R1.5.5.html)

## R1.5.4
*Implemented the Boba Branch and merged it with the main branch. Identical to the latest Boba Update (B1.2)*
> [Aranara MIDI Player Release 1.5.4](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%20R1.5.4.html)

## R1.5.3
> [Aranara MIDI Player Release 1.5.3](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%20R1.5.3.html)

> [Aranara MIDI Player Release 1.5.3 Widescreen](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%20R1.5.3W.html)

## R1.5.3 - Boba Branch
*The Boba Branch is an experimental branch where only the audio events and visual data are used during playback, at the cost of not having a notecount...*

## R1.5.0
*Private Development Branch, not really used for R1.5.X*

## R1.3.2
> [Aranara MIDI Player Release 1.3.2](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%20R1.3.2.html)

> [Aranara MIDI Player Release 1.3.2 Widescreen](https://daniferous.github.io/aranara-midi-player-sb3/amp/Aranara%20MIDI%20Player%20R1.3.2W.html)

# Aranara MIDI Format Versions

> Disclaimer: The term "PPQ" (Pulses Per Quart) and "TPQ" (Ticks Per Quart) are used here interchangeably.

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
>*Note: All values are in hexadecimal.*

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
### 1.2
```
+ Added Header "[Aranara]█"
+ Support for Older Aranara Format MIDIs still allowed
- Fixed Bug which caused Channel 16 events to be parsed as Channel 1 Events
- Older Aranara Format MIDIs will still need to be reconverted using the updated conversion tool.
```

### 1.1
```
+ Added MIDI Resolution (Typically stored as 768 ticks per half note, or 384 ticks per quarter note)
+ Added Support for Program Change
```

### 1.0
```
Initial Version of Aranara MIDI Format
```

# Faelei MIDI Format Versions
*Generally identical to Aranara MIDI, but contains support for MIDI CC and Pitch Bends.*
> [Faelei MIDI Player](https://daniferous.github.io/aranara-midi-player-sb3/faelei/Faelei%20MIDI%20Player%201.0.0.html) and [Faelei MIDI Render Toolkit](https://daniferous.github.io/aranara-midi-player-sb3/faelei/Faelei%20MIDI%20Render%20Toolkit%201.6.4.html) are now available. To convert your MIDIs into compatible Faelei MIDIs, you can visit [the Faelei Branch of the Modded MIDIParser Tool here](https://github.com/Daniferous/MidiParser/tree/Faelei).

> Disclaimer: The term "PPQ" (Pulses Per Quart) and "TPQ" (Ticks Per Quart) are used here interchangeably.

## Main Structure

Structure is as follows:
```
[Data Type][Data Value/s]*
*Variable Length Data Values are concluded with a separator, "|".
```
Data Type can be as follows:
```
0 - 7: First digit of note pitch, which ranges from 00 to 7F.
8 - A: Reserved
B: Pitch Bends
C: Control Change
D: Program Change
E: Tempo Change
F: Track Header
```
Data Values depend on the Data Type:
>*Note: All values are in hexadecimal.*

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

5. Control Change
```
[Controller - 2 chars][Controller Value - 2 chars][Channel - 1 char][Tick - Variable][Separator]
```

6. Pitch Bends
```
[Pitch Bend Value 4 chars][Channel - 1 char][Tick - Variable][Separator]
```

## Versions
### 1.1
```
+ Converted PPQ/TPQ is now identical to the imported MIDI PPQ if the PPQ value is at or below 1536.
+ Converted PPQ will undergo repeated division by 2 until it is at or below 1536.
```

### 1.0 (AranaraMIDI 1.2 Modded)
```
+ Added Header "[Faelei]█"
+ Adaptive PPQ/TPQ. Converted Faelei MIDIs may either have 768, 960, or 1024 PPQ depending on the original MIDI's PPQ. See PPQ rule (Faelei 1.0) below.
- Possible Support for Aranara MIDIs in some Faelei MIDI Players. Since Faelei MIDI is an extension to Aranara MIDIs, it is possible to run Aranara MIDIs.
```

## Faelei MIDI PPQ Rules - Version 1.1

### 1. All Converted MIDIs will retain their PPQ.
- This allows MIDIs with unusual/low PPQ values to be retained. For example, a MIDI with a resolution of 96 PPQ will no longer be converted to a 768 PPQ Faelei MIDI, reducing the converted Faelei MIDI file size by a small amount.
- This does not apply to MIDIs with large PPQs (see below).

### 2. For MIDIs with PPQ values greater than 1536, it will be brought down to a value at or under 1536.
- This is done by dividing the PPQ value by 2 multiple times until it is at or under 1536. For example, a MIDI with an original PPQ value of either 1920 or 3840 will be brought down to 960.
- In the updated Modded Faelei MIDI Parser, the following is the algorithm used to determine the PPQ/TPQ value used in the converted Faelei MIDI.

<div style="text-align: center;">

${\operatorname{ For }}\ \ O_{riginalTPQ}>1536:\ F_{aeleiTPQ}=\frac{O_{riginalTPQ}}{2^{\operatorname{ceil}\left(\log_{2}\left(\frac{O_{riginalTPQ}}{1536}\right)\right)}}$

${\operatorname{ For }}\ \ 1\le O_{riginalTPQ}\le1536:\ \ F_{aeleiTPQ}=O_{riginalTPQ}$

$Where:$

$O_{riginalTPQ}$ - The PPQ Value of the Imported MIDI

$F_{aeleiTPQ}$ - The PPQ Value of the Converted Faelei MIDI

</div>

- Thus, with a division factor of 2, <u>there is minimal loss in data accuracy compared to if it were a factor of 5 or 10</u>. However, issues may arise if a MIDI has a PPQ that is either odd-numbered or is not a multiple of 2<sup>n</sup>, with n being the number of divisions. This should not be an issue for MIDIs having common PPQ values.

- This new system is much simpler than the previous system since only a single logic is required (checking if the PPQ value is greater than 1536 to divide repeatedly) and allows most MIDIs to retain its resolution after conversion.

## Faelei MIDI PPQ Rules - Version 1.0

> Disclaimer: This has been superceded by a new MIDI PPQ System in Faelei 1.1.

### 1. All Converted MIDIs will have a PPQ of 768.
- This is a 2x increase in resolution compared to the Aranara MIDI format of 384 PPQ (Pulses per Quarter note) or 768 TPH (Ticks per Half-Note).
- There are exemptions listed below.

### 2. MIDIs with a PPQ divisible by 120 will have a PPQ of 960.
- This is to accomodate quintuplet notes/divisions.
- Most MIDIs are generally running on a resolution at this range, especially MIDIs made with FL Studio (PC).

### 3. MIDIs with a PPQ divisible by 128 but greater than 768 will have a PPQ of 1024.
- This only applies to MIDIs that either have a PPQ of 2048, 2560, 4096, etc.

> ### Disclaimer
> - It is worth noting that this system is imperfect. There may be new conditions, such as allowing any custom PPQ/resolutions to not conform to either of the rules provided that it falls within an "acceptable range."
> - The acceptable range will be between 512 and 1536. Larger PPQs will have to be rounded down.

---

>[Back to top](https://daniferous.github.io/aranara-midi-player-sb3/versions)

# Navigation Portal

>[Main Page](https://daniferous.github.io/aranara-midi-player-sb3)

>[Aranara MIDI Programs and MIDI Specifications](https://daniferous.github.io/aranara-midi-player-sb3/versions)

>[Lurker of the Lost Game](https://daniferous.github.io/aranara-midi-player-sb3/lostlurkergame)

>[Guidelines for Proper Usage](https://daniferous.github.io/aranara-midi-player-sb3/guidelines)

>[Program Credits](https://daniferous.github.io/aranara-midi-player-sb3/credits)