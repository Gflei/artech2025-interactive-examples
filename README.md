# Interactive Sound Examples

This repository contains interactive sound examples from the article "Decompose/Recompose the Soundscape: Aesthetic experimentation using spectral manipulation techniques in immersive soundscape composition".

## File Structure

```
InteractiveExamples/
├── index.html                 # Main page with spectrogram-only players
├── styles.css                 # Styles for layout and components
├── archive/                   # Archived examples and documentation stubs
├── LICENSE
├── README.md                  # This file
└── audio/                     # Audio files directory
    ├── MonteAhava2.ogg
    ├── 1_SpectraeqTest12_MonteAhava2Fix.ogg
    ├── 4_monteahava2_Autoconvolutionx1.ogg
    ├── 16_SpectraeqTest9_MonteAhavaSoundscape2.ogg
    ├── EditingRomeAmbience_Phonography_SpanishStairs2ViaDelCorso.ogg
    ├── 2_SpectraeqTest21_RomeViaDelCorsonicely.ogg
    ├── vilaRealAmbience1Binaural.ogg
    ├── 10_SpectraeqTest11_VilaRealFix.ogg
    ├── 11_SpectraeqTest13_VilaRealFixerLow.ogg
    ├── StopDemostrationEdit.ogg
    ├── 13_SpectraeqTest23_STOP.ogg
    └── 14_SpectraeqTest3_STOP Demonstration Drummers.ogg
```

## How to Use

1. Open `index.html` in a modern web browser
2. Click on any spectrogram to play/seek; use Play/Pause buttons
3. Only one track plays at a time (others auto-pause)

Archived examples are in `archive/` and are kept for documentation only.

## What You’ll See

- Vertical red progress scroller synced to playback
- Grouped examples by recording/composition

## Technical Details

- WaveSurfer.js v7 (ES module import from CDN)
- Spectrogram plugin settings:
  - height: 550
  - scale: mel
  - frequencyMin: 35, frequencyMax: 20000
  - fftSamples: 2048
  - rangeDB: 60, gainDB: 20
  - color map: hot
  - useWebWorker: true
  - maxCanvasWidth: 4000 (tiling for performance)

## Performance Notes

- Uses Web Workers for FFT computation
- Canvas tiling prevents oversized canvases on long files

## Troubleshooting

If audio doesn't play or the page feels slow:
1. Hard refresh the page (Ctrl+F5) to bypass cache
2. Ensure your browser supports .ogg playback
3. Try closing other heavy tabs
4. Optionally lower `fftSamples` to 1024 in `index.html`

## Full Album

The complete album "Decompose/Recompose the Soundscape" is available on Bandcamp:

[Listen on Bandcamp](https://guyfleisher.bandcamp.com/album/decompose-recompose-the-soundscape)

## Credits

- WaveSurfer.js: https://wavesurfer.xyz/
- Audio Processing: Spectral manipulation techniques
- Field Recordings and Album: [Decompose/Recompose the Soundscape by Guy Fleisher](https://guyfleisher.bandcamp.com/album/decompose-recompose-the-soundscape)

