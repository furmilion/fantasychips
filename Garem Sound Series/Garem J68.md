## Garem J68

Ok, so what the hell is that?

Garem J68 is a very obscure multipurpose metal box.
Barely anything is known about it.
It appeared as silently as it went away.
No certain release year is known, but it is assumed that it was somewhere in early 1990s through late 2010s.
This is both a console and an audio workstation.

## CPU
Most likely is a custom-made one, or a modified Z80 to be a 16-bit CPU.
Clock: 16.363MHz
Controls: APU, Video CPU

## APU
* 20 voices of 12-bit PCM.
* No native 12-bit PCM support, only 8- or 16-bit PCM.
* Output rate: 32KHz Mono, 16KHz Stereo.
* Sample header is 32 bytes and has the following data:
  * Sample length: 16 bits, 131072 samples max, sample length is always even.
  * Sample loop start: 16 bits, 131072 max, loop start is always even.
  * Center frequency: 18 bits, 262144Hz max. This is frequency at which sample will play when C-5 is triggered.
  * Additional 14 bits: Flags.
    * Bit 1: Sample type (0: 8-bit, 1: 16-bit)
    * Bit 2: Interpolation (0: Off, 1: Linear)
    * Bit 3: Reverse
    * Bit 4: Ping-pong loop
    * Bit 5: Reverse loop
    * Bits 6-9: Envelope rate scaling
    * Bit 10: Exp volume
    * Bit 11: Exp Attack
    * Bit 12: Exp Decay 1
    * Bit 13: Exp Decay 2
    * Bit 14: Exp Release
  * Attack: 4 bytes, unsigned. Shortest attack: 0, 0ms. Longest attack: 4294967296, 180000ms.
  * Decay 1: 4 bytes, unsigned. Shortest decay: 0, 0ms. Longest decay: 4294967296, 180000ms
  * Sustain: 4 bytes, unsigned. Highest sustain: 0, 0db. Lowest sustain: 4294967296, -144db.
  * Decay 2: 4 bytes, unsigned. Shortest decay: 0, 0ms. Longest decay: 4294967296, 180000ms
  * Release: 4 bytes, unsigned. Shortest release: 0, 0ms. Longest release: 4294967296, 180000ms
  * Sample position in ROM: 4 bytes, always even.

## Video
* 320i60
* Clock: 16.384MHz