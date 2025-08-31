## Garem SG-122

This was the company's first shot at budget soundcards.
The card was based around 22-channel ES5506: 16 Melodic and 6 Rhythm voices.
Melodic instruments are fully customizable, while drum kits
are limited to editing ADSR. Also custom drum kits cannot
replace built-in ones, only loaded as custom melodic instruments.
Mapping of built-in drum kits is proprietary, although it is
semi-compatible to MIDI mapping, thanks to SGS2MID drivers,
which automatically remap inputted MIDI channel 10 data to
SG-122 Rhythm data.
There is a cost-reduced variation of soundcard, the Garem SG-122R.
using ES5503 to reduce it's cost. This variant has 12 Melodic
channels and 4 Rhythm voices. And also abuses bankswitching
and does streaming for long samples that do not fit within 16KiB
part of memory. The cost-reduced version also uses wavetable
instruments instead of sample-based ones.

## FEATURES
### SG-122
* Hardware Filters
* Large amount of sample RAM is built-in
* 4 Drum Kits:
  - Standard / Power
  - Jazz / Brush
  - TR-808 / TR-909
  - Orchestra / Ethnic (Extra)
* Partial compatibility to MIDI protocol 
* Ability to simultaneously use several sound cards to enhance sound
* Yamaha YMF289B (OPL3-L) and Yamaha YMZ280B (PCMD8) sound expansions can be used
* Technically compatible to all of the OPL/OPN series, and also Yamaha YM2151 (OPM), Yamaha YM2414 (OPZ) thanks to unofficial drivers.
### SG-122R
* No filters
* Only 16 KiB of memory available
* 1 Drum Kit: Standard
* Partial compatibility to MIDI protocol
* Wavetable sounds instead of samples for melodic instruments.
* Streaming for long sounds