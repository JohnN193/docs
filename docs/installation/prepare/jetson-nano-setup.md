---
title: "NVIDIA Jetson Nano Setup Guide"
linkTitle: "Jetson Nano Setup"
weight: 20
type: "docs"
draft: false
description: "Set up the Jetson Nano Developer Kit to prepare your NVIDIA Jetson Nano for viam-server installation."
# SMEs: Pete Garafano
---

The [Jetson Nano](https://developer.nvidia.com/embedded/jetson-nano) from [NVIDIA](https://www.nvidia.com/) is a small computer that is built for embedded applications and is capable of supporting modern AI workloads.
Follow this guide to set up the [Jetson Nano Developer Kit](https://developer.nvidia.com/embedded/jetson-nano-developer-kit) to prepare your NVIDIA Jetson Nano for `viam-server` installation.

<p style="margin:auto; max-width:500px;"><img src="../../img/jetson-nano-setup/jetson-nano-dev-kit.png" alt="The front of the NVIDIA Jetson Nano single-board computer development kit." ></p>

{{< alert title="Note" color="note" >}}

This board is experimental. Stability is not guaranteed.
This guide assumes that you have a Jetson Nano Developer Kit with a Jetson module and reference carrier board, but you may want to use a different carrier board to incorporate your Nano into your robot.
If so, the type of carrier board you use will affect your hardware requirements.

{{% /alert %}}

## Hardware Requirements

You need the following hardware, tools, and software to install `viam-server` on a Jetson Nano:

**Initial Setup with Display Attached:**

1. A [Jetson Nano Developer Kit](https://developer.nvidia.com/embedded/jetson-nano-developer-kit)
2. A microSD card (32GB UHS-1 minimum recommended)
3. A computer display (HDMI or DP) with USB keyboard and mouse
4. A way to connect the microSD card to the computer (like a microSD slot or microSD reader)
5. Ethernet cable and/or Wifi dongle, to establish network connection on the Nano
6. 5V-2A DC with barrel jack connector and/or Micro-USB power supply, to power the Nano

**Initial Setup in Headless Mode:**

1. A [Jetson Nano Developer Kit](https://developer.nvidia.com/embedded/jetson-nano-developer-kit)
2. A microSD card (32GB UHS-1 minimum recommended)
3. An internet-connected computer
4. A way to connect the computer to the Nano (like a USB 2.0 A-Male to Micro B Cable)
5. A way to connect the microSD card to the computer (like a microSD slot or microSD reader)
6. Ethernet cable and/or Wifi dongle, to establish network connection on the Nano
7. 5V-2A DC with barrel jack connector power supply, to power the Nano (Micro-USB port will be taken by the cable connection to computer)

## Jetson Nano Setup Guide

1. Follow the instructions in [Getting Started with Jetson Nano Developer Kit](https://developer.nvidia.com/embedded/learn/get-started-jetson-nano-devkit).
Once you have reached *Next Steps*, return to the Viam docs.
1. Your Jetson Nano now has a Viam-compatible operating system installed.
    Continue to our [viam-server installation guide](/installation/install/).
    Note that the Jetson Nano has aarch64 CPU architecture.

{{< alert title="Tip" color="tip" >}}

If you have issues installing or using `curl` on your Nano, try using `wget http://packages.viam.com/apps/viam-server/viam-server-latest-aarch64.AppImage` to download the `viam-server` binary.

{{% /alert %}}

## Troubleshooting

You can find additional assistance in the [Troubleshooting section](/appendix/troubleshooting/).

You can also ask questions on the [Viam Community Slack](https://join.slack.com/t/viamrobotics/shared_invite/zt-1f5xf1qk5-TECJc1MIY1MW0d6ZCg~Wnw) and we will be happy to help.