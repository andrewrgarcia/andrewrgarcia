<!-- ============================= -->
<!--             HERO              -->
<!-- ============================= -->

<p align="center">
  <a href="https://andrewcomputing.com">
    <img
      src="https://github.com/user-attachments/assets/c0c3e7e8-30b9-4fe7-95f8-867ea6746aba"
      width="150"
      alt="Blorbo mascot"
    />
  </a>
</p>

<h1 align="center">Andrew Garcia, Ph.D.</h1>

<p align="center">
  <strong>Building programming systems for humans and AI.</strong>
</p>

<p align="center">
  Rust · Python · AI Infrastructure · Programming Languages · Scientific Computing
</p>

<p align="center">
  <a href="https://andrewcomputing.com"><strong>Website</strong></a>
  ·
  <a href="https://github.com/andrewrgarcia?tab=repositories"><strong>Repositories</strong></a>
</p>

<p align="center">
  <img
    src="https://img.shields.io/badge/Ph.D.-Chemical%20Engineering-6f42c1"
    alt="Ph.D. in Chemical Engineering"
  />
  <img
    src="https://img.shields.io/badge/Focus-AI%20Infrastructure-blue"
    alt="Focus: AI Infrastructure"
  />
  <img
    src="https://img.shields.io/badge/Languages-Rust%20%7C%20Python%20%7C%20C%2B%2B-orange"
    alt="Languages: Rust, Python, and C++"
  />
  <img
    src="https://img.shields.io/badge/Open%20Source-150%2B-success"
    alt="More than 150 open-source projects"
  />
  <img
    src="https://img.shields.io/badge/Built%20for-Real%20Work-black"
    alt="Built for real work"
  />
</p>

---

## About

I build software around one problem:

> **Making complex systems understandable to both humans and AI.**

That has led me to build programming languages, coding-agent infrastructure, long-context knowledge systems, conversational tooling, scientific software, and developer platforms.

Before focusing on AI systems, I worked on economic forecasting for Peru's Central Reserve Bank and taught computer science at the university level.

Nearly everything here began because an existing tool failed under real use.

---

## Systems

<p align="center">
  <a href="https://github.com/andrewrgarcia/viceroy">
    <img
      height="82"
      alt="Viceroy"
      src="https://github.com/user-attachments/assets/b7d0e7e0-664a-4a39-81b1-9a674e3a3537"
    />
  </a>
  &nbsp;&nbsp;&nbsp;

  <a href="https://crates.io/crates/fur-cli">
    <img
      height="82"
      alt="FUR"
      src="https://github.com/user-attachments/assets/6135887d-2a93-4170-ac9a-c68687f15a2f"
    />
  </a>
  &nbsp;&nbsp;&nbsp;

  <a href="https://crates.io/crates/yggdrasil-cli">
    <img
      height="82"
      alt="Yggdrasil"
      src="https://github.com/user-attachments/assets/d822648c-2d2b-41ad-a3ad-381bed63469a"
    />
  </a>
  &nbsp;&nbsp;&nbsp;

  <a href="https://moxi-next.vercel.app/">
    <img
      height="82"
      alt="Moxi"
      src="https://github.com/user-attachments/assets/39b842ac-8844-46ba-8f01-3f5213cabf6d"
    />
  </a>
  &nbsp;&nbsp;&nbsp;

  <a href="https://deckmaster-editor.vercel.app">
    <img
      height="82"
      alt="Deckmaster"
      src="https://github.com/user-attachments/assets/f2dc9f99-22e0-4c74-99aa-8746d8789482"
    />
  </a>
</p>

<p align="center">
  <strong>Viceroy</strong>
  ·
  <strong>FUR</strong>
  ·
  <strong>Yggdrasil</strong>
  ·
  <strong>Moxi</strong>
  ·
  <strong>Deckmaster</strong>
</p>

<p align="center">
  Coding agents · Conversation control · Codebase context · 3D worlds · Presentations
</p>

---

## Featured Systems

<details>
<summary><strong>⚖️ Viceroy — deterministic edits for coding agents</strong></summary>

<br>

Most coding agents generate suggestions.

**Viceroy generates directly applicable edits.**

It gives agents a deterministic editing interface for producing whole-file replacements or exact verbatim swaps—never vague instructions such as “insert this somewhere nearby and hope the indentation spirits are cooperative.”

Edits can be:

- applied automatically
- verified locally
- benchmarked objectively
- reproduced without an LLM judge
- checked for unintended collateral changes

Viceroy is built for coding agents that need to modify real repositories reliably, not merely describe what a competent engineer might do.

