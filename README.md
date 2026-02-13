DITHER PRO // ULTIMATE


[<iframe width="560" height="315" src="https://www.youtube.com/embed/dPQaT50aZWI?si=HkT3gQtNOV7aD1MT" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
](https://youtu.be/dPQaT50aZWI?si=4k5s1q4JWMiFhkhE)

A high-performance, single-file WebGL workstation for retro image processing, dithering, and professional color grading. This tool runs entirely in the browser using the GPU, requiring no installation or external dependencies.

## Overview

Dither Pro is designed for pixel artists, broadcast designers, and datamosh enthusiasts. It processes images and video in real-time, converting high-fidelity signals into restricted palettes using various dithering kernels and procedural text generation.

## Key Features

### Core Engine
*   **Hard-Lock Resolution:** Canvas physically resizes to match source aspect ratio exactly. Eliminates bleeding and borders.
*   **WebGL 1.0/2.0 Compatible:** Runs locally on the GPU.
*   **Batch Processing:** Queue multiple images for automated processing and export.

### Colorist Suite
*   **L.G.G. Workflow:** Industry-standard Lift (Shadows), Gamma (Midtones), and Gain (Highlights) controls.
*   **White Balance:** Adjustable Temperature (Warm/Cool) and Tint (Magenta/Green).
*   **LUT Engine:** 15+ cinematic and utility Look Up Tables with opacity mixing (0-100%).
    *   Profiles: Kodak Portra, Gold, Fuji Velvia, CineStill, Matrix, Dune, Thermal, Night Vision.

### Dither & Texture
*   **Error Diffusion:** Floyd-Steinberg, Atkinson, Stucki.
*   **Ordered Dither:** Bayer matrices (2x2 up to 16x16).
*   **Procedural Text:** Generates dynamic ASCII/Text layers based on luminance.
*   Modes: English, Katakana (Japanese), Hanzi (Chinese/Kanji), Runic, Binary.
*   **Shape Algorithms:** Blue Noise, White Noise, Halftone Dots, Halftone Lines, Voronoi.

### Audio Reactivity
*   Microphone integration analyzes volume to modulate visual parameters in real-time.
*   Modulation Targets: Glitch Offset, RGB Split, Dither Threshold, Hue Shift.

### Export
*   **Images:** PNG (Lossless), JPG (Web).
*   **Video:** Native MP4 (H.264) and WebM (VP9) recording capabilities.

## Installation

1.  Download the `DitherPro_Ultimate.html` file.
2.  Open the file in any modern web browser (Chrome, Edge, Brave, Firefox).
3.  No server, Node.js, or Python required.

## Usage Guide

### 1. Input Deck
*   **Load File:** Import single images or video files.
*   **Webcam:** Initialize live camera feed.
*   **Batch:** Import multiple images. Use "Batch Run" to process and auto-download.

### 2. Resolution
*   **Native:** Matches source resolution 1:1.
*   **Fixed Width:** Locks width (e.g., 320px) and calculates height based on aspect ratio.
*   **Downscale:** Divides source resolution by a factor (1x - 16x).
*   **Pre-Blur:** Softens input before dithering to reduce noise artifacts.

### 3. Pro Colorist
*   **LUT Profile:** Select color preset.
*   **Mix:** Blend between source color and LUT.
*   **Lift/Gamma/Gain:** Standard color grading controls.
*   **Temp/Tint:** Correct white balance.

### 4. Quantizer (Palette)
*   **True Color:** 32-bit color depth (bypasses palette).
*   **Library:** Select from preset retro consoles (CGA, Gameboy, Macintosh, etc.).
*   **Auto Extract:** Uses K-Means approximation to pull colors from the current image.
*   **1-Bit:** Pure monochrome thresholding.

### 5. Dither Kernel
*   **Algo:** Select the mathematical pattern for pixel distribution.
*   **Threshold/Amt:** Controls the contrast/intensity of the dither mask.
*   **Scale:** Increases the size of the dither pattern relative to the pixel grid.

### 6. Post Process
*   **Sobel Edge:** Detects edges and renders outlines.
*   **Scanline:** Simulates CRT interlace lines.
*   **Bloom:** Adds luminance glow to bright areas.
*   **Chromatic Ab:** Separates RGB channels horizontally.
*   **Ghost Trail:** Temporal blending with previous frames.

### 7. Audio Link
*   **Link Microphone:** Requests browser permission for audio input.
*   **Gain:** Input sensitivity multiplier.
*   **Target:** Selects which FX parameter reacts to volume peaks.

### 8. Export Lab
*   **Save PNG/JPG:** Instant snapshot of current frame.
*   **Video Format:** Select container/codec (MP4 or WebM).
*   **Start Recording:** Captures the canvas stream. Press again to stop and download.

## Compatibility

*   **Chromium (Chrome, Edge, Brave):** Full support including MP4 export.
*   **Firefox:** Full support (MP4 export depends on OS codecs, falls back to WebM).
*   **Safari:** WebGL supported. Video export formats may vary.

## License

MIT License. Free to use, modify, and distribute.
