# NixOS Laptop Configuration

Personal NixOS configuration for my laptop, managed with Nix flakes and Home Manager.

The configuration is designed for a modern desktop workflow with development tools, virtualization, container workloads, and common daily applications.

## Features

- NixOS 25.11
- GNOME desktop environment
- PipeWire audio with ALSA, PulseAudio, and JACK support
- Home Manager for user-level configuration
- Zsh with Oh My Zsh, autosuggestions, and syntax highlighting
- Git and GitHub CLI configuration
- Docker and Docker Compose
- Libvirt/QEMU/KVM with virt-manager
- Flatpak support
- Cloudflare WARP
- Bluetooth and NetworkManager
- Gaming-related tools such as MangoHud, GOverlay, and Steam support
- Increased file descriptor limits for development and gaming workloads
- `vm.max_map_count` configured for Steam and compatible applications
- Nix flakes and the Nix command enabled
- Additional packages from `nixpkgs-unstable`

## Repository Structure

| File | Description |
| --- | --- |
| `flake.nix` | Defines the inputs and the `nixos-btw` system configuration |
| `configuration.nix` | Main system configuration |
| `hardware-configuration.nix` | Hardware-specific configuration generated for the laptop |
| `home.nix` | User configuration managed by Home Manager |
| `flake.lock` | Locks all flake inputs to reproducible versions |

## Requirements

- A working NixOS installation
- A compatible x86_64 system
- Nix flakes enabled
- Basic familiarity with NixOS configuration

This configuration is personal and hardware-specific. It should be adapted before being used on another machine.

## Installation

Clone the repository:

```bash
git clone https://github.com/Pascal-Thommen/nixconf.git
cd nixconf
