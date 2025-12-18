# 🔐 Cancellable Voice Biometrics via Key-Conditioned Deep Audio Steganography

This repository contains the reference implementation for the paper:

**“Cancellable Voice Biometrics through Key-Conditioned Deep Audio Steganography”**  
*(submitted to ICPR 2026)*

---

## Overview

This work presents an end-to-end framework for **privacy-preserving and revocable voice biometrics**.  
Speaker embeddings extracted from a pretrained ECAPA-TDNN network are first transformed using a **key-dependent orthogonal projection** to obtain cancellable templates. These protected templates are then **covertly embedded into benign audio signals** using a **FiLM-conditioned U-Net** operating on log-mel spectrograms.

An auxiliary extractor network recovers the protected templates from the resulting stego audio, enabling standard speaker verification in the protected embedding space while preventing direct exposure of biometric templates.

---

## Key Features

- **Cancellable speaker templates** via key-conditioned orthogonal projections  
- **Deep audio steganography** for covert template embedding  
- **FiLM-conditioned U-Net** for identity-driven hiding  
- **Template recovery network** for protected speaker verification  
- Curriculum training strategy balancing **template fidelity** and **imperceptibility**  
- Evaluation on **LibriSpeech** (speaker identity) with **MUSAN** as benign cover audio  

---

## Repository Status

The codebase is currently being prepared for public release.

The repository will include:
- Training and evaluation scripts  
- Model definitions for the hiding and recovery networks  
- Speaker verification and metric computation utilities  
- Instructions for dataset preparation and reproduction of results  

The final version will be released in conjunction with the conference submission.

---

## Citation

If you find this work useful, please cite the corresponding paper (citation to be added).
