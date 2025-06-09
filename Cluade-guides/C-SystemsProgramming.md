# C Systems Programming Learning Roadmap
*written by Cluade*

This roadmap organizes resources from beginner to advanced, building foundational knowledge before tackling complex topics.

---

# Phase 1: Development Environment & Tools

## Git Version Control (Essential First Step)
- **Git Book**: https://git-scm.com/book
  - *Complete guide to version control - master this first for managing your learning projects*
- **Interactive Git Tutorial**: https://learngitbranching.js.org/
  - *Visual way to understand branching and merging*

## Build Systems (Basic → Advanced)
- **GNU Make Manual**: https://www.gnu.org/software/make/manual/make.html
  - *Start with simple compilation, then learn pattern rules and automatic variables*
- **CMake Tutorial**: https://cmake.org/cmake/help/latest/guide/tutorial/index.html
  - *Cross-platform builds - learn after mastering basic Makefiles*

## Phase 1 Projects:
1. **Basic Makefile** - Compile single C file with dependencies
2. **Multi-file Makefile** - Separate compilation, object files, clean targets
3. **Library Creation** - Static and dynamic library compilation
4. **CMake Project** - Cross-platform build configuration
5. **Git Workflow** - Branching, merging, conflict resolution practice

---

# Phase 2: Networking Fundamentals

## Networking Theory
- **Computer Networking: A Top-Down Approach** (Kurose & Ross)
  - Official site: https://gaia.cs.umass.edu/kurose_ross/index.php
  - Free lectures: https://gaia.cs.umass.edu/kurose_ross/online_lectures.htm
  - Amazon: https://www.amazon.com/Computer-Networking-Top-Down-Approach-7th/dp/0133594149
  - *Essential theory - understand protocols before implementing them*

## Network Analysis Tools
- **Wireshark**: https://www.wireshark.org/
- **Documentation**: https://www.wireshark.org/docs/
  - *Learn to capture and analyze packets - great for understanding theory in practice*

## Phase 2 Projects:
1. **Protocol Analysis** - Capture and analyze HTTP, TCP, UDP packets with Wireshark
2. **Network Topology Mapping** - Document your local network structure
3. **Packet Inspection** - Identify different protocol layers in real traffic
4. **Network Troubleshooting** - Use Wireshark to debug connectivity issues

---

# Phase 3: C Systems Programming

## System-Level Programming
- **TCP/IP Illustrated Vol 1** (Stevens)
  - Amazon: https://www.amazon.com/TCP-Illustrated-Vol-Addison-Wesley-Professional/dp/0201633469
  - Free version: https://freecomputerbooks.com/TCP-IP-Illustrated-Vol-1-The-Protocols.html
  - *Deep dive into network protocols - pairs with Kurose/Ross*

- **Linux Programming Interface**: https://man7.org/tlpi/
  - *System calls, file I/O, process management - core Linux programming*

- **Windows API Documentation**: https://docs.microsoft.com/en-us/windows/win32/
  - *For cross-platform development - learn after Linux basics*

## Debugging Tools (Learn Early, Use Always)
- **GDB Documentation**: https://www.gnu.org/software/gdb/documentation/
  - *Master debugging before complex projects*
- **Valgrind Manual**: https://valgrind.org/docs/manual/
  - *Memory error detection - crucial for C programming*

## Phase 3 Projects:
1. **File System Explorer** - Directory traversal, file operations
2. **Process Manager** - Fork, exec, wait, signal handling
3. **Pipe Communication** - Inter-process communication using pipes
4. **Shared Memory** - Data sharing between processes
5. **Signal Handler** - Custom signal processing and cleanup
6. **Memory Debugger Practice** - Find and fix memory leaks with Valgrind

---

# Phase 4: Network Programming in C

## Socket Programming
- **Unix Network Programming** (Stevens) - Referenced in TCP/IP Illustrated above
  - *The definitive guide - work through examples systematically*
  - *Build: echo server → HTTP client → chat app → multi-threaded server*

