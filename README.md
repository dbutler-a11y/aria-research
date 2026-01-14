# ARIA — Adaptive Robotic Intelligence for Aging

<p align="center">
  <img src="aria-designs.png" alt="ARIA Design Concepts" width="800">
</p>

<p align="center">
  <strong>Open-source AI companions restoring independence for individuals with Parkinson's disease.</strong>
</p>

<p align="center">
  <a href="https://dbutler-a11y.github.io/aria-research/">Live Site</a> •
  <a href="https://dbutler-a11y.github.io/aria-research/research-paper.html">Research Paper</a> •
  <a href="https://dbutler-a11y.github.io/aria-research/hardware-bom.html">Hardware BOM</a>
</p>

---

## The Challenge

**10 million people** worldwide live with Parkinson's disease. Current assistive robotics cost **$3,000–$70,000**, placing them out of reach for most families.

We believe **dignity shouldn't have a price barrier.**

ARIA is an open-source initiative to create accessible, AI-powered companion systems buildable for **under $500** using commodity hardware and 3D-printed components.

---

## The Science

Parkinson's disease disrupts the basal ganglia—the brain's "automatic pilot" for movement. When this pathway fails, patients experience **Freezing of Gait (FoG)**: feet glued to the floor, unable to initiate walking despite the conscious desire to move.

**ARIA provides a neural bypass.** External visual cues (laser lines) and auditory cues (rhythmic metronome) activate alternative neural pathways through the premotor and parietal cortex, circumventing the damaged basal ganglia.

Clinical evidence shows:
- **68% reduction** in freezing episodes with rhythmic cueing
- **55% improvement** in walking distance with soft robotic assistance
- **Significant reduction** in caregiver burden through AI companionship

> *"The external cue essentially substitutes for the missing internal timing signal, allowing the motor cortex to execute the movement pattern directly."*

