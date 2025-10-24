# Interactive Sound Examples

This repository contains interactive sound examples from the article "Decompose/Recompose the Soundscape: Aesthetic experimentation using spectral manipulation techniques in immersive soundscape composition".

## Files Structure

```
InteractiveExamples/
├── WavesurferSimplePage.html    # Main HTML file with interactive examples
├── styles.css                   # CSS styling for the page
├── README.md                    # This file
└── audio/                       # Audio files directory
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

1. **Open the HTML file**: Simply open `WavesurferSimplePage.html` in a web browser
2. **No server required**: The page works locally without needing a web server
3. **Interactive features**:
   - Click on any spectrogram to start playback and seek to position
   - Use Play/Pause buttons for control
   - Only one audio plays at a time (others auto-pause)
   - View spectrograms with frequency analysis and progress scroller

## Audio Content

The examples include four main categories:

### 1. Monte Ahava Soundscape (Alentejo)
- Original field recording
- Three manipulated versions using spectral techniques

### 2. Soundwalk Field Recording (Spanish Stairs to Via Del Corso, Rome)
- Original binaural recording
- Spectral manipulation composition

### 3. Vila Real Soundscape (Binaural)
- Original binaural recording
- Two manipulated versions with different spectral processing

### 4. STOP Demonstration Field Recording
- Original field recording
- Two manipulated versions demonstrating spectral techniques

## Technical Features

- **WaveSurfer.js**: Interactive spectrogram visualization with progress scroller
- **Spectrogram Analysis**: Real-time frequency analysis with classic colormap
- **Optimized Performance**: 
  - Web Worker for FFT calculations
  - Optimized FFT settings (1024 samples)
  - Mel scale frequency analysis
  - Limited frequency range (0-8kHz) for performance
- **Responsive Design**: Works on desktop and mobile devices
- **Local Audio Files**: All examples use local .ogg files

## Browser Compatibility

- Modern browsers with ES6 module support
- Chrome, Firefox, Safari, Edge (recent versions)
- Requires JavaScript enabled

## Performance Notes

The page is optimized for fast loading and smooth interaction:
- FFT calculations run in background threads
- Single canvas spectrograms (no splitting)
- Optimized frequency range for human hearing
- Efficient memory usage

## Troubleshooting

If audio doesn't play:
1. Check that all audio files are in the `audio/` folder
2. Ensure your browser supports .ogg format
3. Check browser console for any error messages
4. Try refreshing the page

## Full Album

The complete album "Decompose/Recompose the Soundscape" is available on Bandcamp:

[![Decompose/Recompose the Soundscape](https://bandcamp.com/EmbeddedPlayer/album=144355698/size=large/bgcol=ffffff/linkcol=0687f5/tracklist=false/transparent=true/)](https://guyfleisher.bandcamp.com/album/decompose-recompose-the-soundscape)

**Listen to the full album**: [https://guyfleisher.bandcamp.com/album/decompose-recompose-the-soundscape](https://guyfleisher.bandcamp.com/album/decompose-recompose-the-soundscape)

## Credits

- **WaveSurfer.js**: https://wavesurfer.xyz/
- **Audio Processing**: Spectral manipulation techniques
- **Field Recordings**: Original compositions and manipulations
- **Album**: [Decompose/Recompose the Soundscape by Guy Fleisher](https://guyfleisher.bandcamp.com/album/decompose-recompose-the-soundscape)
