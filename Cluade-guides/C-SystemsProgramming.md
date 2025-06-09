# C Systems Programming Learning Roadmap
*Written by cluade AI*

This roadmap organizes resources from beginner to advanced, building foundational knowledge before tackling complex topics.

## Phase 1: Development Environment & Tools (Start Here)

### Git Version Control (Essential First Step)
- **Git Book**: https://git-scm.com/book
  - *Complete guide to version control - master this first for managing your learning projects*
- **Interactive Git Tutorial**: https://learngitbranching.js.org/
  - *Visual way to understand branching and merging*

### Build Systems (Basic → Advanced)
- **GNU Make Manual**: https://www.gnu.org/software/make/manual/make.html
  - *Start with simple compilation, then learn pattern rules and automatic variables*
- **CMake Tutorial**: https://cmake.org/cmake/help/latest/guide/tutorial/index.html
  - *Cross-platform builds - learn after mastering basic Makefiles*

## Phase 2: Networking Fundamentals (Theory Before Practice)

### Networking Theory
- **Computer Networking: A Top-Down Approach** (Kurose & Ross)
  - Official site: https://gaia.cs.umass.edu/kurose_ross/index.php
  - Free lectures: https://gaia.cs.umass.edu/kurose_ross/online_lectures.htm
  - Amazon: https://www.amazon.com/Computer-Networking-Top-Down-Approach-7th/dp/0133594149
  - *Essential theory - understand protocols before implementing them*

### Network Analysis Tools
- **Wireshark**: https://www.wireshark.org/
- **Documentation**: https://www.wireshark.org/docs/
  - *Learn to capture and analyze packets - great for understanding theory in practice*

## Phase 3: C Systems Programming (Foundation for Everything)

### System-Level Programming
- **TCP/IP Illustrated Vol 1** (Stevens)
  - Amazon: https://www.amazon.com/TCP-Illustrated-Vol-Addison-Wesley-Professional/dp/0201633469
  - Free version: https://freecomputerbooks.com/TCP-IP-Illustrated-Vol-1-The-Protocols.html
  - *Deep dive into network protocols - pairs with Kurose/Ross*

- **Linux Programming Interface**: https://man7.org/tlpi/
  - *System calls, file I/O, process management - core Linux programming*

- **Windows API Documentation**: https://docs.microsoft.com/en-us/windows/win32/
  - *For cross-platform development - learn after Linux basics*

### Debugging Tools (Learn Early, Use Always)
- **GDB Documentation**: https://www.gnu.org/software/gdb/documentation/
  - *Master debugging before complex projects*
- **Valgrind Manual**: https://valgrind.org/docs/manual/
  - *Memory error detection - crucial for C programming*

## Phase 4: Network Programming in C (Apply Theory)

### Socket Programming
- **Unix Network Programming** (Stevens) - Referenced in TCP/IP Illustrated above
  - *The definitive guide - work through examples systematically*
  - *Build: echo server → HTTP client → chat app → multi-threaded server*

**Practice Projects** (in order):
1. Simple echo client/server
2. HTTP client that fetches web pages
3. Multi-client chat server
4. Basic web server

## Phase 5: Graphics Programming (Choose Your Path)

### Path A: High-Level Graphics (Easier Start)
- **SDL2 Installation**: https://wiki.libsdl.org/SDL2/Installation
- **SDL2 Tutorials**: https://wiki.libsdl.org/SDL2/Tutorials
- **SDL2 Building Guide**: https://www.studyplan.dev/sdl2/building-sdl
  - *Good introduction to graphics concepts with less hardware complexity*

- **LearnOpenGL**: https://learnopengl.com
- **Code Repository**: https://learnopengl.com/Code-repository
  - *Modern 3D graphics - learn after 2D SDL basics*

### Path B: Bare Metal Graphics (Your Preferred Path - Advanced)

#### Start with Linux Framebuffer (Easier than VGA)
- **Kevin Boone's Linux Framebuffer Guide**: https://kevinboone.me/linuxfbc.html
  - *Practical C framebuffer programming - excellent starting point*
- **Toradex Framebuffer Tutorial**: https://developer.toradex.com/linux-bsp/application-development/multimedia/framebuffer-linux/
  - *Another practical guide with examples*
- **Linux Kernel Framebuffer Docs**: https://www.kernel.org/doc/html/v5.15/fb/framebuffer.html
  - *Official documentation - reference after practical tutorials*

#### Progress to VGA Hardware Programming (Most Advanced)
- **Mode 13h Wikipedia**: https://en.wikipedia.org/wiki/Mode_13h
  - *Theory and background - understand before coding*
- **VGA Mode 13h Assembly Tutorial**: https://thiscouldbebetter.wordpress.com/2011/03/17/vga-mode-13h-in-assembly-with-direct-memory-writes/
  - *Practical implementation guide*
- **Graphics Programming Tutorial**: http://devdocs.inightmare.org/tutorials/x86-assembly-graphics-part-i-mode-13h.html
  - *Step-by-step VGA programming*
