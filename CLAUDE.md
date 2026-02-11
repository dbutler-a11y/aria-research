# ARIA Research

## What This Is
Open-source research initiative for accessible AI-powered companion systems for Parkinson's disease patients. Under $500 using commodity hardware (Raspberry Pi 5). Author: Durayveon Butler.

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
| Model | Cost | Purpose |
|-------|------|---------|
| ARIA Bloom | ~$280 | Tabletop companion, medication reminders |
| ARIA Guide | ~$380 | Walker-integrated gait cueing (laser + audio) |
| ARIA Frame | ~$220 | Digital portrait companion, video calling |
| ARIA Rover | ~$430 | Mobile autonomous companion robot |

## Hardware Platform
- Raspberry Pi 5 (8GB), ReSpeaker 4-Mic Array, Pi Camera Module 3
- AI: Whisper.cpp (speech), Qwen 3:1.7b (LLM, local), Piper (TTS)
- Cloud fallback: Claude API for complex conversations
- Satellite IoT: Swarm, Astrocast

## Related Project
The Claw Protocol Collective (~/open-claw/) — community framework that includes ARIA as a flagship initiative.
