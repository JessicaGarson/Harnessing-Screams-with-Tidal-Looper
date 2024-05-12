# Harnessing Screams with Tidal Looper

This repository contains code samples that accompany the blog post "Harnessing Screams with Tidal Looper" on getting started with Tidal Looper.

## Prerequisites

You follow along along ensure you have the following:

- **SuperCollider**: The platform for audio synthesis and algorithmic composition.
- **TidalCycles**: The language for live coding patterns.
- **Microphone with connection to your computer**: Necessary for vocal inputs.

## My Setup

Here's what I currently use for my performances:

- **Motu M4 Audio Interface**
- **Shure SM-52 Microphone with a Switch**: The switch is crucial as it helps manage feedback during performances, allowing for dynamic control.

### Initial Setup

Before you start, configure your audio system to recognize your audio interface or the connection method of your microphone as the primary audio input.

## Why Tidal Looper?

Tidal Looper integrates seamlessly within TidalCycles, enabling live sampling without the need to switch between different software. It emulates a traditional looping pedal with functionalities such as:

- **Recording**: Capture audio in real-time.
- **Replace Mode**: Overwrite existing loops with new audio.
- **Overdub Mode**: Layer additional sounds over existing loops.

## Installation Guide

### Step 1: Download Tidal Looper

Clone or download the Tidal Looper repository from GitHub.

### Step 2: Install as SuperCollider Quark

1. In SuperCollider, go to **Language > Quarks**.
2. Choose **Install a folder** and select the Tidal Looper folder.

### Step 3: Setting up SuperCollider

Create a new file named `start_looper.scd` with the following content:

```SuperCollider
~dirt = SuperDirt.start;
~looper = TidalLooper(~dirt);
