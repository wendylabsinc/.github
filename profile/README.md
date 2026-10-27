# Wendy Labs

Wendy is the full stack physical AI platform: an open-source OS, CLI, and cloud that your coding agent uses to simulate, ship, and operate robots and drones.

[Website](https://wendy.dev) · [Documentation](https://docs.wendy.dev/latest/) · [Discord](https://discord.gg/wendylabsinc)

```sh
curl -fsSL https://install.wendy.dev/cli.sh | bash
wendy tour
```

## What Wendy does

- [Simulation](https://docs.wendy.dev/latest/integrations/sim-to-real/): run WendyOS in a local VM with simulated Unitree Go2 and G1, SO-101 and ROSMASTER R2 robots, then deploy the same app to hardware.
- [Supported hardware](https://docs.wendy.dev/latest/#2-set-up-a-device): NVIDIA Jetson Orin Nano, AGX Orin and AGX Thor; Raspberry Pi 3, 4 and 5; Qualcomm Dragonwing; Arduino UNO Q; any ARM64 or x86-64 Linux computer; Apple Silicon Macs (beta).
- [Robots](https://docs.wendy.dev/latest/integrations/): install the Agent on a Unitree G1's onboard computer, and use a Unitree Go2's ROS 2 topics and front camera from your apps.
- [AI coding agents](https://docs.wendy.dev/latest/guides/llm-integration/): an MCP server and plugins for Claude Code and Codex, a hosted ChatGPT plugin, `wendy chat` in the terminal, and persistent agents that talk A2A.
- [ROS 2](https://docs.wendy.dev/latest/integrations/ros2/): standard ROS 2 in containers, `wendy device ros2` to inspect a remote robot, and a Foxglove bridge.
- [ESP32 (beta)](https://docs.wendy.dev/latest/installation/wendy-lite-esp32/): flash Wendy Lite firmware, then build and deploy native ESP-IDF apps with `wendy run`.
- [Wendy Net](https://docs.wendy.dev/latest/guides/wendy-net/): connect nearby devices over Ethernet, Wi-Fi, Bluetooth or Wi-Fi Aware so their apps can find each other.
- [SensorLink](https://docs.wendy.dev/latest/hardware/camera/#wendy-lite-cameras): view a Wendy Lite board's camera from your computer, or pair sensor sources with a device using `wendy device pair`.
- [Developer loop](https://docs.wendy.dev/latest/guides/stagefile/): Stagefile builds that upload only what changed, `wendy run --watch`, a shared remote build host, and multi-service apps.
- [Install and flashing](https://docs.wendy.dev/latest/advanced/clients/wendy-cli/commands/install/): `wendy install` flashes Jetson, Raspberry Pi, Dragonwing, Arduino UNO Q and ESP32 boards from your computer.
- [WendyOS](https://docs.wendy.dev/latest/advanced/clients/wendy-cli/commands/os/update/): a Yocto-based Linux distribution with A/B OS updates through `wendyos-update`, automatic rollback, and stable and nightly channels.
- [Cameras](https://docs.wendy.dev/latest/hardware/camera/): USB, CSI and IP (RTSP/ONVIF) cameras and ROS 2 image topics all appear to apps as `/dev/video` devices.
- [Wendy Data](https://docs.wendy.dev/latest/data/): record sensor data, app events and model results around trigger events, and retrieve them as episodes.
- [Templates and tutorials](https://docs.wendy.dev/latest/guides/tutorials/): start from `wendy init` templates in Python, TypeScript, Rust, C++, Swift and Mojo.
- [Wendy Cloud](https://docs.wendy.dev/latest/cloud/): enroll devices and reach them and their services through tunnels, without opening inbound ports.
- [Security](https://docs.wendy.dev/latest/security/): mutual TLS for provisioned devices, certificate-based enrollment, apps sandboxed by entitlements, and a published threat model.

## Start here

- [WendyOS](https://github.com/wendylabsinc/WendyOS): the `wendy` CLI, Wendy Agent, MCP server and documentation
- [WendyOS-Builder](https://github.com/wendylabsinc/WendyOS-Builder): Yocto build for WendyOS images
- [templates](https://github.com/wendylabsinc/templates): project templates for `wendy init`
- [samples](https://github.com/wendylabsinc/samples): sample applications
- [wendy-lite](https://github.com/wendylabsinc/wendy-lite): Wendy for ESP32 microcontrollers
- [wendy-agentic-coding](https://github.com/wendylabsinc/wendy-agentic-coding): plugin for Claude Code and Codex
