# Aranara MIDI Player Credits

>This section may be a little lengthy, so I have a summarized list at the bottom of this page. Though, I would greatly appreciate it if you took the time to read the succeeding paragraphs. Have a great day!

Here are the following people I'd like to thank for *not only* the development of the Aranara MIDI Player and Renderer, but also for the development and evolution of my MIDI Player Programs since the beginning.

I would not have began my journey of making MIDI Progams in Scratch if it weren't for [Lataliat](https://scratch.mit.edu/users/Lataliat/) and their [Black MIDI project](https://scratch.mit.edu/projects/119882065). This project made me realise that I could recreate those Black MIDI videos in Scratch! My first MIDI related projects in Scratch were mostly [modifications](https://scratch.mit.edu/projects/256335788/) on their MIDI Projects.

Eventually, I developed the first "MIDI Format" that served as an extension of the format that Lataliat's program runs with. I called that format the "Lataliat Format" and its modification became known as the "OjasnGamer101" (OJG) Format, following the tradition of naming things by their author which still someone lives to this day. A project that contains such modification is the ["11.5k Notes! Black MIDI Undertale - Dogsong"](https://scratch.mit.edu/projects/324550497/) project.

The OJG format evolved to become the "New Eden Format" (NEF) which was fundamentally the same thing in terms of structure but now includes the note's velocity and its length, parameters absent in both the OJG and Lataliat formats. I believe [an earlier iteration of this project](https://scratch.mit.edu/projects/557223554/) uses the NEF format in its compressed form (CNEF), prior to its update to using the "MK9" format which I will talk about next.

