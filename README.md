# Digitalker Audio Archive

This repository is an audio archive of the National Semiconductor MM54104 Mozer Digitalker speech synthesis integrated circuit system. The system was developed in the late 1970s and early 1980s, and allowed early computer to output remarkably clear human speech by sequencing pre-recorded word ROMs. Multiple ROMs were released with varying vocabularies before the product was discontinued circa 1990.

This repository stores audio recordings of the different ROM chip vocabularies played through the MM54104 chip.

The audio recordings in this repo were generated using a custom Digitalker hardware platform designed by me, [Digichiver](https://github.com/frindaddy/digichiver). All ROM binary files and dictionary.jsons can be found in that repo [in the software folder](https://github.com/frindaddy/digichiver/tree/main/Software).

## How to Use

Each Digitalker word is uploaded as its own `.wav` file. Each ROM's vocabulary is separated into its own folder.

When possible, the file names follow the convention `<index>_<word>.wav`, where `index` is the word address in the word list and `word` is the word name.

Unfortunately, word lists do not exist for all ROMs. In cases where there is no word list, wav files are just stored as `<index>.wav`

## Availible ROMs

| ROM Name | Info |
| :----: | :---: |
| DT1052 | Short word list consisting of 0-9 and "point." Probably shipped as a demo with the MM54104 chip. |
| DVSS | This ROM dump contains all the possible words from the Digitalker Voice Selection Software (DVSS). This National Semiconductor program allowed creation of custom speech ROMs from a vocabulary list of 654 words and sounds. This ROM dump is provided by [@MarkD833](https://github.com/MarkD833). |
| Elevator | Guessing this is a ROM for an elevator controller. Numbers and some status words. |
| Face-off | This is a hockey arcade game from 1983 created by SoftLogic ([link](https://www.arcade-museum.com/tech-center/machine/faceoffh)). I'm not sure if I have all the ROM binary files. The only audio files I can generate seem to be of a crowd cheering at a stadium. |
| Genesis | This is a ROM for an alarm panel manufacturd by Genesis. It has some special words related to security, such as `intruder`, `gun`, and `burglar`. |
| [Harem](https://www.youtube.com/watch?v=ZP5FEuuYfRM) | Harem was a 1983 arcade game released by Italian company I.G.R, their only known output. This ROM is mostly silences with a few arcade related words. |
| Jameco JE520 | This was an expansion card for the Commodore 64 (JE520-CM) or Apple II (JE520-AP) that brought Digitalker voice to home computers. |
| RS-Type2 and Type4 | These ROMs were created and distributed by RS Components in the United Kingdom. They feature a british accent, which is pretty fun. |
| Sensaphone | This ROM was used in Sensaphone remote monitoring autodialers like the Sensaphone 1104. |
| SSR1/2/5/6 | As far as I know, these are the only official ROMs made by National Semiconductor. These have a science/math focus. No one is sure if SSR3 and SSR4 exist. |
| Zaccaria's Scorpion Pinball | ROM used in Zaccaria's *Scorpion* Pinball (not Williams *Scorpion*). |

## Missing Datasheets, ROMs

### Recording Software

The holy grail of Digitalker archiving is the program used to record your own audio and create Digitalker ROM files. If you happen to know where an archive of this software is, please contact me.

### Word Lists

The following ROMs are missing official datasheets and word lists. Files are named to the best of my hearing capability.

- Elevator
- Face-off
- Genesis Alarm Panel
- Harem
- RS-Type2
- RS-Type4
- Sensaphone
- Zaccaria's Scorpion Pinball

### ROMs

- Missing all of Dynamic Logic LTD ROM
- Potentially missing some Face-off words/audio

## ROM Image Sources

ROM images from the Digitalker Digital Voice Selection Software (DVSS) are provided as a courtesy by [@MarkD833](https://github.com/MarkD833) thanks to his invaluable work archiving the DVSS outputs [(link to DVSS repo)](https://github.com/MarkD833/Digitalker-Digital-Voice-Selection-Software). The DVSS images have been converted from Intel HEX to binary files for compatability with the Digichiver hardware.

All other ROM images are sourced from the [Internet Archive](https://archive.org/details/digitalker).
