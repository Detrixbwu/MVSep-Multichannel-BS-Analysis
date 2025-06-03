# 🧠 MVSep Multichannel BS – Behavioral Overview

This document contains a deeper look at how the model separates audio channels from multichannel formats such as Dolby Atmos.

## 🔄 Input Used for Testing

- Format: Dolby Atmos (E-AC-3 JOC, 768 kb/s)
- Source: TIDAL (downloaded via orpheus.py)
- Channels: 6
- Sample rate: 48.0 kHz

## 🧪 Testing Summary

During multiple tests using Dolby Atmos music, the model consistently returned:

- 6 vocal channels
- 6 instrumental channels

Even though the input was 6-channel Atmos, the model appears to **duplicate and isolate** different elements into vocal/instrumental stems with separate 6-channel layouts.

### Vocal Channel Behavior

| Channel | Observations                             |
|---------|------------------------------------------|
| 1 & 2   | Most prominent, stereo-panned vocals     |
| 3       | Intermediate mono blend                  |
| 4       | Empty (consistently across tests)        |
| 5 & 6   | Alternative stereo channels (e.g. harmonies, backing vocals) |

### Instrumental Channel Behavior

| Channel | Observations                          |
|---------|---------------------------------------|
| 1 & 2   | Main instruments (melody, guitars)     |
| 3       | Drums (with some bass overlap)        |
| 4       | Isolated bass                         |
| 5 & 6   | Additional melodic or stereo elements  |

These layouts are based on personal testing and may vary slightly depending on the song structure.
