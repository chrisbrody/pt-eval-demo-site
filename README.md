# PT Intake — Interactive Demo

A standalone demo page that simulates a PT-patient interview being transcribed and converted into a SOAP note in real time.

**Live:** [chrisbrody.github.io/pt-eval-demo-site](https://chrisbrody.github.io/pt-eval-demo-site/)

## What It Does

- Plays back a sample PT-patient interview (left wrist injury scenario)
- Displays a diarized transcript with speaker labels (PT in blue, Patient in pink)
- Highlights detected keywords color-coded by SOAP section
- Builds the SOAP note in real time as the interview plays
- Runs an AI refinement pass after the interview, polishing each section with clinical language
- Completes in ~20 seconds

## Features

- **Real-time SOAP building** — S/O/A/P sections populate as each sentence is categorized
- **Keyword highlighting** — matched keywords glow in their section color (blue/green/orange/purple)
- **Speaker diarization** — PT and Patient lines are visually distinct
- **AI refinement** — spinner per section, then polished clinical text replaces raw transcript
- **Per-section copy** — hover any SOAP card to copy just that section
- **Full-note copy** — single button copies the entire SOAP note
- **Audio waveform** — animated bars simulate live recording
- **Fade-in animations** — sentences slide in smoothly
- **Early access form** — CTA submits to Make.com webhook

## Tech

Single HTML file. No build step, no dependencies, no backend. All JavaScript is inline. Deploys via GitHub Pages.

## Deployment

Push to `main` on [chrisbrody/pt-eval-demo-site](https://github.com/chrisbrody/pt-eval-demo-site) — GitHub Pages deploys automatically.