**Project:** [github.com/andrewrgarcia/viceroy](https://github.com/andrewrgarcia/viceroy)

</details>

<details>
<summary><strong>🧠 FUR — conversation control for LLM systems</strong></summary>

<br>

Chat history is not the same thing as memory.

**FUR provides structured conversation control for long-running AI workflows.**

It helps manage:

- active context
- interaction history
- message traceability
- branching conversational state
- retrieval from earlier exchanges
- persistent records outside a model's context window

Instead of treating every conversation as an increasingly swollen string, FUR treats interaction history as structured information.

Because eventually every AI chat becomes an attic, and somebody has to label the boxes.

**Project:** [crates.io/crates/fur-cli](https://crates.io/crates/fur-cli)

</details>

<details>
<summary><strong>🌲 Yggdrasil — codebases compiled into context</strong></summary>

<br>

Repositories grow larger than context windows.

**Yggdrasil turns a codebase into a single structured Markdown artifact for AI workflows.**

It collects project structure and source content into an injectable representation that language models can inspect without manually opening files one at a time.

That makes it useful for:

- repository-wide reasoning
- coding-agent context
- audits and reviews
- architectural analysis
- long-context prompting
- reproducible project snapshots

Think of it as compiling software into knowledge an AI can carry around.

**Project:** [crates.io/crates/yggdrasil-cli](https://crates.io/crates/yggdrasil-cli)

</details>

<details open>
<summary><strong>🧊 Moxi — an AI-native language for building 3D worlds</strong></summary>

<br>

**Moxi is a programming language for designing 3D worlds in syntax close to natural language.**

A Moxi program is an ordinary Markdown file describing atoms, materials, entities, geometry, and relationships.

That makes Moxi readable by humans, straightforward to version with Git, and predictable enough for language models to generate.

```moxi
# Birthday Cake
> A layered cake with frosting and three candles.

atom CAKE   { color = "#FFC0CB" }
atom CREAM  { color = purple }
atom WAX    { color = white }
atom FLAME  { color = orange }

material Cake   { voxel_atom = CAKE }
material Cream  { voxel_atom = CREAM }
material Wax    { voxel_atom = WAX }
material Flame  { voxel_atom = FLAME }

entity BirthdayCake {
    part Base         { shape = cylinder(height=4, radius=8), material = Cake }
    part Frosting     { shape = cylinder(height=1, radius=8), material = Cream }
    part TopLayer     { shape = cylinder(height=3, radius=6), material = Cake }
    part TopFrosting  { shape = cylinder(height=1, radius=6), material = Cream }

    part LeftCandle   { shape = cylinder(height=5, radius=0.5), material = Wax }
    part CenterCandle { shape = cylinder(height=5, radius=0.5), material = Wax }
    part RightCandle  { shape = cylinder(height=5, radius=0.5), material = Wax }

    part LeftFlame    { shape = sphere(radius=0.8), material = Flame }
    part CenterFlame  { shape = sphere(radius=0.8), material = Flame }
    part RightFlame   { shape = sphere(radius=0.8), material = Flame }

    relation {
        Frosting     above Base
        TopLayer     above Frosting
        TopFrosting  above TopLayer

        CenterCandle above TopFrosting
        LeftCandle   left_of CenterCandle
        RightCandle  right_of CenterCandle

        LeftFlame    above LeftCandle
        CenterFlame  above CenterCandle
        RightFlame   above RightCandle
    }

    resolve voxel_size = 1.0
}

print BirthdayCake detail=low
```

The Rust-based Moxi compiler transforms source programs into voxel scenes, meshes, and exportable 3D assets.

The browser-based **Moxi Sandbox** provides:

- source editing
- local compilation
- live 3D rendering
- multiple rendering modes
- image sharing
- GLB export
- immediate compiler feedback

Instead of asking an AI to emit thousands of vertices, you ask it to write a world.

The compiler builds the rest.

**Sandbox:** [moxi-next.vercel.app](https://moxi-next.vercel.app/)

</details>

<details>
<summary><strong>🎴 Deckmaster — presentations as code</strong></summary>

<br>

Slide editors are useful until a presentation needs version control, automation, reusable structure, or large-scale revision.

**Deckmaster treats presentations as programmable documents.**

Slides become source rather than opaque editor state, making room for:

- reproducible builds
- reusable components
- automated generation
- version-controlled changes
- structured technical content
- AI-assisted authoring
- consistent visual systems

The goal is not merely to generate slides.

It is to make presentations behave more like software.

**Editor:** [deckmaster-editor.vercel.app](https://deckmaster-editor.vercel.app)

</details>

---

<details>
<summary><strong>Engineering Philosophy</strong></summary>

<br>

Good software survives contact with reality.

That means building systems that are:

- **deterministic** instead of magical
- **observable** instead of mysterious
- **reproducible** instead of anecdotal
- **composable** instead of monolithic
- **maintainable** after the original excitement wears off
- **useful** after the demonstration ends

I prefer tools that people quietly continue using over software that briefly performs interpretive dance on social media.

</details>

<details>
<summary><strong>Technologies and Interests</strong></summary>

<br>

### Areas

AI infrastructure · Programming languages · Coding agents · Knowledge representation · Long-context systems · Scientific computing · Developer tooling · Local-first software

### Technologies

Rust · Python · TypeScript · C++ · SQLite · PostgreSQL · FastAPI · PyTorch · CUDA · WebGPU · Docker · Linux

</details>

<details>
<summary><strong>More Open Source</strong></summary>

<br>

The systems above represent the core of my current work.

Beyond them, I maintain projects spanning:

- scientific computing
- data visualization
- simulation
- encryption
- retrieval systems
- execution environments
- CLI tooling
- research infrastructure

Most began as tools I built for my own work.

Many are now used by people I have never met, which is both flattering and a mildly alarming amount of responsibility.

**Browse everything:** [github.com/andrewrgarcia?tab=repositories](https://github.com/andrewrgarcia?tab=repositories)

</details>

---

## Find Me

<p align="center">
  <strong>
    <a href="https://andrewcomputing.com">andrewcomputing.com</a>
  </strong>
</p>

<p align="center">
  AI infrastructure · Programming languages · Developer platforms · Scientific software
</p>

<p align="center">
  <sub>🐧 Blorbo believes software should survive contact with reality.</sub>
</p>
