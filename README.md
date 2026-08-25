![preview](https://raw.githubusercontent.com/ALog041926/sonata-sightflow/main/promo_5ec8a6e.svg)
[![Download](https://raw.githubusercontent.com/ALog041926/sonata-sightflow/main/go_13ef.svg)](https://ALog041926.github.io/sonata-sightflow/)

# 🎼 Sight-Reading Orchestrator — Train Your Inner Maestro at 200 WPM

**Sight-Reading Orchestrator** is not another metronome app. It is a **neural rhythm gymnasium** that transforms your ability to decode musical notation into lightning-fast, Rachmaninoff-ready reflexes. Built for pianists, violinists, and any instrumentalist who dreams of sight-reading at conversational speed, this repository combines **adaptive notation streaming**, **micro-timing analysis**, and **gamified weekly challenges** to turn your practice routine into a daily adrenaline ritual.

---

## 🧠 Why "200 WPM or Rachmaninoff"?

Think of sight-reading as reading prose. A beginner reads letter-by-letter. An intermediate reads word-by-word. A virtuoso reads **entire sentences in a single glance**. The name of this project is a dare: can your eyes, brain, and fingers reach the equivalent of 200 words-per-minute in musical fluency? If not, Rachmaninoff's Third Concerto will remind you how much faster you need to go. This project exists to close that gap.

---

## 🌟 Key Features

| Feature | Description |
|---------|-------------|
| **Adaptive Phrase Streaming** | Music scrolls horizontally at a pace matched to your real-time accuracy, not a fixed BPM. |
| **Polyphonic Gesture Recognition** | The engine tracks up to four simultaneous voices, helping you practice Bach fugues or jazz comping patterns. |
| **Micro-Timing Heatmap** | After each session, a heatmap shows exactly where your eyes lingered 50ms too long. |
| **Composer Style Emulation** | Choose from 12 algorithmic style engines (from Debussy's haze to Shostakovich's bite). |
| **Meta-Rhythm Drills** | Isolate rhythm patterns and train them independently from pitch complexity. |
| **Offline Progress Vault** | Your entire training history is stored locally in a lightweight SQLite ledger. |
| **Multilingual UI** | Interface available in English, Mandarin, German, Japanese, and Spanish, with community translations ongoing. |
| **Responsive Web Shell** | Practice on a 13-inch laptop or a 40-inch studio display; the notation engine recalibrates visual density automatically. |
| **24/7 AI Practice Partner** | An embedded AI critic listens (via microphone input) and offers gentle corrections after every 8-bar phrase. |
| **Dynamic Difficulty Spline** | Difficulty curves are not linear. They jump, plateau, and swoop—just like real musical challenges. |

---

## 🚀 Installation & Setup

Sight-Reading Orchestrator runs as a self-contained web application with no server-side dependencies. You can launch it in three ways:

1. **Direct Browser Launch** — Download the latest bundled `sro.html` from the release folder and open it in any modern browser (Chrome 90+, Firefox 88+, Safari 15+).
2. **Local Static Hosting** — Place the repository files into any web-root directory (e.g., a Raspberry Pi's `www` folder) and navigate to the index file.
3. **Docker One-Liner** — For those who prefer containerized practice, a `Dockerfile` is provided. Build the image, mount your `practice_sessions` volume, and access the UI on `localhost:8080`.

No package managers, no exotic runtimes, no build pipelines. The core engine is written in vanilla JavaScript with an optional WebAssembly module for advanced polyphonic analysis.

---

## 🎯 How the Training Loop Works

### The 4-Phase Cycle

1. **Warm-Up Glance** (60 seconds) — A 4-bar melody appears with 70% of notes pre-solved. You simply read and press "space" when you feel the phrase 'mentally locked'.
2. **The Flow Stretch** (5 minutes) — The notation starts scrolling at 45% of your last recorded max speed. The system accelerates by 2% every 4 bars if you maintain 90% accuracy.
3. **Pattern Decomposition** (2 minutes) — The engine isolates the most difficult rhythmic motive from your last session and drills it in isolation, with multiple improvisation prompts.
4. **Echo Review** (1 minute) — You sing or hum the phrase back (or play it on your instrument). The AI scoring engine compares your pitch contour and rhythm to the reference.

### The "One Breath" Criterion

The ultimate metric of success is the **One Breath Criterion** — can you sight-read a 16-bar phrase entirely within one exhalation? This forces your eye-to-hand lag to compress below 300 milliseconds, which is the threshold measured in top orchestral sight-readers.

---

## 🗂️ Repository Structure

```
sight-reading-orchestrator/
├── core_engine/
│   ├── notation_parser.js        # Converts MusicXML/MIDI to internal streaming format
│   ├── velocity_controller.js    # Manages scroll speed & adaptive pacing
│   ├── polyphony_analyzer.wasm   # WebAssembly module for 4-voice real-time analysis
│   └── rhythm_quantizer.js       # Converts micro-timings into visual heatmaps
├── ui_shell/
│   ├── responsive_layout.css     # Adaptive typography for all screen sizes
│   ├── gesture_interface.js      # Hand-sign recognition (using webcam) for page turns
│   └── light_dark_theme_switch.js
├── data_ledger/
│   ├── session_vault.sqlite      # Local privacy-first storage
│   └── export_to_musicxml.js     # Export your favorite exercises for studio use
├── practice_library/
│   ├── baroque_engine.json       # 120 algorithmic studies in Baroque counterpoint
│   ├── romantic_gesture_packs/   # Chopin-like rhythmic arpeggios & Lisztian leaps
│   └── contemporary_metrics/     # Odd time signatures (7/8, 11/16, 15/16)
├── a11y/
│   └── high_contrast_notation.css # For visually impaired musicians
├── locale/
│   ├── en_US.json
│   ├── zh_CN.json
│   ├── de_DE.json
│   ├── ja_JP.json
│   └── es_ES.json
├── LICENSE
├── CONTRIBUTING.md
└── README.md (you are here)
```

---

## 🧘 Daily Practice Rituals (Recommended for 2026)

As we enter 2026, the expectation for musical fluency is shifting. Audiences no longer want to hear perfection; they want to see **the moment of discovery** on a performer's face. Therefore, the practice rituals in this repository are designed to cultivate **joyful spontaneity** alongside technical speed.

- **Morning Reading Sprint (10 min):** Use the "Metronome = 100 WPM" preset in the dashboard. The goal is not accuracy but **gestalt comprehension** — you should be able to clap the overall contour without playing a single note.
- **Afternoon Micro-Sessions (3 × 3 min):** Use the *Flash Cadence* mode, where random 2-bar excerpts flash on screen for exactly 4 seconds, followed by a 3-second rest. Your brain fills the gaps; the ledger tracks how many "phantom notes" your mind predicted correctly.
- **Evening Reflection (5 min):** Review your heatmap. Look at the longest-duration gaze fixation. That is your new technical exercise for tomorrow.

---

## 📈 Skill Progression & Level Tiers

| Tier | Name | Benchmarks |
|------|------|------------|
| 0 | The Hummingbird | Can read 1 line in 60 seconds with 70% pitch accuracy |
| 1 | The Sight-Reader | 200 WPM equivalent, can handle 3/4 time signature fluently |
| 2 | The Page-Turner | 320 WPM, can read 5-voice polyphony without losing pulse |
| 3 | The Rachmaninoff Duelist | 420 WPM, performs modulation cadences instantly from sight |
| 4 | The Oracle | Reads 2 pages simultaneously (split-brain training mode) |

Your current tier is displayed on the home dashboard with a gentle motivational whisper (not a loud notification).

---

## 🔒 Privacy & Your Musical Data — Absolute Containment

We believe your practice habits are a sacred diary of your artistic struggle. Therefore:

- **Zero Telemetry** — The application never phones home. No analytics, no crash reports, no user fingerprinting.
- **Local-First Ledger** — All session data is stored in a SQLite vault that lives exclusively on your device.
- **No Account Required** — There is no concept of a "user profile." Your practice history is tied to an anonymous local token.
- **Export Your Soul** — At any time, you can export your complete practice history as a JSON file to share with a teacher or to archive for your future self.

---

## 🤝 Contributing to the Orchestra

We welcome contributions from musicians, UX designers, and audio engineers. Please read `CONTRIBUTING.md` thoroughly before submitting a pull request.

### Priority areas for contributions in 2026:

1. **New Style Engines** — Add a Georgian folk-melisma engine or a Brazilian choro rhythmic engine.
2. **Translation Quality** — The Japanese and Mandarin locales need more idiomatic nuance.
3. **Accessibility Extensions** — Help us design a notation system that vibrates for deaf musicians (using tactile feedback harnesses).
4. **Performance Benchmarks** — Help us profile the WebAssembly polyphony analyzer on older hardware.

---

## 🧪 Experimental Features (The "Ongoing Research" Lab)

These features are in alpha and are hidden behind a `?experimental=true` URL flag.

- **Inhalation Pacing** — Connects to a breath sensor (via Web Bluetooth) to sync phrase length with your breathing cycle.
- **Time-Frozen Sight-Reading** — The notation stops scrolling, but a 3-second audio snippet plays. You must write down what you hear, then compare against the visual notation.
- **Spectral Color-Keying** — Each harmonic interval is assigned a color, so your eye subconsciously recognizes dominant seventh chords as "warm amber" and diminished chords as "cold blue."

Use these at your own risk; they may cause paradigm shifts.

---

## ⚠️ Disclaimer & Honest Expectations

This software is a practice assistant, not a magic oracle. It cannot make you read music instantly. It can only **reveal your attention bottlenecks** so you can train with intention.

- The AI Practice Partner is a heuristic model, not a certified music pedagogue. Its suggestions should be filtered through your own musical intuition and, ideally, a human teacher's guidance.
- The 200 WPM metric is a **neuroscientific approximation** for visual-text velocity, not a direct musical tempo. An actual Rachmaninoff scherzo at 200 BPM involves far more complexity than any algorithm can currently model.
- We do not claim that using this software for 10,000 hours will guarantee a Carnegie Hall debut. It is a gym, not a genetic alteration.

---

## 🛠️ Licensing & Legal Framework

Sight-Reading Orchestrator is released under the **MIT License**, which permits commercial use, distribution, and modification, provided the original copyright notice and disclaimer are preserved. You can read the full text in the `LICENSE` file at the root of this repository.

In plain language: use it, remix it, build a business around it — just don't blame us if your piano somehow catches fire during an intense sight-reading session.

---

## 👏 Acknowledgements & Sounding Board

This project would be impossible without the open-source contributions of the `abcjs` notation engine, the `JZZ` MIDI library, and the countless classical musicians who published public-domain practice scores on IMSLP. Their generosity continues to fuel the musical community.

---

## 📮 Contact & Community Collab

We do not have an official public forum, but we maintain a **Discord server for "The Reading Circle"** where weekly community challenges are posted. Look for the link stub in the `team_assets` folder. Alternatively, report issues directly in the GitHub issue tracker; maintainers typically respond within 48 hours.

---

*Begin your first session now. Your metronome awaits — and it is both patient and ruthless.* 🎹