After several months have passed, I stumbled upon the [MIDI Player Piano Roll Project](https://scratch.mit.edu/projects/406337184/) made by [K9shyguy](https://scratch.mit.edu/users/K9shyguy/) which was how I found out about the [MIDI Importer tool](https://github.com/FlynnD273/MidiParser) they made, which eventually became the foundation of the current [Modded MIDI Parser](https://github.com/Daniferous/MidiParser/tree/master) tool.

It was there I realised how I can now import my [own MIDIs](https://www.youtube.com/watch?v=-h7W-vkyi3s) into Scratch. I called the MIDI format the original MIDI Parser used the "MK9" format, which is short for "Modified K9Shyguy". As far as I remember, this format remained persistent as it had gone through 5 major changes throughout my usage of it in my MIDI Programs. A lot of my MIDI Programs have used this format, such as:

- [The Scratch Piano From Above Project](https://scratch.mit.edu/projects/633610677/)
- [KazuMIDI Project](https://scratch.mit.edu/projects/852652452/)
- [My Horizontal MIDI Player](https://scratch.mit.edu/projects/603901091/)
- ["Newer" Eden MIDI Player](https://scratch.mit.edu/projects/722655492/)

Funnily enough, all of them still converted the input MK9 formats into the old NEF formats aforementioned, which meant that the Import process was often very slow (most especially with the Scratch PFA project).

While working on the "Newer" Eden MIDI Player, I found a project made by [52525rr](https://scratch.mit.edu/users/52525rr/) titled ["scratch PFA v1.5 MIDI SUPPORT"](https://scratch.mit.edu/projects/717549463/) and saw how wonderful it was. She made a wonderful MIDI Project and I was able to learn a bit from her, especially when it came to processing MIDI Data, in which she utilized [Radix Sorting](https://en.wikipedia.org/wiki/Radix_sort).

Radix Sorting is used to sort MIDI events by their absolute time. This was because the actual file structure of a MIDI involves iterating through the tracks FIRST and having every event in each track sorted by time. To put it simply, Radix Sorting helped "merge" all MIDI tracks into just one track that the player or renderer could process.

I would like to thank [vicketick](https://scratch.mit.edu/users/vicketick) for their [implementation of Radix Sort in Scratch](https://scratch.mit.edu/projects/711353120) as their code became the reason why even my current MIDI players and renderers have decent MIDI import processing times.

While I was working on KazuMIDI, I started thinking of a new format. This format would eventually become the Aranara MIDI Format. I called this such because I used to play this one game called [Genshin Impact](https://genshin.hoyoverse.com/) and there were these small creatures called the [Aranara](https://genshin-impact.fandom.com/wiki/Aranara) and I thought naming a new MIDI format out of those would make sense, since at the time, the Aranara MIDI Format would be slightly less in size compared to actual MIDI Data converted into readable text.

The structure of the AraMIDI format has remained mostly unchanged since its infancy, other than the addition of new features such as support for Control Change and Instruments.

That being said, it does not mean that development has stopped here. In fact, I have recently made [an updated form of the Aranara MIDI Format: The Faelei Format](https://github.com/Daniferous/MidiParser/tree/Faelei).

Which leads to the one person who is the main reason why I am able to do things like this. He is a very talented individual who helped me understand a little more about how MIDI works. I learned a lot because of him, and it is why I greatly thank [hevean](https://scratch.mit.edu/users/hevean_3/) for practically the success of the Aranara MIDI Program and its formats. He is also the mastermind behind the MIDI Plugin that the Faelei MIDI Programs rely on to have full Control Change Support.

Overall, both hevean and 52525rr have helped improve my skills and understanding on how MIDIs work and how to render them (hopefully) as efficient as possible, except for one small thing which I will point out later.

But without Lataliat and K9shyguy/Flynn, I would have never progressed and develop the skills I have currently.

Thank you, all of you, for making all this possible.

## Summary
Special thanks to the following, by order of precedence:
1. [Lataliat](https://scratch.mit.edu/users/Lataliat/) - For starting my MIDI Programming Journey.
2. [Flynn/K9shyguy](https://scratch.mit.edu/users/K9shyguy/) - For making me realize MIDI Import and its capabilities.
3. [52525rr](https://scratch.mit.edu/users/52525rr/) - For showing me how to import and render MIDIs faster, and for being a good friend.
4. [vicketick](https://scratch.mit.edu/users/vicketick) - For showing me how to implement Radix Sorting.
5. [hevean](https://scratch.mit.edu/users/hevean_3/) - For showing me how to further optimize my code, helping me learn more about MIDI, for developing new techniques to further improve MIDI rendering and playing, for developing MIDI Synth support, and for being a great friend in general.

Without you all, this wouldn't be possible. Thank you!

## Sound Asset Credits
> To be honest, I don't fully remember which assets have been used, especially the sound assets as different piano soundfonts were used in each MIDI Program. However, I only remember the ones who made them.

Special thanks to the following:
1. [MBMS Productions](https://www.youtube.com/@MBMS) - For their contributions to the Soundfont Community, and for developing iconic soundfonts such as the A9 Soundfont, Amethyst Grand Soundfont, and the CFaz Soundfont.

2. [Maxime Abbey of Arachnosoft](https://www.arachnosoft.com/main/download.php?id=soundfont-sf2) - For the creation of the Arachno Soundfont, which in my opinion is a widely-used soundfont (at least, back then) for Black MIDIs utilizing instruments! Especially for the Drum Instruments, in which it originated from the Arachno Soundfont.

## Visual Asset Credits
Save for the Scratch Piano From Above Project, which was inspired by [Piano From Above by Brian Pantano](https://github.com/brian-pantano/PianoFromAbove), most of my textures, including that of the Fonts used, were made by me.

The Palette Menu in the Aranara MIDI Render Toolkit is developed by me.

## Plugin Credits
Special thanks to the following for making my projects possible:
1. [GarboMuffin](https://scratch.mit.edu/users/GarboMuffin/#comments) - For developing TurboWarp, the framework for my Aranara MIDI Programs, as well as several of the plugins they have created for TurboWarp.
2. [CST1229](https://scratch.mit.edu/users/CST1229/), [BludIsAnLemon](https://scratch.mit.edu/users/BludIsAnLemon/), and [Man-o-Valor](https://scratch.mit.edu/users/man-o-valor/) - For the Text Plugin
3. [TrueFantom](https://scratch.mit.edu/users/TrueFantom/) - For the Base and Math Plugins
4. [ObviousAlexC](https://scratch.mit.edu/users/pinksheep2917/) - For the Pen Plus V7 and the Sensing Plus Plugins 
5. [LilyMakesThings](https://scratch.mit.edu/users/LilyMakesThings/) - For A LOT of the Plugins used in my MIDI Programs, such as the Clones Plus, Looks Plus, More Events, and List Tools Plugins.
6. [XeroName](https://scratch.mit.edu/users/plant2014/) - For the Delta Time Plugin

## Disclaimer
Feel free to contact me through my email, [Scratch Profile](https://scratch.mit.edu/users/OjasnGamer101/), and [Daniferousity Discord Server](https://discord.gg/kTD8y6YDjJ), if you have not been included in this Credits list. This list is not 100.00...00% exhaustive, and I might have forgotten some bits and pieces here and there. I'd appreciate it if you point out any corrections. Thank you!

## Conclusion
Man, being curious about everything really leads to things like these. I spent a good chunk of my life doing projects like these and I have no regrets. I learned new things, met new wonderful people, and made good memories. These are the things I will continue to cherish throughout my life, and I hope to continue to make random stuff like these in the future.

But yeah, stay curious and be creative. Perhaps you may come up with a breakthrough that can change everything for the better!

And thank you so much for taking your time to read this. It means a lot to me that I am able to voice out my thoughts and to give credit where it is due. I hope that you would do the same, not just to me but to everyone who has helped you.

This has been very long, oops...

---

>[Back to top](https://daniferous.github.io/aranara-midi-player-sb3/credits)

---

# Navigation Portal

>[Main Page](https://daniferous.github.io/aranara-midi-player-sb3)

>[Aranara MIDI Programs and MIDI Specifications](https://daniferous.github.io/aranara-midi-player-sb3/versions)

>[Lurker of the Lost Game](https://daniferous.github.io/aranara-midi-player-sb3/lostlurkergame)

>[Guidelines for Proper Usage](https://daniferous.github.io/aranara-midi-player-sb3/guidelines)

>[Program Credits](https://daniferous.github.io/aranara-midi-player-sb3/credits)