- **Programming the VGA Guide**: http://www.fysnet.net/modex.htm
  - *Comprehensive VGA hardware reference*

#### Code Examples (Study These After Theory)
- **REND13X VGA Renderer**: https://github.com/Roninkoi/REND13X
  - *Real C + Assembly VGA renderer*
- **8086 Graphics Examples**: https://github.com/amrwc/8086-graphics
  - *Various graphics programming examples*
- **Bare Metal x86 Code**: https://gist.github.com/lucasw/019ded8bf79557081e7fed7d2e4e7506
  - *Low-level examples*

## Phase 6: Advanced C Programming & Optimization

### Advanced C Concepts
- **Expert C Programming: Deep C Secrets** (Peter van der Linden)
  - Amazon: https://www.amazon.com/Expert-Programming-Peter-van-Linden/dp/0131774298
  - Free version: https://freecomputerbooks.com/Expert-C-Programming-Deep-C-Secrets.html
  - Archive.org: https://archive.org/details/expert-c-programming-deep-c-secrets-by-peter-van-der-linden
  - *Advanced C idioms, pitfalls, and professional techniques*

- **C Puzzles and Traps** (Andrew Koenig)
  - *Common C programming mistakes and how to avoid them*

- **Advanced C Programming by Example** (John Perry)
  - Amazon: https://www.amazon.com/Advanced-Programming-Example-John-Perry/dp/0534951406
  - *Practical advanced C programming techniques*

### Performance Optimization & Profiling
- **Write Great Code Series** (Randall Hyde)
  - Volume 1: Understanding the Machine
  - Volume 2: Thinking Low-Level, Writing High-Level
  - *Hardware-aware programming for maximum performance*

- **Optimizing C++** (Steve Heller)
  - Amazon: https://www.amazon.com/Optimizing-C-Steve-Heller/dp/0139774300
  - *Performance optimization techniques (applies to C as well)*

### Memory Management & Data Structures
- **Hacker's Delight** (Henry Warren)
  - *Bit manipulation tricks and low-level optimization*

- **Data Structures and Algorithm Analysis in C** (Mark Weiss)
  - *Efficient algorithms and data structures for performance*

### Assembly Language Integration
- **Programming from the Ground Up** (Jonathan Bartlett)
  - *Assembly language programming - crucial for optimization*

- **x86-64 Assembly Language Programming with Ubuntu** (Ed Jorgensen)
  - *Modern x86-64 assembly for C integration*

### Profiling and Analysis Tools
- **Intel VTune Profiler**: https://www.intel.com/content/www/us/en/develop/tools/oneapi/components/vtune-profiler.html
  - *CPU performance profiling*

- **Perf Tools**: https://perf.wiki.kernel.org/index.php/Main_Page
  - *Linux performance analysis*

- **Cachegrind (Valgrind)**: https://valgrind.org/docs/manual/cg-manual.html
  - *Cache performance analysis*

### Compiler Optimization
- **GCC Optimization Options**: https://gcc.gnu.org/onlinedocs/gcc/Optimize-Options.html
  - *Understanding compiler optimizations*

- **Clang Optimization Guide**: https://clang.llvm.org/docs/CommandGuide/clang.html
  - *Alternative compiler optimization techniques*

## Phase 7: Kernel-Level Graphics & Advanced Hardware

### Kernel-Level Graphics
- **Frame Buffer Library API**: https://www.kernel.org/doc/html/latest/driver-api/frame-buffer.html
- **Framebuffer Console**: https://www.kernel.org/doc/html/latest/fb/fbcon.html
  - *Deep kernel graphics programming*

## Recommended Learning Timeline

**Weeks 1-2**: Git, Make, basic development setup
**Weeks 3-6**: Networking theory (Kurose/Ross), Wireshark practice
**Weeks 7-10**: System programming fundamentals, debugging tools
**Weeks 11-16**: Socket programming, network projects
**Weeks 17-20**: Choose graphics path - start with framebuffer
**Weeks 21-24**: Advanced VGA programming and projects
**Weeks 25-30**: Advanced C programming, optimization techniques
**Weeks 31+**: Performance profiling, assembly integration, kernel programming

## Key Success Strategies

1. **Build projects at each phase** - don't just read
2. **Master debugging early** - you'll need it constantly
3. **Start simple, add complexity gradually**
4. **Keep detailed notes in your Git repo** - you'll reference them often
5. **For bare metal graphics**: Start with framebuffer before VGA hardware
6. **Test on real hardware when possible** - virtual machines can hide timing issues

## Suggested Git Repository Structure

```
/learning-systems-programming/
├── notes/
│   ├── git-and-tools/
│   ├── networking-theory/
│   ├── systems-programming/
│   ├── network-programming/
│   ├── graphics-programming/
│   ├── advanced-c-programming/
│   └── optimization-and-performance/
├── projects/
│   ├── networking/
│   ├── graphics-framebuffer/
│   ├── graphics-vga/
│   └── optimization-examples/
└── resources/
    └── bookmarks-and-references.md
```

Good luck on your systems programming journey! The bare metal graphics path is challenging but incredibly rewarding.
