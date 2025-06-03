# 🎧 MVSep Multichannel BS - Unofficial Technical Analysis

> This repository provides a detailed, research-based overview of the **MVSep Multichannel BS** model for audio source separation from multichannel formats like 5.1, 7.1, and Dolby Atmos. There is no official documentation available at the time of writing — all insights are based on our own tests and observations.

## 🔍 What is MVSep Multichannel BS?

**MVSep Multichannel BS** is an advanced machine learning model designed to separate vocals and instrumental elements from **multichannel audio** such as:

- 5.1 Surround Sound
- 7.1 Surround Sound
- Dolby Atmos (E-AC-3 JOC)
- Any multichannel format beyond stereo

The model emphasizes **lossless processing** and **maintains the original number of channels and sample rate** of the input.

## 🎛 Output Structure

When tested with Dolby Atmos tracks (e.g. from TIDAL), the model consistently outputs:

- **6 vocal channels**
- **6 instrumental channels**

Each group is delivered as a **6-channel FLAC file** (or other format of choice). Typical output specs: FLAC, 48.0 kHz, 24 bits, 6 channels, ~3 342 kb/s

## 🧪 Behavior Summary

> ⚠️ Channel 4 in the vocal output is often empty. This behavior was consistent across multiple tests and might reflect characteristics of Dolby Atmos mixing, not an error in the model.

### Key Observations

- **Vocal and instrumental elements are spatially distributed.** Panning and separation between lead vocals (e.g. Camila) and other singers (e.g. Shawn) were preserved.
- **Instrumental stems are clearly structured:** low-end elements like bass appear isolated in specific channels, while others retain stereo guitar, drums, or melody components.
- **Minimal quality degradation.** The model introduces almost no audible artifacts.

You can find a detailed technical breakdown in [`analysis/behavior-overview.md`](analysis/behavior-overview.md).

## 📂 Output Formats

Supported output formats include:
- FLAC
- WAV
- M4A
- MP3

## 📎 Disclaimer

There is **no official documentation** for this model as of June 2025. All behavior described is the result of hands-on testing. If future documentation is released, this repository will be updated accordingly.

## 📢 Contributions

If you’ve tested this model with other tracks or formats and observed different behaviors, feel free to open an issue or pull request. Let’s document this together.
