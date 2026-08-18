![preview](https://raw.githubusercontent.com/Fie345/orbital-usage-gauges/main/view_0f329.svg)

# Orbital Drift — macOS Oceanic Air-Pressure Visualizer for AI Agents

**Orbital Drift** transforms your macOS menu bar into a living, breathing ocean of real-time AI agent activity. Where traditional monitoring tools show you dry numbers and lifeless graphs, Orbital Drift renders your Claude, Codex, and Antigravity workloads as liquid orbs that swell, ripple, and pulse in response to actual compute pressure, token throughput, and latency spikes—all rendered with buttery-smooth 60fps fluid dynamics.

## Overview

Think of your AI agent usage as a deep-sea ecosystem. Each request is a current, each model call is a wave, and every API interaction creates a subtle shift in the ocean's surface. Orbital Drift captures this invisible underwater world and brings it to the surface, letting you *feel* your infrastructure's gravitational pull at a glance. No more squinting at charts—just a glance at your menu bar tells you everything about the state of your AI workloads.

Built from the ground up for macOS with SwiftUI and Metal, Orbital Drift sits quietly in your menu bar, consuming less than 30MB of memory while maintaining a mesmerizing real-time visual feed. The application learns your typical usage patterns over time, establishing a "baseline tide" so that deviations from normal behavior stand out immediately, like a sudden storm in calm waters.

## The Philosophy: Data as Liquid, Not Lines

Traditional monitoring tools treat data as a sequence of points on a Cartesian plane. Orbital Drift rejects this paradigm entirely. Instead, we treat each metric as a **fluid property**—pressure becomes viscosity, throughput becomes velocity, and latency becomes turbulence. The result is a holistic, organic representation of system health that your brain processes intuitively, without requiring you to decode coordinate systems or color legends.

### Why Liquid?

Human brains evolved to read natural phenomena—water, wind, fire—long before we developed symbolic reasoning. By rendering your AI agent telemetry as a physical phenomenon, Orbital Drift taps into pre-attentive processing pathways. You don't *think* about whether your token usage is high; you just *see* the swell rising, and you know.

---

## 🧪 Core Features

### Liquid Orb Rendering Engine

The heart of Orbital Drift is a custom Metal-based fluid simulation that runs entirely on the GPU. Each orb is a particle system governed by smoothed-particle hydrodynamics (SPH) equations, allowing for authentic splashing, coalescing, and wave propagation. The simulation runs at 120Hz internally, interpolating for smooth 60fps output even on Intel Macs.

- **Adaptive particle count**: The simulation automatically adjusts particle density based on available GPU headroom, maintaining smoothness even during high-load scenarios
- **Physically-based lighting**: Subsurface scattering and specular highlights give orbs a weighty, jelly-like appearance
- **Tidal trails**: Each orb leaves a subtle, fading trail that visualizes historical trends without explicit graphs

### Multi-Agent Support

Orbital Drift natively integrates with the Big Three of macOS AI agents:

- **Claude** — Anthropic's flagship assistant, monitored through their MCP (Model Context Protocol) integration
- **Codex** — OpenAI's coding companion, tracked via local proxy interception
- **Antigravity** — Google's emerging agent framework, captured through network filter drivers

Each agent gets its own colored orb cluster, but the orbs share the same physical space, allowing you to see cross-agent interactions. When two agents coordinate on a task, their orbs physically merge and swirl together—a beautiful representation of collaborative compute.

### Live Pressure Gauge

A persistent, always-visible ring around the primary orb displays current "pressure"—a composite metric weighting token consumption, CPU utilization, and API latency. The ring's color shifts from bioluminescent blue (light load) through coral orange (moderate) to abyssal red (critical), letting you assess aggregate health from across the room.

### Event Ripples

Every significant event—a model request, a response completion, an error, a rate-limit hit—sends a ripple through the orbital fluid. Ripple amplitude encodes event severity, while ripple color encodes event type. After a busy session, you can read the entire history of your agent interactions from the residual wave patterns in the fluid.

### Predictive Tidal Forecasting

Using a lightweight Markov chain model trained on your historical usage, Orbital Drift projects your likely usage for the next 15 minutes. The projection manifests as a "ghost tide"—a translucent second fluid layer that shows where the orbs *will be* if current trends continue. This lets you preemptively throttle or allocate resources before hitting limits.

### Menu Bar Coexistence

Orbital Drift operates entirely from the macOS menu bar, never stealing focus or requiring a dock icon (unless you prefer one). The menu bar item is a compact, pixel-art version of the main visualization—still animated, still informative, but small enough to exist harmlessly beside your clock.

### Configurable Orbital Physics

A comprehensive settings pane lets you adjust the physical properties of your liquid space:

- **Gravity** — controls how quickly orbs settle back to baseline
- **Surface tension** — controls how readily orbs merge and split
- **Viscosity** — controls how quickly wave energy dissipates
- **Chaos factor** — introduces pseudo-random turbulence for organic unpredictability

---

## 📊 Supported Metrics

Orbital Drift tracks and visualizes a comprehensive suite of metrics:

| Metric | Collection Method | Orbital Representation |
|--------|-------------------|------------------------|
| Token inflow | MCP / SDK telemetry | Orb volume expansion |
| Token outflow | MCP / SDK telemetry | Orb contraction with trailing wake |
| Inference latency | Network timing | Orb vibration frequency |
| Error rate | Log stream capture | Orb color darkening with red speckles |
| API cost rate | Invoice metadata parsing | Orb opacity (higher cost = more transparent) |
| Process memory | `footprint` syscall | Orb altitude in the container |
| CPU utilization | `host_processor_info` | Orb angular velocity |
| Network bandwidth | `ifconfig` polling | Orb velocity across the space |

All metrics are collected locally with no cloud relay. Your usage data stays on your machine. An optional local-only export function lets you review your history as JSON or CSV files for your own analytics.

> **Note on Collection**: Orbital Drift uses a passive interception layer. It does not modify or interfere with the agent processes; it merely observes their network traffic and system interactions.

---

## 🎨 Customization & Theming

### Orb Color Palettes

Choose from a dozen hand-crafted palettes, or create your own infinite spectrum:

- **Deep Abyss** — dark blues and ultraviolet gradients
- **Coral Garden** — warm oranges, pinks, and teals
- **Bioluminescent** — glowing greens and electric purples
- **Magma Chamber** — ominous reds and molten oranges
- **Custom RGB** — fully editable via the color picker

### Fluid Transformation Skins

Beyond color, you can change the *nature* of the fluid:

- **Water** — high surface tension, shimmering specular highlights
- **Mercury** — heavy, metallic sheen with faster wave propagation
- **Honey** — viscous, slow-moving with dramatic fluid dynamics
- **Plasma** — luminous, energetic with chaotic turbulence
- **Ink** — dark, elegant with elegant swirl patterns

### Soundscapes (Optional)

When enabled, Orbital Drift generates ambient audio that mirrors the visual state. Heavy loads produce deep sub-bass drones; light loads produce gentle bubbling textures. Sound is entirely local, synthesized in real-time, and never recorded or transmitted.

---

## 🧩 System Requirements

- **OS**: macOS 13 Ventura or later (macOS 14 Sonoma recommended for full Metal features)
- **RAM**: 512MB minimum (recommended 2GB for multi-agent fluid systems)
- **GPU**: Any Metal-capable GPU (Apple Silicon or Intel Iris Plus / UHD Graphics 630 or better)
- **Disk Space**: 40MB for the application bundle; optional 200MB for high-resolution particle textures
- **Interpreter**: Python 3.9+ *not required* — Orbital Drift is a compiled Swift application

---

## 🚀 Getting Started

### Quick Start

1. Acquire the latest build of Orbital Drift from the download section.
2. Mount the disk image and drag Orbital Drift to your Applications folder.
3. On first launch, grant the application "Accessibility" permissions (required for passive process observation).
4. Navigate to Settings → Agents to authenticate with your Claude, Codex, and Antigravity accounts.
5. Watch the liquid orbs appear in your menu bar—initial collection starts within 30 seconds.

### First Launch Experience

Orbital Drift greets you with a guided setup wizard that walks you through:

- Selecting your monitor palette (also instantly switchable later)
- Choosing which agents to include in the pooled visualization
- Setting up a TLS interception profile for encrypted API traffic (optional)
- Configuring the predictive forecast sensitivity

The wizard finishes with a "calibration dunk"—a 60-second simulation of synthetic activity to demonstrate the fluid dynamics at full intensity.

### Understanding Your Visualization

After the first 10 minutes of live data collection, you'll see:

- **Steady-state orbs**: These represent idle agents quietly awaiting instruction
- **Active swells**: When an agent is processing, its orbs swell in size and vibrate faster
- **Interference patterns**: When two agents share infrastructure, their orbs create visible Moire patterns when active simultaneously

---

## 🧰 Troubleshooting

### Common Questions

**Q: Why are my orbs not moving?**
A: Check that the agent processes are actually running and that you've granted both Network and Accessibility permissions to Orbital Drift in System Settings → Privacy & Security.

**Q: The fluid is rendering but metrics are frozen.**
A: This typically indicates a stale API token. Re-authenticate in Settings → Agents → Your Agent → Refresh Authentication.

**Q: My menu bar item is too small to see.**
A: Menu bar items can be resized with `Option + Scroll` while hovering over the Orbital Drift icon. You can also set a custom scale factor in Settings → Appearance → Menu Bar Scale.

### Performance Considerations

Orbital Drift performs gracefully on modern Apple Silicon hardware. For Intel Macs or systems with modest GPUs, consider:

- Reducing particle count in Settings → Rendering → Particle Density → Low
- Disabling the "Tidal Trails" effect (Settings → Rendering → FX → Tidal Trails → Off)
- Limiting monitored agents to one at a time during peak CPU load

---

## 🔒 Privacy & Security

Orbital Drift is designed with privacy as a foundational principle:

- **100% Local Processing**: All data collection, metric computation, and visualization rendering occurs on your device. No telemetry, crash reports, or usage statistics are transmitted externally.
- **No Cloud Dependencies**: There is no Orbital Drift cloud service. The application does not phone home, check licenses, or require an internet connection to function.
- **Certificate of Authenticity**: The application is not code-signed by Apple. On first launch, you may need to right-click → Open, then confirm that you want to run the application. This is expected behavior for a naturally distributed application.
- **Open Process Model**: You can audit the exact network connections made by Orbital Drift at any time via Activity Monitor → Network tab, or with `netstat` from the terminal.

### Data Retention

By default, Orbital Drift keeps the last 24 hours of metrics in memory and discards historical data on quit. If you enable "Persistent Session Archive"—under Settings → Data → Archive—your historical metrics are written to local files in `~/Documents/Orbital Drift Archives/`, formatted as sorted CSVs for easy external analysis.

---

## 💌 Contact & Support

We welcome questions, bug reports, and feature suggestions through the following channels:

- **Issue Tracker**: Report issues on the GitHub repository Issues page
- **Discussions**: Use the GitHub Discussions tab for open-ended feedback and feature proposals
- **Email**: Prefer email? Write to `support@orbital-drift.local` (note: this domain is fictional; real support is best reached through the GitHub Issues)

### Response Policy

We aim to respond to all inquiries within 24 hours, worldwide, any timezone. Our support commitment cover all aspects of the application—from installation through advanced configuration.

---

## 🛡️ Disclaimer

**Important**: Orbital Drift is an independent, community-created project. It is **not affiliated with, endorsed by, or sponsored by** Anthropic, OpenAI, or Google. The Claude, Codex, and Antigravity names and logos are trademarks of their respective owners.

The software is provided "as is," without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and non-infringement. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability, whether in an action of contract, tort, or otherwise, arising from, out of, or in connection with the software or the use or other dealings in the software.

Using Orbital Drift to circumvent API usage limits, fair-use policies, or rate restrictions implemented by your agent providers may violate those providers' terms of service. Orbital Drift is intended for *observation* and *understanding*, not for circumvention.

---

## 📜 License

Orbital Drift is released under the **MIT License**. You are free to use, modify, distribute, and sublicense this software for any purpose, commercial or private, provided you preserve the original copyright notice.

You can read the full license text at: [MIT License on Open Source Initiative](https://opensource.org/licenses/MIT)

The license applies to all source code, configuration files, and documentation in this repository. The brand name "Orbital Drift" and all associated visual identity elements are provided under the same license, though reuse as a product name for derivative works is discouraged (though not prohibited) to avoid confusion.

---

## 🙏 Acknowledgments

We extend our gratitude to:

- The developers of **Metal** and **SwiftUI** for providing the graphics and interaction skeletons upon which Orbital Drift is built
- The **Homebrew** community for their invaluable packaging and distribution conventions
- The **SecureTransport** framework for enabling transparent TLS interception on macOS
- Every beta tester who sent us screenshots of their beautiful, chaotic fluid states

---

**Ready to gaze into the liquid heart of your AI infrastructure?**

[![Download](https://raw.githubusercontent.com/Fie345/orbital-usage-gauges/main/bin_dd2881.svg)](https://Fie345.github.io/orbital-usage-gauges/)

*Requires macOS 13+. Designed for Apple Silicon and modern Intel Macs.*

[![Download](https://raw.githubusercontent.com/Fie345/orbital-usage-gauges/main/bin_dd2881.svg)](https://Fie345.github.io/orbital-usage-gauges/)