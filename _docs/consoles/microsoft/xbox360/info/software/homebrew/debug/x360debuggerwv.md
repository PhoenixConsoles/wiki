---
title: X360DebuggerWV
description: Xbox 360 remote debugger for debug monitor
tags:
 - consoles
 - microsoft
 - xbox360
---

# X360DebuggerWV

A remote debugging application for the Xbox 360 debug monitor.

## Installation

You will need:

- XBDM
- JRPC2
- Xbox 360 Neighborhood
- [X360DebuggerWV](https://github.com/zeroKilo/X360DebuggerWV)

## Features

- General information, including Name, IP Address, CPU Key, Kernel Version, Current Executable
- File Browser, including previewing/saving files and running xex executables
- Modules: show base address in dump, show entry point in dump or CPU, explore sections
- Memory Regions: browse all allocated memory sections, see which module sections are inside
- Memory Dump: dump memory or write back to it with hex editor, load/save from/to file, hex pattern search
- CPU: play, pause, step(if breakpoint was reached, not yet working for branching!), disassembly of ppc, current threads, current thread's  registers, find end of a subfunction and export to XEXDecompiler 3  (integrated now)
- Trace: Load/save/clear and see register changes
- Overall Options: break on Module Load, break on Thread Create, record breakpoints to trace