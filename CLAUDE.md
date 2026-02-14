# ARIA Research

## What This Is
Open-source research initiative for accessible AI-powered companion and therapeutic systems. Includes Parkinson's disease companions and therapeutic devices, plus ARIA Heal musculoskeletal diagnostic/therapeutic platform. Under $560 using commodity hardware (Raspberry Pi). Author: Durayveon Butler.

## Repo & Deployment
- **GitHub:** github.com/dbutler-a11y/aria-research
- **Live:** dbutler-a11y.github.io/aria-research/
- **License:** MIT

## Tech Stack
- Static HTML/CSS site (no build step, no framework)
- GitHub Pages deployment (auto from main branch)
- Fonts: Source Serif 4, Inter, JetBrains Mono
- Colors: navy #1a365d, blue #3182ce, orange #dd6b20

## Files
```
index.html               # Landing page (products, videos, overview)
therapeutics.html        # Parkinson's therapeutic devices (Pulse, Glow, Cycle)
aria-heal.html           # ARIA Heal shoulder diagnostic & therapeutic platform
research-lab.html        # Research lab (25+ approaches to Parkinson's)
cancer-research.html     # Cancer cure research (AI-driven unconventional approaches)
research-paper.html      # Academic paper (18 citations, 51KB)
hardware-bom.html        # Interactive bill of materials
connectivity.html        # ARIA Sentinel satellite connectivity
ecosystem.html           # Open core + tokenized model
research-data.html       # Market analysis & investor pitch
support.html             # Donation/sponsor page
aria-designs.png         # Product concept sketches (6.9MB)
aria-guide-video.mp4     # FoG intervention demo
aria-bloom-video.mp4     # Medication reminder demo
```

## Product Variants

### Companions (Parkinson's)
| Model | Cost | Purpose |
|-------|------|---------|
| ARIA Bloom | ~$280 | Tabletop companion, medication reminders |
| ARIA Guide | ~$380 | Walker-integrated gait cueing (laser + audio) |
| ARIA Frame | ~$220 | Digital portrait companion, video calling |
| ARIA Rover | ~$430 | Mobile autonomous companion robot |

### Therapeutics (Parkinson's)
| Model | Cost | Purpose |
|-------|------|---------|
| ARIA Pulse | ~$78 | 40Hz gamma entrainment (light + sound + vibration) |
| ARIA Glow | ~$105 | NIR photobiomodulation helmet (810nm) |
| ARIA Cycle | ~$4 | Forced-exercise cycling controller |

### Musculoskeletal
| Model | Cost | Purpose |
|-------|------|---------|
| ARIA Heal | ~$560 | Shoulder diagnostic & therapeutic platform (ultrasound, EMG, PEMF, PBM, rehab) |

## Color Themes
- Companions: navy #1a365d, blue #3182ce
- Therapeutics (Parkinson's): amber #92400e, orange #dd6b20
- ARIA Heal: teal #0f766e, emerald #0d9488
- Cancer Research: rose #9f1239, crimson #e11d48

## Hardware Platform
- Raspberry Pi 4/5, various sensor/therapeutic hardware per device
- AI: Whisper.cpp (speech), Qwen 3:1.7b (LLM, local), Piper (TTS)
- Cloud fallback: Claude API for complex conversations
- Satellite IoT: Swarm, Astrocast (companions only)

## Related Projects
- The Claw Protocol Collective (~/open-claw/) — community framework
- Parkinson's Therapy Platform (~/parkinsons-therapy-platform/) — Pulse/Glow/Cycle codebase
- Shoulder Therapy Platform (~/shoulder-therapy-platform/) — ARIA Heal codebase
