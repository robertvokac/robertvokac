# 👋 Robert Vokáč - C++ Systems Engineer

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

---

## Projects

### 1. CNA - C++ framework (XNA-style API)

🔗 https://github.com/openeggbert/cna · 🌐 https://libcna.com · 🌐 https://cna.openeggbert.com · 🎮 [WebAssembly demo](https://speedyblupi.com/SpeedyBlupi2013/) · 📏 ≈292.2k LOC

* XNA-style API in native C++ under `Microsoft::Xna::Framework`
* rendering, input, audio, resource lifecycle, backend abstraction
* restructured into 15 independently buildable modules plus a renderer layer of ~40 backends, each with its own CMake target
* 46 rendering backends spanning modern APIs (Vulkan, bgfx, WebGPU, native Direct3D 9/10/11/12, SDL_GPU, Metal, Diligent Engine, Sokol), the full legacy DirectX line (DirectX 1–9, Wine/DXVK-verified), desktop and mobile OpenGL/OpenGL ES/OpenVG, and specialty targets (HTML Canvas, SVG, GDI, Glide, headless)
* one codebase targets Windows, Linux, WebAssembly, and Android
* used to port a real C# / XNA game (Speedy Blupi, 2013)

➡️ Focus: **cross-platform framework, runtime systems, API compatibility**

---

### 2. CNA Samples - XNA sample collection ported to C++

🔗 https://github.com/openeggbert/cna-samples · 📏 ≈48.0k LOC

* C++ ports of the official Microsoft XNA Game Studio 4.0 sample collection, running on CNA
* a continuously growing compatibility test bed proving the framework's API coverage on real code
* 🎮 web demos coming soon

---

### 3. Sharp Runtime - C#/.NET subset in native C++

🔗 https://github.com/openeggbert/sharp-runtime · 🌐 https://sharpruntime.openeggbert.com · 📏 ≈78.9k LOC

* `System::*` namespaces implemented in idiomatic modern C++
* covers exceptions, events, delegates, collections, and system-level building blocks
* restructured into 39 independently selectable modules (41 CMake components)
* foundation layer for CNA, Mesh Craft, and Galaxy Eggbert

Assembly, and Android from a single C++ codebase

---

### 4. easy-gl - OpenGL/OpenGL ES rendering wrapper

🔗 https://github.com/openeggbert/easy-gl · 🌐 https://easygl.openeggbert.com · 📏 ≈3.6k LOC

* toolkit-independent C++20 OpenGL/OpenGL ES wrapper
* host owns window and GL context; easy-gl owns all OpenGL interaction
* built on top of meta-gl; used by CNA as its OpenGL rendering backend

---

### 5. meta-gl - low-level OpenGL function loader

🔗 https://github.com/openeggbert/meta-gl · 🌐 https://metagl.openeggbert.com · 📏 ≈8.9k LOC

* type-safe C++23 OpenGL ES 2.0+ function loader
* runtime loading via host-supplied `GetProcAddress` — no windowing, no context creation
* `enum class` wrappers for all OpenGL constants; foundation layer for easy-gl

### 6. Lexicon - desktop knowledge dictionary

🔗 https://github.com/robertvokac/lexicon · 🌐 https://lexicon.robertvokac.com · 📏 ≈2.8k LOC

* desktop knowledge dictionary for structured technical notes (C++23, Qt 6 Widgets, SQLite)
* typed term relationships with backlinks, Markdown content with live preview, full-text search

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

* a 3D scene editor (Mesh Craft)
* cross-platform C++ framework running real games (Windows / Linux / WebAssembly / Android)
* DirectX 3 / WinAPI compatibility layers
* backend platform (≈45k LOC)
* multiple reusable system libraries

---

## 🧰 Tech Focus

* C++20/23
* Linux, CMake, Git, GCC / Clang
* SDL3, OpenGL / OpenGL ES
* SQLite
* 3D tooling, cross-platform frameworks, compatibility layers, runtime systems, system architecture

---

## 📫 Contact

* Email: [robertvokac@robertvokac.com](mailto:robertvokac@robertvokac.com)
* Web: https://robertvokac.com
* GitHub: https://github.com/robertvokac
* Org: https://github.com/libcna · https://libcna.com
* LinkedIn: https://cz.linkedin.com/in/robert-vok%C3%A1%C4%8D-081170381/
* Location: Prague, Czech Republic

---

⭐ **Pinned repositories show my current direction and strongest work**
