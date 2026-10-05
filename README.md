# Quentin Morineau

## C/C++ Developer | Systems & Graphics Programming | Brussels

Student at 42 Belgium, after 12 years as a pastry chef in international kitchens. I build low-level C/C++ software: system utilities, real-time renderers and GPU simulations, with a focus on memory behavior and performance. Open to roles in systems, graphics and embedded.

[LinkedIn](https://www.linkedin.com/in/quentin-morineau) / q.morineau@gmail.com

---

## Projects

### [particle_system (GPU Particle Simulator)](https://github.com/qmorineau/particle_system) | C++17, OpenGL, compute shaders

Real-time particle simulator running entirely on the GPU: 6 million particles at a steady 60 FPS on a 2013 iMac (Linux), and 120 FPS (display-capped) on an RTX 40-series GPU.

* Simulation done in compute shaders, with particle state stored in SSBOs (no CPU readback).

* Smoke rendering mode with textured quads, lifetime-based opacity and size.

* Runtime controls for emitter position, gravity point, particle count and speed.

### [ft_ls (System Listing Utility)](https://github.com/qmorineau/ft_ls) | C

Clone of the Unix `ls`, within ~1.1-2x of GNU `ls` execution time.

* Used `statx(2)` field masking to reduce the data copied from kernel to userland.

* Wrote a custom pool allocator to cut allocation overhead on large recursive traversals.

* Batched output through a 16 KB cache-aligned buffer to reduce `write` syscalls.

### [scop (OBJ Visualizer & Minimal 3D Engine)](https://github.com/qmorineau/scop) | C++17, OpenGL

Minimal 3D engine and OBJ viewer, built from scratch on Modern OpenGL.

* Modular architecture: windowing, input, GPU resources (VAO/VBO/EBO), scene graph, rendering.

* Custom OBJ/MTL parser (normals, UVs, materials, diffuse textures).

* Material-based lighting and textured modes, FPS and orbital cameras, real-time light editor.

### [abstract_data](https://github.com/qmorineau/abstract_data) | C++98 (in progress)

Reimplementation of STL containers under C++98, without using the STL.

* `vector`, `list` and iterator system implemented; `deque` and others in progress.

* Same test suite built against both the custom containers and the STL, outputs diffed, with ASan/UBSan.

### [Rubik (Cube Solver & Simulator)](https://github.com/qmorineau/rubik) | C++17, OpenGL

Real-time 3D Rubik's Cube simulator with an automatic solver.

* Implemented Kociemba's two-phase algorithm with precomputed pruning tables.
* Animated face rotations rendered with Modern OpenGL, with manual and scripted moves.
* Average solution length: 23.613 moves | Average solve time: 0.0668 s over 1,000 tests.

### [Transcendence (Real-Time Gaming Platform)](https://github.com/qmorineau/transcendance) | TypeScript, Node.js

Multiplayer Pong platform with an authoritative server, supporting 3D web and SSH CLI clients.

---

## Skills

| Category | Skills |
| :--- | :--- |
| **Languages** | C, C++ (98 and C++17), GLSL |
| **Graphics** | OpenGL, compute shaders, linear algebra, 3D transformations |
| **Systems** | Linux, syscalls, memory management, multithreading, processes and signals |
| **Tools** | Git, Make, Docker, gdb, valgrind, sanitizers |
| **Familiar with** | TypeScript/Node.js (Transcendence), PostgreSQL |
