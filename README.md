# ppm-testing
Details of WAV files that can be used to test audio PPMs for conformity to IEC 60268-10 Type II (as used in the BBC)

Link to WAV files: https://www.dropbox.com/sh/pxittrt813vgzum/AADxCvsb3sf-67EPPgSUprRZa?dl=0

PPM Level
File name: PPM Level - PPM 4 (4s), Silence (2s), PPM 1-7 (2s each).wav
This checks that the PPM reads correctly (on the marks of the scale) on continuous 1 kHz tone
- 0:00 4 seconds of PPM 4 (-18 dBFS / 0 dBu) for line-up purposes
- 0:04 2 seconds of silence
- 0:06 2 seconds of PPM 1 (-30 dBFS / -12 dBu)
- 0:08 2 seconds of PPM 2 (-26 dBFS / -8 dBu)
- 0:10 2 seconds of PPM 3 (-22 dBFS / -4 dBu)
- 0:12 2 seconds of PPM 4 (-18 dBFS / 0 dBu)
- 0:14 2 seconds of PPM 5 (-14 dBFS / +4 dBu)
- 0:16 2 seconds of PPM 6 (-10 dBFS / +8 dBu)
- 0:18 2 seconds of PPM 7 (-6 dBFS / +12 dBu)

PPM Integration Time
File name: PPM 10 ms Integration - PPM 4, 6, 5.5, 5, 3.75, 1.75.wav
A BBC PPM should be Type II (10 ms integration time causing a 2dB drop for a 10 ms 5 kHz tone burst)
- 5 seconds of PPM 4 (-18 dBFS / 0 dBu) for line-up purposes
- 100 ms of PPM 6 - should read PPM 6 (0 dB drop)
- 10 ms of PPM 6 - should read PPM 5.5 (2 dB drop)
- 5 ms of PPM 6 - should read PPM 5 (4 dB drop)
- 1.5 ms of PPM 6 - should read PPM 3.75 (9 dB drop)
- 0.5 ms of PPM 6 - should read PPM 1.75 (17 dB drop)

PPM Return Time
File name: PPM 2.8 s Return Time - PPM 7 to 1.wav
This checks that the return time of the PPM is 24 dB in 2.8 seconds (to fall from PPM 7 to PPM 1)
The frequency used for this test is 1 kHz
- 5 seconds of PPM 4 (-18 dBFS / 0 dBu) for line-up purposes
- 0.2 seconds of PPM 7 (-6 dBFS / +12 dBu)
- 2.8 seconds of silence
- meter should just reach PPM 1 before next tone burst arrives
- and repeat ...

https://www.dropbox.com/sh/pxittrt813vgzum/AADxCvsb3sf-67EPPgSUprRZa?dl=0
