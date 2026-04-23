# Garem SS-16

Garem SS-16 is a professional sound synthesizer.
Available in 38, 68, 88 and full 128 key layout.
Was made in early 2000s.

Garem SS-16 is a combo of FM and PCM synthesizers in one shell,
developed by Garem and Yamaha.
In total, there are 24 FM and 32 PCM voices available.

Usually the synthesizer comes with an additional `Built-in Sounds`
expansion card, that contains, well, the default samples for the
synth, and a memory card. SS-16 can freely operate without
the `Built-in Sounds` card, but the default PCM sound set will not
be available. As soon as the card is inserted, SS-16 automatically
loads all the default sounds into the ROM, and it only loads those
from the aforementioned card, another expansion card will not work.

Synthesizer is fully compatible with TX81Z, and can load all the
patches from that synth, via either SysEx, MIDI (which also sends SysEx),
or via a USB connection.

Garem SS-16 also has the ability to load additional PCM sounds, via either
Expansion cards or, again, USB, using the corresonding SS-16 Sound Editor,
a desktop application developed by Garem to control various aspects of the
synthesizer.

There is also Garem Syntex32, which is really just 2 SS-16s glued in a single shell.
This was made later in 2010s as hardware got cheaper and customers could afford paying for this synth.

## Compatibility
- Garem SS-16 is compatible with any sound card or synthesizer module
that is using YM2151 "OPM", YM2414 "OPZ" or YM2424 "OPZ2" chips,
as OPZ2 is by itself compatible with OPZ (the only difference being
that OPZ2 has carrier fixed frequency down to 0Hz) and OPZ is fully
compaatible with OPM sound-wise.
- Garem SS-16 is fully compatible with MIDI Level 1 protocol, 
having 24 FM and 32 PCM voices, thus meeting the 24-voice
requirement in both mediums, and it additionally has Bank MSB (CC#0)
and Bank LSB (CC#32) to access up to 128\*256\*256 patches across
256^2 banks.
- Garem SS-16 is compatible with Yamaha's new e**X**tended **G**M protocol.

## Main Features
- Has 4MB (not MiB) of Sample ROM for long-term sample storage.
- 1MB of Sample RAM for storing samples ready for playback.
- Hard-panning for FM channels (as Yamaha always did for FM chips).
- Full panning for PCM channels, with both Left and Right channels having 256 volume steps.
- Compatibility with TX81Z Rack Synthesizer Module.
- Expansion Cards, for additional samples and FM patches. Each card has own Bank LSB corresponding to it.
- 32-symbol 8-line LCD for general text display, 24-charcter 1-line display for other panes.
- RAM expansions!

4MB of Sample ROM can be used to store custom samples.

## Panels
Garem SS-16 is a synthesizer, and thus needs a way to edit sounds.
Thus, there are "panes": modular metallic plates that are mounted
on top of the synth's surface. They are immovable though, and
the customer must explicitly specify the way he wants to arrange
the panes, and pay a little extra for that since the face of the
synth will be custom-made instead of the default layout.


This is how an operator editing pane looks:
```
+--------------------------------------------+
|  [A:31 D:00 S:00 D:00 R:08]    OP Matrix   |
| Atk [O]  [|]   [|]F   [#| ]    [ 1   2 ]   |
| Dec [O]   | T   | B   [#|#]    [ |   | ]   |
| Sus [O]   | L   | C   [#|#]    [ 3   4 ]   |
| De2 [O]   |     | K   [#|#]    [ +>O<+ ]   |
| Rel [O]   |     |     [#|#]  Algorithm [ ] |
| OPx [P] [003]  [5]     V U                 |
+--------------------------------------------+
```
The pane is seen 4 times, as there are 4 operators.
Figures:
- `[O]` is a knob
- `[P]` is a pan switcher. Order: L, C, R
- `[Text]` is a generic display
- `[ ]` is a button
- `[|]` is a vertical slider

NOTE! Feedback is only applied to Operator 1.


This is how cartridge loader and patch screen look:
```
+----------------------------------+
| [001-001. SPACE-VOYAGER ] [SAVE] |
| [-] [+] [@]  [GET] [SEND]        |
| [||||||||||||||||] CARD SLOT     |
| [MEM:023%|OK            ] STATUS |
+----------------------------------+
```
Figures:
- `[-]` `[+]` `[#]` are Patch Subtract, Patch Increase and
Random Patch buttons, are used to change the current patch.
- `[GET]` `[SEND]` are Patch Get and Patch Send options, get or
send the current patch to/from connected PC or another SS-16 synth.
- `[SAVE]` is a save button, writes patch with current settings to current slot.


This is how PCM configurtion screen looks:
```
+--------------------------------------------------+
|  [A:CF D:00 S:00 D:00 R:86]                      |
| Atk [O]  [|]L  [ | ]  PCM SELECT [-] [+] [@]     |
| Dec [O]   | E  [ | ]  [000: NONE               ] |
| Sus [O]   | V  [ |#]  SWITCH PCM BANK [ ]        |
| De2 [O]   | E  [#|#]  BREAKPOINT [O]  PAN [O]    |
| Rel [O]   | L  [#|#]  POINTLO [O]  POINT HI [O]  |
|   PCM   [255]   V U   KEYSHFT [O]  FINETUNE [O]  |
+--------------------------------------------------+
```
Figures:
- `[O]` is still a knob
- `[|]` is still a vertical slider
- `[-]` `[+]` `[@]` are PCM Increase, PCM Decrease and PCM Random
buttons. They select next, previous and random PCM sound respectively.
- `BREAKPOINT` is a knob selecting one of the 16 breakpoints, `0..15`
- `POINTLO` and `POINT HI` are knobs telling the low and high notes of
current breakpoint, `0..127`.
- `KEYSHIFT` and `FINETUNE` are coare and fine tune of current brekpoint sample.
- `SWITCH PCM BANK` is a button that switches current PCM bank from built-in PCM to Card PCM.
- All envelope values, volume and pan are knobs/sliders with range of `0..255`.

Some advanced options, like separate left/right volume of PCM and
Breakpoint Volume Fade are only controllable via software.

## Expansion Cards
There are 8 factory expnsions in total:
- SS160: Factory; Contains base presets.
- SS161: Chromtic Percussion; Adds various chromatics like marimbas, kalimbas, glockens and so on
- SS162: World of Ethnics; Adds varous ethnic percussions like sitar, bongos etc.
- SS163: Woodwinds; Self-explanatory. Adds woodwind instruments
- SS164: TB or not to be?; Adds TB303-like sounds, like acid.
- SS165: SpoT Right in the Spotlight; Adds percussion alike to one of Roland TR series.
- SS166: OPeration no. Six; Adds various presets that sound like DX-7.
- SS167: OPeration Krust; No, the typo here is intended. Adds lo-fi percussion like the one seen in rare Yamaha YM7129 "OPK2" chip, including samples from the ROM of that chip.

Factory PCM presets are:
- 01. Acoustic Grand
- 02. Acoustic Bass
- 03. Slap Bass
- 04. Brass Section
- 05. Saxophone (Alto)
- 06. Vibraphone
- 07. Tububells
- 08. Overdriven Gt.
- 09. Distortion Gt.
- 10. Rhythm Guitar
- 11. Power Chords
- 12. Marimba
- 13. Square Wave
- 14. Saw Wave
- 15. Doctor Solo
- 16. Warm/Sweep Pad
FM Factory patches are made to replicate GM Level 1 collection.

# SOUND CHIPS

## SS16D78-11
The heart of FM Synthesis of SS-16.

It bears:
- 24 FM voices
- 4-operator synthesis
- Hard-pan (Left, Center, Right)

This is an enhanced version of OPZ, so TX81Z patches are fully compatible.
There is nothing much different from OPZ here, other than having 24 voices.

FM Waveforms:
- 1. Sine
- 2. Triangle (Sine^2)
- 3. Half Sine
- 4. Half Triangle
- 5. Even Sine
- 6. Even Triangle
- 7. Even Camel Sine
- 8. Evel Camel Triangle
- 9. Abs Sine
- 10. Abs Triangle
- 11. Quarter Abs Sine  (/_/)
- 12. Quarter Abs Triangle (/_/)
- 13. Quarter Sine (/_\\_)
- 14. Quarter Triangle (/_\\_)
- 15. Square
- 16. Accumulator (aka Sawtooth, aka Derived Sawtooth)
- 17. Abs Accumulator
- 18..32. tbd

## SS16D78-12
The heart of PCM Synthesis of SS-16.

Bears:
- 32 PCM voices
- Hardware AD1SD2R envelope, inherited from Yamaha YMW258-B "Sega MultiPCM"
- 256 volume levels, linear scale, separate L/R level
- Envelope parts have range of 256 steps
- Better hardware LFO, with 256 steps of range, frequency and depth.
- 4 PCM formats: 8-bit, 16-bit, IMA ADPCM and log2 8-bit
- 16 MB sample RAM addressable.

Enhanced version of Sega MultiPCM, having 32 voices.
LFO:
- Pitch range: -2..2 semitones
- Rate: at 12MHz clock speed, rate 0 is 0Hz and rate 255 is 100Hz, linear steps.
- Separate Tremolo and vibrato depth
- 2 LFOs per each PCM Voice

Can access up to 16MB of sample memory,
which is the size Expansion cards usually have.
