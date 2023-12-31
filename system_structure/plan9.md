# Plan 9 from Bell Labs (1990)
Reference: https://github.com/parasj/papers/blob/master/os_structures/plan9.md?plain=1

The Plan 9 paper addressed the challenge of managing computing resources and facilitating inter-process communication (IPC) in a networked environment. It looked at the difficulties in administering multiple self-maintained machines and the challenges posed by distributed systems.


**Key ideas**:
1. Everything is a file (incl. hardware, window manager)
2. Central server with clients rendering windows. This centralizes administration while allowing users to customize their workspace.
3. Integrated backups each day
4. Per process namespaces

## Motivation
Small self-maintained machines made it easier for users to do work but made administration much more difficult. Instead Plan 9 uses network storage and CPU to do work. Per-process namespaces led to easier distributed systems and IPC.

## Key principles
1. Resources are named and accessed like files in FS
2. Standard protocol for accessing these resources
3. All resources in one single hierarchical namespace
