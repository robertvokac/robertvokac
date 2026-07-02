# 👋 Robert Vokáč — C++ Systems Engineer

**Modern C++ · Cross-platform frameworks · Compatibility layers · Runtime systems**

---

## 🚀 Focus

C++ developer focused on **system-level engineering**, **cross-platform framework design**, and **compatibility layers**.

Looking for roles in:

* C++ systems engineering
* runtime / framework development
* cross-platform / platform abstraction work
* backend / platform architecture
* game technology / engine tooling

---

## 🧠 What I build

I design and implement **C++ frameworks, platform abstraction layers, and compatibility systems** in modern C++, focusing on:

* explicit API design
* system behavior reproduction
* modular architecture
* cross-platform execution (Windows · Linux · WebAssembly · Android)
* long-term maintainability

Validated on real-world applications (Planet Blupi 1996, Speedy Blupi 2001/2013)

---

## 🔥 Main Projects

### 🥇 CNA — C++ framework (XNA-style API)

🔗 https://github.com/openeggbert/cna · 🌐 https://libcna.com · 🌐 https://cna.openeggbert.com

* XNA-style API in native C++ under `Microsoft::Xna::Framework`
* rendering, input, audio, resource lifecycle, backend abstraction
* backends: SDL3 / OpenGL (easy-gl) / bgfx
* one codebase targets Windows, Linux, WebAssembly, and Android
* used to port a real C# / XNA game (Speedy Blupi, 2013)

➡️ Focus: **cross-platform framework, runtime systems, API compatibility**

---

### 🥈 Free Direct — DirectX 3 (2D) compatibility layer

🔗 https://github.com/openeggbert/free-direct · 🌐 https://freedirect.openeggbert.com

* reimplementation of DirectDraw / DirectSound subset over SDL3
* CPU surface model, blitting, palettes, color keys, locking, presentation
* designed to replace original DirectX 3 SDK dependencies in legacy applications

➡️ Focus: **low-level graphics systems, legacy API compatibility**

---

### 🥉 Free API — WinAPI compatibility layer

🔗 https://github.com/openeggbert/free-api · 🌐 https://freeapi.openeggbert.com

* WinAPI-style windowing, message loop, input, timers, multimedia APIs
* SDL3-based implementation (Linux / cross-platform)
* works together with Free Direct as the system/platform side of legacy application compatibility

➡️ Focus: **system APIs, OS abstraction, runtime behavior**

---

### easy-gl — OpenGL/OpenGL ES rendering wrapper

🔗 https://github.com/openeggbert/easy-gl · 🌐 https://easygl.openeggbert.com

* toolkit-independent C++20 OpenGL/OpenGL ES wrapper
* host owns window and GL context; easy-gl owns all OpenGL interaction
* built on top of meta-gl; used by CNA as its OpenGL rendering backend

---

### meta-gl — low-level OpenGL function loader

🔗 https://github.com/openeggbert/meta-gl · 🌐 https://metagl.openeggbert.com

* type-safe C++23 OpenGL ES 2.0+ function loader
* runtime loading via host-supplied `GetProcAddress` — no windowing, no context creation
* `enum class` wrappers for all OpenGL constants; foundation layer for easy-gl

---

### Sharp Runtime — C#/.NET subset in native C++

🔗 https://github.com/openeggbert/sharp-runtime · 🌐 https://sharpruntime.openeggbert.com

* `System::*` namespaces implemented in idiomatic modern C++
* covers exceptions, events, delegates, collections, and system-level building blocks
* foundation layer for CNA, Mesh Craft, Mesh World, and Galaxy Eggbert

---

### Galaxy Eggbert — 3D game (CNA)

🔗 https://github.com/openeggbert/galaxy-eggbert · 🌐 https://galaxyeggbert.openeggbert.com

* 3D remake of Speedy Blupi validating the full CNA engine stack
* targets Linux, Windows, WebAssembly, and Android from a single C++ codebase

---

### Mesh Craft — 3D scene editor

🔗 https://github.com/openeggbert/mesh-craft · 🌐 https://meshcraft3d.com · 🌐 https://meshcraft.openeggbert.com

* 3D scene editor for the `.mc3.xml` format — primitive shapes, CSG (union/difference/intersection via Manifold), materials, PBR textures, animation
* native `.mc3.xml` format: human-readable XML-based editable source compiled to glTF/GLB or binary MCB via `mc3togltf` / `mc3tomcb` CLI tools
* built on CNA + sharp-runtime; exercises the full C++ engine stack as a real editor application
* Early prototype — project structure, core class skeletons, and MC3 library in place

---

### Mesh World — procedural 3D world generator

🔗 https://github.com/openeggbert/mesh-world · 🌐 https://meshworld3d.com · 🌐 https://meshworld.openeggbert.com

* generates infinite 3D city and landscape chunks from a JSON config — 20 C++ chunk generators + 17 Lua object generators
* Lua scripting sandbox (sol2 + Lua 5.4) for content modding; auto-discovered at startup
* SQLite content packs: taxonomy registry, material registry, generator bundles in portable `.sqlite` files
* real-time 3D explorer (MeshWorldApp) built on Mesh Craft + CNA (SDL3/OpenGL)
* 119 tests passing, zero warnings, CI on every push

---

### 🧠 Hive (archived) — backend platform

🔗 https://github.com/robertvokac/hive

* ~44k LOC metadata-driven C++ backend system
* custom ORM, migrations, REST API generator
* plugin architecture (models, jobs, triggers, queries)
* scheduler + event-driven automation

➡️ Focus: **backend systems, platform design, architecture**

---

### Other utilities

* **Lexicon** — https://github.com/robertvokac/lexicon — desktop knowledge dictionary (C++23, Qt Widgets, SQLite)
* **bit-backup** — https://github.com/robertvokac/bit-backup — bit rot detection via SHA-512 checksums (C++23, SQLite, OpenSSL)

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

* cross-platform C++ framework running real games (Windows / Linux / WebAssembly / Android)
* DirectX 3 / WinAPI compatibility layers
* 3D engine with Urho3D scene graph + CNA rendering backends
* backend platform (~44k LOC)
* multiple reusable system libraries

---

## 🧰 Tech Focus

* C++20/23
* Linux, CMake, Git, GCC / Clang
* SDL3, OpenGL / OpenGL ES, bgfx
* SQLite
* cross-platform frameworks, compatibility layers, runtime systems, system architecture

---

## 📫 Contact

* Email: [robertvokac@robertvokac.com](mailto:robertvokac@robertvokac.com)
* GitHub: https://github.com/robertvokac
* Org: https://github.com/openeggbert
* LinkedIn: https://cz.linkedin.com/in/robert-vok%C3%A1%C4%8D-081170381/
* Location: Prague, Czech Republic

---

⭐ **Pinned repositories show my current direction and strongest work**
