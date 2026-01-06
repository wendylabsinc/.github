# Wendy Labs

Welcome to Wendy Labs! We're building the future of edge computing and IoT development with powerful, developer-friendly tools for building, deploying, and managing applications on edge devices.

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

## Important Repositories

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
- Yocto Scarthgap-based
- Multiple image size configurations (4GB-64GB)
- NVMe and eMMC/SD card support
- Mender v5.0.x integration

### System Libraries (Swift)

#### [dbus](https://github.com/wendylabsinc/dbus)
Pure Swift 6 D-Bus protocol implementation with SwiftNIO and modern concurrency support. Enables interprocess communication on Linux systems.

**Features:**
- No C library dependencies
- Full async/await support
- Server-side object export
- BlueZ integration examples

#### [bluetooth](https://github.com/wendylabsinc/bluetooth)
Swift Bluetooth library for Linux, enabling BLE communication on edge devices.

#### [gstreamer](https://github.com/wendylabsinc/gstreamer)
Swift 6.2 GStreamer wrapper for robotics and computer vision applications on Jetson devices.

#### [tensorrt-swift](https://github.com/wendylabsinc/tensorrt-swift)
TensorRT Swift 6.2 bindings for Linux, enabling high-performance deep learning inference on NVIDIA hardware.

#### [deepstream-swift](https://github.com/wendylabsinc/deepstream-swift)
DeepStream Swift bindings for building intelligent video analytics applications.

### Utilities & Tools

#### [homebrew-tap](https://github.com/wendylabsinc/homebrew-tap)
Homebrew tap for easy installation of Wendy CLI on macOS:
```bash
brew tap wendylabsinc/tap
brew install wendy
```

#### [wendy-swift-tools](https://github.com/wendylabsinc/wendy-swift-tools)
Custom Swift SDK releases optimized for edge computing needs.

#### [service-protos](https://github.com/wendylabsinc/service-protos)
Shared Protocol Buffers definitions for Wendy Agent and cloud services communication.

### Specialized Libraries

#### [ffmpeg-swift](https://github.com/wendylabsinc/ffmpeg-swift)
Swift 6.2+ bindings for FFmpeg with cross-platform artifact bundle support.

#### [grayskull-swift](https://github.com/wendylabsinc/grayskull-swift)
Ergonomic cross-platform Swift wrapper library for GraySkull.

#### [pulsar-client](https://github.com/wendylabsinc/pulsar-client)
Cross-platform Swift 6.1 Pulsar client for messaging and streaming.

#### [BundleProtocolv7](https://github.com/wendylabsinc/BundleProtocolv7)
Swift implementation of the Bundle Protocol v7 for delay-tolerant networking.

#### [cbor](https://github.com/wendylabsinc/cbor)
Swift CBOR (Concise Binary Object Representation) implementation.

#### [jq](https://github.com/wendylabsinc/jq)
JQ filter library wrapper package for Swift, for JSON processing.

#### [sqlite-extension-kit](https://github.com/wendylabsinc/sqlite-extension-kit)
Swift 6.2 package for building SQLite loadable extensions with type-safe API.

### Web & Visualization

#### [react-three-map](https://github.com/wendylabsinc/react-three-map)
Use React and Three.js inside Mapbox and Maplibre for 3D geospatial visualizations.

#### [react-three-mesh-editor](https://github.com/wendylabsinc/react-three-mesh-editor)
React-based 3D mesh editing tools.

#### [office-syntax-highlighter](https://github.com/wendylabsinc/office-syntax-highlighter)
Microsoft Office Add-In for Shiki syntax highlighting in documents.

#### [opfs-checker](https://github.com/wendylabsinc/opfs-checker)
Check browser support for Origin Private File System (OPFS).

## Getting Started

### For Developers

1. **Install the Wendy CLI** (macOS):
   ```bash
   brew tap wendylabsinc/tap
   brew install wendy
   ```

2. **Set up your device** with WendyOS or install wendy-agent on a compatible Linux system

3. **Try a sample application**:
   ```bash
   git clone https://github.com/wendylabsinc/samples.git
   cd samples/swift/hello-world
   wendy run --device <your-device-hostname>
   ```

### For System Builders

1. **Build WendyOS** for NVIDIA Jetson:
   ```bash
   git clone https://github.com/wendylabsinc/meta-wendyos-jetson.git
   cd meta-wendyos-jetson
   ./bootstrap.sh
   ```

2. Follow the instructions to build and flash the image to your device

## Documentation

- **Main Documentation**: https://wendy.sh/docs/
- **Website**: https://wendyos.io

## Community & Support

- **GitHub Issues**: Use the individual repository issue trackers
- **Discussions**: [Coming soon]

## License

Most repositories are licensed under the Apache License 2.0 or MIT License. Check individual repositories for specific license information.

## Contributing

We welcome contributions! Please check individual repositories for contribution guidelines.

---

Built with ❤️ by Wendy Labs