---
layout: default
title: Download
---

# Download Astaraxia

## Stage Tarballs (Recommended)

Stage tarballs are pre-built base systems. Extract and bootstrap from there.

### Latest Release: v0.1.0 (Alpha)

| File | Size | SHA256 |
|------|------|--------|
| [stage3-amd64.tar.xz](https://github.com/Astaraxia-Linux/Horizon/releases) | ~500MB | Coming soon |
| [stage3-arm64.tar.xz](https://github.com/Astaraxia-Linux/Horizon/releases) | ~450MB | Coming soon |

## Bootstrap from Scratch

Don't trust pre-built tarballs? Build everything yourself with Horizon.
```bash
# Install Astral
curl -O https://raw.githubusercontent.com/Astaraxia-Linux/Astral/main/astral
chmod +x astral
sudo mv astral /usr/bin/

# Initialize Horizon
export LFS=/mnt/lfs
sudo mkdir -pv $LFS
sudo astral -h --init

# Run stages (12-20 hours)
sudo astral -h --stage 1
sudo astral -h --stage 2
sudo astral --chroot $LFS
astral -h --stage 3
```

## Live ISO (Coming Soon)

A live environment for trying Astaraxia without installation.

- [ ] astaraxia-live-2026.01.iso
- [ ] Includes installer
- [ ] NetworkManager pre-configured

## Mirrors

**Primary**: GitHub Releases  
**Mirror 1**: Coming soon  
**Mirror 2**: Coming soon

## Verify Downloads
```bash
# Check SHA256
sha256sum -c stage3-amd64.tar.xz.sha256

# Check GPG signature (when available)
gpg --verify stage3-amd64.tar.xz.sig
```

## System Requirements

### Minimum
- CPU: x86_64 or ARM64
- RAM: 512MB
- Disk: 10GB
- Time: Patience

### Recommended
- CPU: Multi-core (for parallel compilation)
- RAM: 4GB+
- Disk: 20GB+
- Time: Lots of coffee

## Next Steps

After downloading:
1. [Installation Guide](/docs/install)
2. [Horizon Bootstrap](/docs/horizon)
3. [Package Management](/docs/astral)
