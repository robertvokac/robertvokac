# 👋 Robert Vokáč — C++ Systems Engineer

**Modern C++ · 3D tooling · Cross-platform frameworks · Compatibility layers · Runtime systems**

---

## 🚀 Focus

C++ developer focused on **3D tooling**, **system-level engineering**, **cross-platform framework design**, and **compatibility layers**.

Looking for roles in:

* C++ systems engineering
* runtime / framework development
* cross-platform / platform abstraction work
* backend / platform architecture
* game technology / engine tooling

---

## 🧠 What I build

I design and implement **3D tools, C++ frameworks, platform abstraction layers, and compatibility systems** in modern C++, focusing on:

* explicit API design
* system behavior reproduction
* modular architecture
* cross-platform execution (Windows · Linux · WebAssembly · Android)
* long-term maintainability

Validated on real-world applications (Planet Blupi 1996, Speedy Blupi 2001/2013) — playable web builds at [speedyblupi.com](https://speedyblupi.com). Ecosystem hub: [openeggbert.com](https://openeggbert.com).

**≈282k lines of C++** across the projects below.¹

---

## 🔥 Projects

### 1. Mesh Craft — 3D scene editor

🔗 https://github.com/openeggbert/mesh-craft · 🌐 https://meshcraft3d.com · 🌐 https://meshcraft.openeggbert.com · 📏 ≈16.5k LOC

* C++23 3D scene editor for the `.mc3.xml` format — primitive shapes, hierarchical groups, CSG (union/difference/intersection via Manifold), extrude-along-path, PBR materials, keyframe animation, prefabs
* native `.mc3.xml` format: human-readable XML-based editable source compiled to glTF/GLB or binary MCB via `mc3togltf` / `mc3tomcb` CLI tools
* Dear ImGui editor (orbit camera, gizmos, timeline, undo/redo, autosave) built on CNA + sharp-runtime; exercises the full C++ engine stack as a real editor application
* Actively developed — full XML load/save roundtrip, all primitives, CSG, animation, and GLB export working

➡️ Focus: **3D tooling, file formats, geometry processing, editor UX**

---

### 2. Mesh World — procedural 3D world generator

🔗 https://github.com/openeggbert/mesh-world · 🌐 https://meshworld3d.com · 🌐 https://meshworld.openeggbert.com · 📏 ≈8.6k LOC

* generates infinite 3D city and landscape chunks from a JSON config — 20 C++ chunk generators + 17 Lua object generators
* Lua scripting sandbox (sol2 + Lua 5.4) for content modding; auto-discovered at startup
* SQLite content packs: taxonomy registry, material registry, generator bundles in portable `.sqlite` files
* real-time 3D explorer (MeshWorldApp) built on Mesh Craft + CNA (SDL3/OpenGL)
* 119 tests passing, zero warnings, CI on every push

---

### 3. CNA — C++ framework (XNA-style API)

🔗 https://github.com/openeggbert/cna · 🌐 https://libcna.com · 🌐 https://cna.openeggbert.com · 🎮 [WebAssembly demo](https://speedyblupi.com/SpeedyBlupi2013/) · 📏 ≈61.5k LOC

* XNA-style API in native C++ under `Microsoft::Xna::Framework`
* rendering, input, audio, resource lifecycle, backend abstraction
* backends: SDL3 / OpenGL (easy-gl) / bgfx
* one codebase targets Windows, Linux, WebAssembly, and Android
* used to port a real C# / XNA game (Speedy Blupi, 2013)

➡️ Focus: **cross-platform framework, runtime systems, API compatibility**

---

### 4. CNA Samples — XNA sample collection ported to C++

🔗 https://github.com/openeggbert/cna-samples · 📏 ≈32.3k LOC

* C++ ports of the official Microsoft XNA Game Studio 4.0 sample collection, running on CNA
* a continuously growing compatibility test bed proving the framework's API coverage on real code
* 🎮 web demos coming soon

---

### 5. Sharp Runtime — C#/.NET subset in native C++

🔗 https://github.com/openeggbert/sharp-runtime · 🌐 https://sharpruntime.openeggbert.com · 📏 ≈36.4k LOC

* `System::*` namespaces implemented in idiomatic modern C++
* covers exceptions, events, delegates, collections, and system-level building blocks
* foundation layer for CNA, Mesh Craft, Mesh World, and Galaxy Eggbert

---

### 6. Free Direct — DirectX 3 (2D) compatibility layer

🔗 https://github.com/openeggbert/free-direct · 🌐 https://freedirect.openeggbert.com · 🎮 [Speedy Eggbert 2 demo](https://speedyblupi.com/SpeedyEggbert2/) · 🎮 [Planet Blupi demo](https://speedyblupi.com/PlanetBlupi/) · 📏 ≈3.2k LOC

* reimplementation of DirectDraw / DirectSound subset over SDL3
* CPU surface model, blitting, palettes, color keys, locking, presentation
* designed to replace original DirectX 3 SDK dependencies in legacy applications

➡️ Focus: **low-level graphics systems, legacy API compatibility**

---

### 7. Free API — WinAPI compatibility layer

🔗 https://github.com/openeggbert/free-api · 🌐 https://freeapi.openeggbert.com · 📏 ≈4.1k LOC

* WinAPI-style windowing, message loop, input, timers, multimedia APIs
* SDL3-based implementation (Linux / cross-platform)
* works together with Free Direct as the system/platform side of legacy application compatibility

➡️ Focus: **system APIs, OS abstraction, runtime behavior**

---

### 8. Free Eggbert — Speedy Eggbert 2 reconstruction

🔗 https://github.com/openeggbert/free-eggbert · 🌐 https://freeeggbert.openeggbert.com · 🎮 [WebAssembly demo (partial)](https://speedyblupi.com/SpeedyEggbert2/) · 📏 ≈28.1k LOC

* buildable reconstruction of the 1998–2001 game Speedy Eggbert 2, reverse-engineered from original binaries (Ghidra, IDA, ILSpy)
* made portable beyond Windows/DirectX via Free API + Free Direct (SDL3)
* Emscripten web build with IndexedDB save persistence

➡️ Focus: **reverse engineering, game preservation**

---

### 9. Mobile Eggbert — C++ port of Speedy Blupi (2013)

🔗 https://github.com/openeggbert/mobile-eggbert · 🌐 https://mobileeggbert.openeggbert.com · 🎮 [Play in browser](https://speedyblupi.com/SpeedyBlupi2013/) · 📏 ≈20.5k LOC

* C++ port of the 2013 Windows Phone XNA game Speedy Blupi, running on CNA
* migration chain: C# XNA 4.0 → ILSpy decompilation → MonoGame → native C++/CNA
* playable on desktop and in the browser (IndexedDB saves); reference implementation for Galaxy Eggbert

---

### 10. Galaxy Eggbert — 3D game (CNA)

🔗 https://github.com/openeggbert/galaxy-eggbert · 🌐 https://galaxyeggbert.openeggbert.com · 📏 ≈5.4k LOC

* 3D remake of Speedy Blupi validating the full CNA engine stack
* targets Linux, Windows, WebAssembly, and Android from a single C++ codebase

---

### 11. easy-gl — OpenGL/OpenGL ES rendering wrapper

🔗 https://github.com/openeggbert/easy-gl · 🌐 https://easygl.openeggbert.com · 📏 ≈3.6k LOC

* toolkit-independent C++20 OpenGL/OpenGL ES wrapper
* host owns window and GL context; easy-gl owns all OpenGL interaction
* built on top of meta-gl; used by CNA as its OpenGL rendering backend

---

### 12. easy-3d — 3D helper library for CNA

🔗 https://github.com/openeggbert/easy-3d · 🌐 https://easy3d.openeggbert.com · 📏 ≈0.7k LOC

* small C++23 helper library beside CNA — deliberately a library, not an engine
* cameras (orbit/follow), texture atlas, billboard and cube batching, debug draw
* first consumer: Galaxy Eggbert

---

### 13. meta-gl — low-level OpenGL function loader

🔗 https://github.com/openeggbert/meta-gl · 🌐 https://metagl.openeggbert.com · 📏 ≈7.8k LOC

* type-safe C++23 OpenGL ES 2.0+ function loader
* runtime loading via host-supplied `GetProcAddress` — no windowing, no context creation
* `enum class` wrappers for all OpenGL constants; foundation layer for easy-gl

---

### 14. Mobile Eggbert Legacy — C#/MonoGame preservation archive

🔗 https://github.com/openeggbert/mobile-eggbert-legacy

* preserved C#/MonoGame stage of the Mobile Eggbert migration
* ILSpy-decompiled Windows Phone XNA 4.0 sources; related repositories merged via git subtree

---

### 15. Mobile Eggbert LibGDX — Java port

🔗 https://github.com/openeggbert/mobile-eggbert-libgdx

* Java/LibGDX port of Speedy Blupi (Mobile Eggbert) with a small XNA/.NET compatibility bridge
* desktop (LWJGL3), Android, and HTML targets

---

### 16. Sprite Utils — sprite utilities and assets

🔗 https://github.com/openeggbert/sprite-utils · 📏 ≈1.2k LOC

* small C++23 sprite utility library and assets (number spritesheets, web component) supporting the game projects

---

### 17. YouTube Frontend — static index generator for ArchiveBox

🔗 https://github.com/openeggbert/youtube-frontend · 🌐 https://youtube.openeggbert.com · 📏 ≈1.4k LOC

* C++23 tool that generates static HTML index pages for ArchiveBox video archives
* uses OpenCV, FFmpeg libraries, and libcurl

---

### 18. 🧠 Hive — backend platform

🔗 https://github.com/robertvokac/hive · 🌐 https://hive.robertvokac.com · 📏 ≈45.0k LOC

* metadata-driven C++23 backend system
* custom ORM, migrations, REST API generator
* plugin architecture (models, jobs, triggers, queries)
* scheduler + event-driven automation

➡️ Focus: **backend systems, platform design, architecture**

---

### 19. bit-backup — bit rot detection

🔗 https://github.com/robertvokac/bit-backup · 📏 ≈3.1k LOC

* command-line tool that detects silent data corruption via SHA-512 checksums stored in SQLite (C++23, OpenSSL)
* parallel hashing, ignore patterns, rotating scrub verification, CSV reporting for cron integration

---

### 20. Lexicon — desktop knowledge dictionary

🔗 https://github.com/robertvokac/lexicon · 🌐 https://lexicon.robertvokac.com · 📏 ≈2.8k LOC

* desktop knowledge dictionary for structured technical notes (C++23, Qt 6 Widgets, SQLite)
* typed term relationships with backlinks, Markdown content with live preview, full-text search

---

¹ *LOC measured with cloc (July 2026): C++ sources and headers (`.cpp`/`.hpp`/`.h`), `src/` and `include/` directories only, excluding tests, vendored, and third-party code.*

---

## 🧭 Why I build runtimes and frameworks

Runtimes and compatibility layers force:

* precise API design
* understanding of system behavior
* control over execution model
* clear ownership and lifecycle
* deep debugging of real-world software

> behaviorally accurate, modular, and architecture-driven — not just feature-driven

---

## 🔄 C++ Transition

After several years in enterprise backend development (Java),
I transitioned toward **system-level engineering in C++**.

Since my previous work did not involve C++ directly,
I built expertise through **real implementations**, including:

* a 3D scene editor and a procedural world generator (Mesh Craft + Mesh World)
* cross-platform C++ framework running real games (Windows / Linux / WebAssembly / Android)
* DirectX 3 / WinAPI compatibility layers
* backend platform (≈45k LOC)
* multiple reusable system libraries

---

## 🧰 Tech Focus

* C++20/23
* Linux, CMake, Git, GCC / Clang
* SDL3, OpenGL / OpenGL ES, bgfx, Dear ImGui
* SQLite, Lua (sol2)
* 3D tooling, cross-platform frameworks, compatibility layers, runtime systems, system architecture

---

## 📫 Contact

* Email: [robertvokac@robertvokac.com](mailto:robertvokac@robertvokac.com)
* Web: https://robertvokac.com
* GitHub: https://github.com/robertvokac
* Org: https://github.com/openeggbert · https://openeggbert.com
* LinkedIn: https://cz.linkedin.com/in/robert-vok%C3%A1%C4%8D-081170381/
* Location: Prague, Czech Republic

---

⭐ **Pinned repositories show my current direction and strongest work**