## Phase 4 Projects:
1. **Simple Echo Server/Client** - Basic socket programming
2. **HTTP Client** - Fetch web pages, parse headers
3. **Multi-threaded Chat Server** - Handle multiple clients simultaneously  
4. **Basic Web Server** - Serve static files, handle HTTP requests
5. **Network Scanner** - Port scanning, service detection
6. **Simple FTP Client** - File transfer protocol implementation
7. **DNS Resolver** - Query DNS servers directly
8. **Packet Sniffer** - Capture and analyze network packets (using raw sockets)

---

# Phase 5: Bare Metal Graphics Programming

## Linux Framebuffer Programming
- **Kevin Boone's Linux Framebuffer Guide**: https://kevinboone.me/linuxfbc.html
  - *Practical C framebuffer programming - excellent starting point*
- **Toradex Framebuffer Tutorial**: https://developer.toradex.com/linux-bsp/application-development/multimedia/framebuffer-linux/
  - *Another practical guide with examples*
- **Linux Kernel Framebuffer Docs**: https://www.kernel.org/doc/html/v5.15/fb/framebuffer.html
  - *Official documentation - reference after practical tutorials*

## VGA Hardware Programming
- **Mode 13h Wikipedia**: https://en.wikipedia.org/wiki/Mode_13h
  - *Theory and background - understand before coding*
- **VGA Mode 13h Assembly Tutorial**: https://thiscouldbebetter.wordpress.com/2011/03/17/vga-mode-13h-in-assembly-with-direct-memory-writes/
  - *Practical implementation guide*
- **Graphics Programming Tutorial**: http://devdocs.inightmare.org/tutorials/x86-assembly-graphics-part-i-mode-13h.html
  - *Step-by-step VGA programming*
- **Programming the VGA Guide**: http://www.fysnet.net/modex.htm
  - *Comprehensive VGA hardware reference*

## Code Examples
- **REND13X VGA Renderer**: https://github.com/Roninkoi/REND13X
  - *Real C + Assembly VGA renderer*
- **8086 Graphics Examples**: https://github.com/amrwc/8086-graphics
  - *Various graphics programming examples*
- **Bare Metal x86 Code**: https://gist.github.com/lucasw/019ded8bf79557081e7fed7d2e4e7506
  - *Low-level examples*

## Phase 5 Projects:

### Framebuffer Projects:
1. **Pixel Drawing Program** - Set individual pixels, draw lines
2. **Basic Shape Renderer** - Rectangles, circles, polygons
3. **Bitmap Font Renderer** - Display text without libraries
4. **Simple Paint Program** - Interactive drawing with mouse/keyboard
5. **Image Viewer** - Load and display raw image files
6. **2D Game Engine** - Sprites, collision detection, game loop
7. **Mandelbrot Set Visualizer** - Complex mathematical visualization

### VGA Hardware Projects:
8. **Mode 13h Setup** - Initialize 320x200 256-color mode
9. **Palette Programming** - Custom color palettes, palette animation
10. **Basic VGA Graphics** - Pixels, lines, circles in assembly/C
11. **VGA Text Mode** - Custom fonts, colored text display
12. **Hardware Scrolling** - Smooth scrolling backgrounds
13. **Mode X Programming** - Higher resolution modes (320x240, 360x480)
14. **VGA Raycaster** - Simple 3D engine like early Doom
15. **Copper Bar Effects** - Hardware-timed palette changes
16. **Hardware Sprites** - Fast sprite rendering with VGA tricks

---

# Phase 6: Advanced C Programming & Optimization

## Advanced C Concepts
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

## Performance Optimization & Profiling
- **Write Great Code Series** (Randall Hyde)
  - Volume 1: Understanding the Machine
  - Volume 2: Thinking Low-Level, Writing High-Level
  - *Hardware-aware programming for maximum performance*

- **Optimizing C++** (Steve Heller)
  - Amazon: https://www.amazon.com/Optimizing-C-Steve-Heller/dp/0139774300
  - *Performance optimization techniques (applies to C as well)*

## Memory Management & Data Structures
- **Hacker's Delight** (Henry Warren)
  - *Bit manipulation tricks and low-level optimization*

