# Astaraxia Linux 

> **"Tranquility through source-based minimalism."**

Astaraxia is a POSIX-compliant, source-based Linux distribution built from the ground up for users who want total control. No systemd, no bloat, just pure shell-driven automation.

---

##  The Core Components

- **Astral:** A monolithic, 5,000+ line pure POSIX `sh` package manager. 
- **Horizon:** The automated bootstrap engine that drives the 3-stage LFS-style deployment.
- **Recipes:** Versatile metadata formats (v1, v2, v3) for building software from source.

---

##  Quick Start

You can bootstrap Astaraxia from any existing Linux environment using the Astral engine:

```bash
# Fetch the engine
curl -O [https://raw.githubusercontent.com/Astaraxia-Linux/Astral/main/astral](https://raw.githubusercontent.com/Astaraxia-Linux/Astral/main/astral)
chmod +x astral
sudo mv astral /usr/bin/

# Initialize the Horizon bootstrap
export LFS=/mnt/lfs
sudo astral -h --init

# Run stages (Compilation heavy)
sudo astral -h --stage 1
