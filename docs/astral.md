---
layout: default
title: Astral Package Manager
---

# Astral Package Manager

Minimal POSIX package manager for Astaraxia.

## Basic Usage
```bash
# Install package
sudo astral -S package-name

# Remove package
sudo astral -R package-name

# Search packages
astral -s keyword

# Update repos
sudo astral -u
```

## Features
- POSIX sh (no bash required)
- Three recipe formats (v1, v2, v3)
- Dependency resolution
- Git repository support
- Chroot environments

See [GitHub](https://github.com/Astaraxia-Linux/Astral) for full documentation.
