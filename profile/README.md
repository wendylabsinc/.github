# Wendy Labs

Welcome to Wendy Labs! We're building the future of edge computing and IoT development with powerful, developer-friendly tools for building, deploying, and managing applications on edge devices.

- **Main Documentation**: https://wendy.sh/docs/
- **Website**: https://wendy.sh

## What is Wendy?

**Wendy** is a comprehensive CLI and development platform that makes it simple to build, deploy, and debug applications on edge devices like NVIDIA Jetson, Raspberry Pi, and other ARM-based hardware. It brings the ease of modern cloud development to the edge computing world.

### Key Features

- **Multi-Language Support**: Build applications in Swift, Python, Rust, TypeScript/Node.js, and more
- **Cross-Platform Development**: Develop on macOS or Linux, deploy to ARM devices
- **Container-Based Deployment**: Automatic Docker containerization and multi-architecture builds
- **Remote Debugging**: Full LLDB debugging support for edge applications
- **Developer Experience**: Simple commands like `wendy run` handle all the complexity
- **Privacy-First Analytics**: Optional anonymous usage analytics to help improve the developer experience

## What is WendyOS?

**WendyOS** is a custom Linux distribution based on Yocto/OpenEmbedded, specifically optimized for edge computing devices. It provides a minimal, secure, and production-ready operating system for IoT and edge applications.

### Key Features

- **Hardware-Optimized**: Purpose-built for NVIDIA Jetson Orin Nano and other edge devices
- **OTA Updates**: Built-in Mender integration for reliable over-the-air updates with A/B partition redundancy
- **Minimal Footprint**: Headless, systemd-based init, optimized for embedded systems
- **Production Ready**: Secure, stable, and designed for long-term deployment
- **Developer Friendly**: Pre-configured with Docker, SSH, and development tools

### Core Platform

#### [wendy-agent](https://github.com/wendylabsinc/wendy-agent)
The heart of the Wendy platform - a CLI and app manager for WendyOS written in Swift. Handles application deployment, debugging, and device management.

**Key Features:**
- Swift 6.2+ with modern async/await
- Docker-based application management
- Remote debugging with LLDB
- Network configuration (NetworkManager/ConnMan support)
- Privacy-first analytics

#### [wendy-vscode](https://github.com/wendylabsinc/wendy-vscode)
Visual Studio Code extension for Wendy development, providing seamless integration with the Wendy CLI and device management.

#### [samples](https://github.com/wendylabsinc/samples)
Sample applications demonstrating how to build applications with Wendy across multiple languages:
- Python (hello-world)
- Swift (hello-world)
- Rust (hello-world, simple-server)
- Node.js/TypeScript (hello-world, simple-server)

### Operating System

#### [meta-wendyos-jetson](https://github.com/wendylabsinc/meta-wendyos-jetson)
Yocto meta-layer for building WendyOS for NVIDIA Jetson Orin Nano Developer Kit. Includes Docker-based build environment and Mender OTA update support.

**Features:**
- Yocto-based
- Multiple image size configurations (4GB-64GB)
- NVMe and eMMC/SD card support
- OTA Updates

### System Libraries (Swift)

#### [dbus](https://github.com/wendylabsinc/dbus)
Pure Swift 6 D-Bus protocol implementation with SwiftNIO and modern concurrency support. Enables interprocess communication on Linux systems.

#### [bluetooth](https://github.com/wendylabsinc/bluetooth)
Swift Bluetooth (Bluez) library for Linux, enabling BLE communication on edge devices.

#### [gstreamer](https://github.com/wendylabsinc/gstreamer)
Swift 6.2 GStreamer wrapper for robotics and computer vision applications on Jetson devices.

#### [tensorrt-swift](https://github.com/wendylabsinc/tensorrt-swift)
TensorRT Swift 6.2 bindings for Linux, enabling high-performance deep learning inference on NVIDIA hardware.

#### [deepstream-swift](https://github.com/wendylabsinc/deepstream-swift)
DeepStream Swift bindings for building intelligent video analytics applications.

---

Built with ❤️ by Wendy Labs