- **Data Structures and Algorithm Analysis in C** (Mark Weiss)
  - *Efficient algorithms and data structures for performance*

## Assembly Language Integration
- **Programming from the Ground Up** (Jonathan Bartlett)
  - *Assembly language programming - crucial for optimization*

- **x86-64 Assembly Language Programming with Ubuntu** (Ed Jorgensen)
  - *Modern x86-64 assembly for C integration*

## Profiling and Analysis Tools
- **Intel VTune Profiler**: https://www.intel.com/content/www/us/en/develop/tools/oneapi/components/vtune-profiler.html
  - *CPU performance profiling*

- **Perf Tools**: https://perf.wiki.kernel.org/index.php/Main_Page
  - *Linux performance analysis*

- **Cachegrind (Valgrind)**: https://valgrind.org/docs/manual/cg-manual.html
  - *Cache performance analysis*

## Compiler Optimization
- **GCC Optimization Options**: https://gcc.gnu.org/onlinedocs/gcc/Optimize-Options.html
  - *Understanding compiler optimizations*

- **Clang Optimization Guide**: https://clang.llvm.org/docs/CommandGuide/clang.html
  - *Alternative compiler optimization techniques*

## Phase 6 Projects:
1. **Memory Pool Allocator** - Custom memory management system
2. **Lock-Free Data Structures** - Queue, stack, hash table without mutexes
3. **SIMD Optimization** - Vector operations using intrinsics
4. **Cache-Friendly Algorithms** - Data structure layout optimization
5. **Bit Manipulation Library** - Fast bit operations, compression
6. **Custom String Library** - Optimized string operations
7. **High-Performance Hash Table** - Robin Hood hashing, open addressing
8. **Assembly Integration** - Critical loops in assembly language
9. **Profiler Integration** - Add profiling to existing projects
10. **Benchmark Suite** - Performance testing framework

---

# Phase 7: Kernel-Level Graphics & Advanced Hardware

## Kernel-Level Graphics
- **Frame Buffer Library API**: https://www.kernel.org/doc/html/latest/driver-api/frame-buffer.html
- **Framebuffer Console**: https://www.kernel.org/doc/html/latest/fb/fbcon.html
  - *Deep kernel graphics programming*

## Phase 7 Projects:
1. **Custom Framebuffer Driver** - Write a basic framebuffer kernel module
2. **Boot Loader Graphics** - Display graphics before OS loads
3. **Embedded Graphics System** - Bare metal graphics on microcontroller
4. **Game Engine** - Combine networking, graphics, and optimization
5. **3D Software Renderer** - No GPU, pure CPU 3D rendering
6. **Network Graphics Protocol** - Send graphics commands over network
7. **Real-Time Graphics** - Hard timing constraints, no frame drops
8. **Multi-Core Graphics** - Parallel rendering across CPU cores

---

# Recommended Learning Timeline

**Weeks 1-2**: Git, Make, basic development setup
**Weeks 3-6**: Networking theory (Kurose/Ross), Wireshark practice
**Weeks 7-10**: System programming fundamentals, debugging tools
**Weeks 11-16**: Socket programming, network projects
**Weeks 17-20**: Framebuffer programming basics
**Weeks 21-24**: Advanced VGA programming and projects
**Weeks 25-30**: Advanced C programming, optimization techniques
**Weeks 31+**: Performance profiling, assembly integration, kernel programming

# Key Success Strategies

1. **Build projects at each phase** - don't just read
2. **Master debugging early** - you'll need it constantly
3. **Start simple, add complexity gradually**
4. **Keep detailed notes in your Git repo** - you'll reference them often
5. **For bare metal graphics**: Start with framebuffer before VGA hardware
6. **Test on real hardware when possible** - virtual machines can hide timing issues
7. **Learn optimization systematically**: Understand before optimizing
8. **Profile before optimizing**: Measure performance bottlenecks first
9. **Study assembly language**: Essential for true optimization mastery

Good luck on your systems programming journey! The bare metal graphics path is challenging but incredibly rewarding.