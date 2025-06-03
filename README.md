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

Each group is delivered as a **6-channel FLAC file** (or other format of choice). Typical output specs:
