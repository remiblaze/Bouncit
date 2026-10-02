# Bouncit: Stereo Delay / Echo

![Bouncit free stereo delay & echo plugin UI](https://raw.githubusercontent.com/RemiBlaze/Bouncit/main/bouncit-ui-screenshot.png)

**A BPM-synced stereo delay for grooves that bounce.**

Bouncit is a tempo-synced stereo delay with independent left/right timing, a filtered and saturated feedback path, tape-style modulation, ducking, swing, freeze, and stereo-width control.

**macOS** (Apple Silicon and Intel): AU, VST3, CLAP, AAX, Standalone. Signed and notarized by Apple.

**Windows** 10 and 11, 64-bit: VST3, CLAP, Standalone. Authenticode signed.

AAX ships on macOS only.

---

## 🚀 Download & Install

Go to the [latest release](https://github.com/RemiBlaze/Bouncit/releases/latest) and pick your platform.

**macOS**
1. Download **`Bouncit_Installer.pkg`**.
2. Double-click it and follow the installer. It is signed and notarized by Apple, so it installs cleanly with no security warnings.
3. Restart your DAW and rescan plug-ins. Bouncit appears under **Remi Blaze**.

**Windows 10 and 11, 64-bit**
1. Download **`Bouncit_Installer.exe`**.
2. Run it and follow the installer. It is Authenticode signed.
3. Restart your DAW and rescan plug-ins. Bouncit appears under **Remi Blaze**.

No dongle and no extra account on either platform.

Full guide: **[remiblaze.com/support](https://remiblaze.com/support/)**.

---

## 🎛️ Features
- **Tempo-synced delay**: Sync to host BPM across 6 note values (1/32, 1/16, 1/8, 1/4, 1/2, 1/1), or switch off Sync for free time (1–2000 ms).
- **Independent L/R timing**: Link both channels together, or set each side separately for ping-pong effects.
- **Feedback**: 0–95%, with an internal Freeze mode that loops the delay buffer infinitely.
- **LP Filter**: Low-pass tone shaping in the feedback path (200 Hz – 20 kHz).
- **HP Filter**: High-pass in the feedback path (20 Hz – 2 kHz) to keep repeats out of the low end.
- **FB Saturation**: Tanh saturation in the feedback loop (0–100%) for repeats that grow warmer as they decay.
- **Ducking**: Delay repeats duck out of the way when the input signal is present (0–100%).
- **Mod Rate / Mod Depth**: LFO modulation of the delay time (0.01–5 Hz rate, 0–100% depth) for tape-style pitch wobble.
- **Stereo Width**: Mid/side width control on the wet signal, from mono (0%) to extra-wide (200%).
- **Swing**: Offsets the right-channel delay for a shuffled, grooving feel (0–100%).
- **Mix**: Dry/wet blend (0–100%) for series or parallel use.
- **Output**: Output level trim (−24 to +6 dB).
- **Freeze & Bypass**: One-click infinite-hold and true bypass with a click-free crossfade.
- **Preset menu**: 14 factory presets, selectable from the UI.
- **A/B compare**: Snapshot two settings and flip between them instantly.
- **Randomize**: Generate a fresh starting point with one click.
- **User presets**: Save and load your own `.preset` files.

---

## 🔬 Under the Hood
- **TPT feedback filters**: Low-pass and high-pass filters run inside the feedback loop using a topology-preserving state-variable design for stable, allocation-free per-sample cutoff changes.
- **Anti-aliased saturation**: Both the feedback saturator and the output soft-clipper use first-order antiderivative anti-aliasing (ADAA) to keep the drive clean.
- **DC blocker**: A one-pole ~10 Hz high-pass in the feedback loop prevents DC build-up in long-decay repeats.
- **Fractional delay**: Linearly interpolated delay reads with smoothed delay times for click-free timing and subdivision changes.
- **Output safety**: A soft-clip stage plus a hard ceiling and NaN/Inf guards protect the output at all times.
- **Universal binary**: Native on Apple Silicon and Intel.

---

## 💻 System Requirements

**macOS**
- macOS 15.0 or later
- Apple Silicon or Intel Mac (Universal Binary)
- An AU, VST3, CLAP or AAX host

**Windows**
- Windows 10 or Windows 11, 64-bit
- A VST3 or CLAP host

---

## 🎚️ Factory Presets (14)

| Preset | Best For |
|--------|----------|
| Init | Clean starting point |
| Subtle Slap | Short slapback |
| Ping Pong | Bouncing L/R echoes |
| Dub Echo | Filtered dub repeats |
| Vocal Throw | Vocal delay throws |
| Dotted Eighth | Rhythmic free-time delay |
| Dark Repeats | Low-pass filtered tails |
| Filtered Tape | Warm tape-style echo |
| Rhythmic Bounce | Grooving ping-pong with swing |
| Long Wash | Long ambient tails |
| Remi Blaze Echo | Signature dub throw |
| The Rolling Dub | Long feedback dub |
| Satin Shimmer | Bright wide shimmer |
| Warehouse Build | Big filtered build |

---

## 🐛 Bugs & Issues
Open an issue on the **[Issues](https://github.com/RemiBlaze/Bouncit/issues)** tab with your macOS or Windows version, DAW + version, and steps to reproduce.

---

## 📄 License & Credits
- **Plugin page:** [remiblaze.com/plugins/bouncit/](https://remiblaze.com/plugins/bouncit/).
- **Developer:** [Remi Blaze](https://remiblaze.com).
- **Framework:** [JUCE](https://juce.com).
- **License:** free under a proprietary [Freeware License](LICENSE) (see also our [terms](https://remiblaze.com/terms/)). Reverse-engineering, repackaging, binary redistribution, or reselling the compiled installer is strictly prohibited.

---

## Trademarks

All product names, company names, and logos mentioned herein are trademarks or registered trademarks of their respective owners. Any such references are used for descriptive or compatibility purposes only and do not imply affiliation with, endorsement by, or sponsorship from their owners.

VST is a trademark of Steinberg Media Technologies GmbH, registered in Europe and other countries.

Apple, macOS, Audio Units (AU), and Apple Silicon are trademarks of Apple Inc., registered in the U.S. and other countries.

AAX, Avid, and Pro Tools are trademarks or registered trademarks of Avid Technology, Inc. in the U.S. and other countries.

Microsoft and Windows are trademarks of the Microsoft group of companies.
