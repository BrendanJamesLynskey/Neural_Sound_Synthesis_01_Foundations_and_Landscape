# Neural Sound Synthesis · Part 1 — Foundations & the Landscape

The opening part of the [Neural Sound Synthesis](https://github.com/BrendanJamesLynskey/Neural_Sound_Synthesis) series. Builds the vocabulary of the whole field: why generating audio is uniquely hard, the four representation domains a model can work in, the five generative-model families, and how synthesis quality is measured.

### [Launch App](https://brendanjameslynskey.github.io/Neural_Sound_Synthesis_01_Foundations_and_Landscape/)

Part of the [DSP & Music](https://github.com/BrendanJamesLynskey/DSP_and_Music) collection.

---

## What's inside

| Section | Content |
|---------|---------|
| **The Problem** | Dimensionality of audio, the long-range-dependency problem, why next-sample prediction is costly |
| **Four Domains** | Raw waveform ↔ spectrogram ↔ discrete tokens ↔ continuous latent — with a **live demo showing one clip in all four** |
| **Quantization** | μ-law companding, the 6 dB/bit rule, derivations — with a **live μ-law vs linear listener** at 2–8 bits |
| **Long Context** | Dilated causal convolutions, exponential receptive field — with an **interactive dependency-cone visualiser** |
| **Model Families** | Autoregressive · GAN · Diffusion · Flow · VAE — objectives, trade-offs, and a **schematic animator** of each |
| **Evaluation** | MOS, MUSHRA, FAD, PESQ, CLAP — the metrics ladder, with the Fréchet Audio Distance derived |
| **Timeline** | The neural era, 2016 → 2024, cross-linked to every later part |

## Live demos (all synthesised in-browser, no audio files)

1. **Domain explorer** — generates a sung vowel / plucked string / drum hit and renders it live as a waveform, a mel spectrogram, a discrete-token sequence (k-means codebook), and a latent trajectory.
2. **μ-law listener** — hear quantization at 2–8 bits with and without companding; see the curve and the SQNR.
3. **Receptive-field playground** — drag layers/kernel and watch the dilated-convolution dependency cone widen exponentially.
4. **Generative-families animator** — watch how AR, GAN, diffusion, flow, and VAE each turn noise/context into a sample.

## Technology

Single-file HTML/CSS/JS · Web Audio API · HTML5 Canvas · KaTeX · Palatino + Lucida Console · No external dependencies · No build step
