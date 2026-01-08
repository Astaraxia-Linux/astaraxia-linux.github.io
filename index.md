---
layout: default
title: Home
---

# Astaraxia Linux

> A minimal, source-based Linux distribution for control freaks who enjoy compiling.

## What is Astaraxia?

Astaraxia is a POSIX-compliant, source-based Linux distribution that follows these principles:

- **Minimalism**: Only install what you need
- **Transparency**: Every package built from source
- **Simplicity**: Easy to understand, modify, and maintain
- **Control**: You decide what goes into your system

## Quick Start
```bash
# Download latest stage3
wget https://github.com/Astaraxia-Linux/Horizon/releases/latest/stage3.tar.xz

# Extract
tar xvf stage3.tar.xz -C /mnt/lfs

# Bootstrap
astral -h --init
```

## Features

### Astral Package Manager
Minimal POSIX shell-based package manager. No Python, no systemd dependency, just shell scripts.

### Three Recipe Formats
- **v1**: Legacy @SECTION format
- **v2**: Modern $PKG.* syntax
- **v3**: Separated build/runtime dependencies

### LFS-Style Bootstrap
Build your system from scratch with [Horizon](/docs/horizon), our 3-stage bootstrap system.

## Why Astaraxia?

| Feature | Astaraxia | Gentoo | Arch | LFS |
|---------|-----------|--------|------|-----|
| Source-based | ✓ | ✓ | ✗ | ✓ |
| Binary packages | Soon™ | ✓ | ✓ | ✗ |
| POSIX sh | ✓ | ✗ | ✗ | ✗ |
| Systemd-free | ✓ | Optional | ✗ | ✓ |
| Easy bootstrap | ✓ | ✓ | ✗ | Manual |

## Community

- **GitHub**: [Astaraxia-Linux](https://github.com/Astaraxia-Linux)
- **Packages**: [AOHARU](https://github.com/Izumi-Sonoka/AOHARU) (official)
- **Community**: [ASURA](https://codeberg.org/Izumi/ASURA) (overlay)
- **IRC**: #astaraxia on Libera.Chat (coming soon)

## Latest News

**2026-01-08**: Astral 3.3.0.0 released with Git support and chroot feature!

## Get Started

1. [Download](/download) - Get stage3 tarball or ISO
2. [Documentation](/docs) - Read the installation guide
3. [Packages](/packages) - Browse available packages
4. [GitHub](https://github.com/Astaraxia-Linux) - Contribute!

---

*"Because life's too short to not compile everything from source"*
