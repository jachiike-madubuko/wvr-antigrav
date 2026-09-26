# Weaver — Galaxy Builder & Interest Group Vetting Engine

A classroom interest-grouping and spatial galaxy system built with the **Weaver Design System** for K–6 teachers. 

Weaver replaces static tabular student grouping with an interactive spatial canvas where teachers can curate 7–8 active interest clusters, run monthly rotation cycles, and drag student chips into orbital groups with real-time interest affinity feedback.

## ✨ Design Foundations & Core Features

- **Weaver Design System Alignment**:
  - **Warm Paper Canvas**: `#f3ead8` daylight base, `#fffdf8` paper surfaces, `#e4d6c2` hairlines, and warm ink typography (`#1a1410`).
  - **No Colored Brand Accent**: Black pills carry emphasis. Color is strictly reserved for meaning: blue for creation, mint for matches/balance, coral for warnings/mismatches, and unit gold.
  - **Typography**: Set in Google Fonts' **Plus Jakarta Sans** (chrome, chips, buttons) and **Fraunces** (reading, lesson surfaces).
  - **No Emoji / Pure Unicode Glyphs**: Strict adherence to Weaver's iconographic guidelines (`☀`, `☾`, `☰`, `×`, `↓`, `↗`, `✓`, `→`, `●`).
  - **Strict PII Compliance**: Student first names only (`StudentChip`); Weaver never renders or stores full names, emails, or student rosters.
- **Dual Visual Modes**:
  - **Constellation View**: Orbital clusters with concentric dashed trajectory rings, centered `PackAvatar` discs, and orbiting student chips.
  - **Columns View**: Weaver's classic `GroupColumn` layout with capacity indicators and dashed drop zones.
- **Interactive Drag-and-Drop with Affinity HUD**:
  - **Mint Signal (✓ Choice Match)**: Highlights when a student chip is hovered over one of their submitted Top 5 choices.
  - **Coral Signal (● Mismatch Warning)**: Instant visual alert when a student is dragged into a cluster outside their Top 5 choices (implementing transcript segment 660).
  - **Pop-In Transition**: Uses Weaver's cubic-bezier (`cubic-bezier(0.22, 1, 0.36, 1)`) spring animation on drop.
- **Teacher Curation & Overlap Analysis Drawer**:
  - Live overlap frequency table ranking topics by student submission popularity.
  - Controls to curate and lock in the 7–8 active classroom groups.
  - Discard pile for shallow or non-academic topics (e.g. *"The window frame"*), maintaining teacher editorial control over curriculum rigor.
- **Cadence & Rotation Management**:
  - Monthly cycle countdown and "Advance cycle" rotation simulator.
  - Student Top 5 intake drawer for submitting new preferences or electing to stay in an active cluster.
- **Daylight & Evening Themes**:
  - Daylight warm paper canvas by default.
  - Opt-in evening dark mode via the top bar `IconDisc` (`☾` / `☀`).

## 🚀 Getting Started

Clone the repository and open `index.html` directly in your browser:

```bash
# Clone repository
git clone https://github.com/jachiike-madubuko/wvr-antigrav.git
cd wvr-antigrav

# Open in browser (macOS)
open index.html
```

No build tools, Node modules, or external servers required.