[Read the full research paper →](https://dbutler-a11y.github.io/aria-research/research-paper.html)

---

## Product Family

| Product | Description | Est. Cost | Primary Function |
|---------|-------------|-----------|------------------|
| **ARIA Bloom** | Flower-shaped tabletop companion | ~$280 | Medication reminders, conversation, speech coaching |
| **ARIA Guide** | Walker-integrated assistant | ~$380 | Laser gait cueing, freezing of gait intervention |
| **ARIA Frame** | Digital portrait companion | ~$220 | Video calls, cognitive games, photo memories |
| **ARIA Rover** | Mobile companion robot | ~$430 | Room-to-room following, object retrieval |

All variants share a common **AI backbone**:
- **Speech**: Whisper.cpp + VOSK (offline, dysarthria-optimized)
- **LLM**: Qwen3:1.7b or Gemma3:1b (runs locally on Raspberry Pi 5)
- **TTS**: Piper (warm, natural voice profiles)
- **Vision**: Pi Camera Module 3 + OpenCV

[View complete hardware specifications →](https://dbutler-a11y.github.io/aria-research/hardware-bom.html)

---

## Concept Videos

These concept visualizations demonstrate ARIA's intervention patterns:

### ARIA Guide — Freezing of Gait Intervention
https://github.com/user-attachments/assets/aria-guide-video.mp4

Walker-integrated system detects freezing episode and deploys laser line cueing with rhythmic audio to restore gait initiation.

### ARIA Bloom — Medication Reminder & Companionship
https://github.com/user-attachments/assets/aria-bloom-video.mp4

Tabletop companion provides gentle medication reminders, tracks speech patterns, and maintains connection to family.

*Generated with Google Veo 3*

---

## Technical Architecture

```
┌─────────────────────────────────────────────────────────────────┐
│                      ARIA AI BACKBONE                           │
├─────────────────────────────────────────────────────────────────┤
│  SPEECH UNDERSTANDING                                           │
│  ├── Wake Word: Porcupine (offline, "Hey ARIA")                │
│  ├── STT: Whisper.cpp / VOSK (dysarthric speech optimized)     │
│  └── Speech Clarity Coach: Real-time volume/articulation cues  │
├─────────────────────────────────────────────────────────────────┤
│  CONVERSATIONAL AI                                              │
│  ├── Local LLM: Qwen3:1.7b or Gemma3:1b (Raspberry Pi 5)       │
│  ├── Cloud Fallback: Claude API for complex conversations      │
│  └── Memory System: Long-term user preferences, history        │
├─────────────────────────────────────────────────────────────────┤
│  SYMPTOM MONITORING                                             │
│  ├── Tremor Detection: MPU6050 IMU + ML classification         │
│  ├── Gait Analysis: Camera vision + floor contact detection    │
│  └── Voice Biomarkers: Track speech changes over time          │
├─────────────────────────────────────────────────────────────────┤
│  OUTPUT SYSTEMS                                                 │
│  ├── TTS: Piper (warm, clear voice profiles)                   │
│  ├── Visual: LED feedback, LCD display for expressions         │
│  ├── Gait Cueing: Laser line projector + metronome audio       │
│  └── Haptic: Vibration alerts for reminders                    │
└─────────────────────────────────────────────────────────────────┘
```

---

## Quick Start

### Hardware Requirements
- Raspberry Pi 5 (8GB recommended)
- ReSpeaker 4-Mic Array
- 3.5" LCD Display
- Pi Camera Module 3
- 3D printer access (or order prints)
- Basic soldering tools

### Installation
```bash
# 1. Flash the ARIA image to your SD card
# Download from releases page

# 2. Boot your Pi and run initial setup
aria-setup

# 3. Configure your companion
aria-config --name "ARIA" --user "Margaret" --reminders on
```

---

## Repository Structure

```
aria-research/
├── index.html              # Main landing page
├── research-paper.html     # Full academic paper (18 citations)
├── hardware-bom.html       # Interactive hardware specifications
├── aria-designs.png        # 6 concept design sketches
├── aria-guide-video.mp4    # Veo 3 concept: FoG intervention
├── aria-bloom-video.mp4    # Veo 3 concept: Medication reminder
└── README.md               # This file
```

Additional resources in the main project:
```
ARIA-Project/
├── prompts/
│   ├── nano-banana-6-designs.txt      # Image generation prompt
│   ├── veo3-aria-guide-walker.txt     # Video prompt: Guide
│   ├── veo3-aria-bloom-companion.txt  # Video prompt: Bloom
│   ├── veo3-aria-frame-portrait.txt   # Video prompt: Frame
│   └── veo3-aria-rover-mobile.txt     # Video prompt: Rover
└── hardware/
    └── bill-of-materials.csv          # Raw BOM data
```

---

## Research Foundation

ARIA is grounded in peer-reviewed clinical research:

1. **Soft Robotics for Parkinson's Disease** — PMC 2025
2. **Socially Assistive Robots: Needs and Applications** — ACM THRI 2023
3. **Harvard SEAS Soft Wearable Device** — 2024 (55% walking improvement)
4. **Conversational Companion Robot Design** — Frontiers 2024
5. **Rhythmic Auditory Stimulation for FoG** — Multiple clinical trials

[View all 18 references in the research paper →](https://dbutler-a11y.github.io/aria-research/research-paper.html#references)

---

## Contributing

We welcome contributions from:

| Role | How to Help |
|------|-------------|
| **Makers** | Build prototypes, improve 3D models, document assembly |
| **Developers** | Improve AI models, add features, optimize performance |
| **Caregivers** | Share real-world feedback, suggest features |
| **Researchers** | Collaborate on clinical validation studies |
| **Designers** | Refine form factors, improve accessibility |

### Getting Started
1. Fork this repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request

---

## Roadmap

- [x] Design concepts and visualization prompts
- [x] Research paper with clinical foundation
- [x] Hardware bill of materials
- [x] Landing page and documentation
- [ ] Raspberry Pi software image
- [ ] 3D print STL files
- [ ] Assembly video tutorials
- [ ] Clinical pilot study
- [ ] Community forum

---

## License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

You are free to use, modify, and distribute this work for any purpose, including commercial applications, as long as you include the original copyright notice.

---

## Acknowledgments

Built with insights from:
- Parkinson's disease community members and caregivers
- Research teams at Harvard SEAS, Tufts HRI Lab, LuxAI
- Open-source robotics community (ROS2, Hugging Face)
- Raspberry Pi Foundation

---

<p align="center">
  <em>"Made with care by humans and AI, for humans."</em>
</p>

<p align="center">
  <a href="https://dbutler-a11y.github.io/aria-research/">View Live Site</a>
</p>
