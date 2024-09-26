---
layout: default
title: Installation
description: "Getting Started"
parent: CaaS for OctoPrint
nav_order: 2
---
# Getting Started
---

## OctoPi Installation (Recommended)


First, you need to install the OctoPrint image on your Raspberry Pi. Follow these steps:

1. **Download Raspberry Pi Imager**: Go to the [official Raspberry Pi website](https://www.raspberrypi.org/software/) and download the Raspberry Pi Imager.
   
2. **Flash the OctoPrint Image**: Use Raspberry Pi Imager to select the **OctoPi** image (which includes OctoPrint pre-installed) from the operating system list and write it to your microSD card.

3. **Configure Advanced Settings**: Before flashing the image, press `Ctrl + Shift + X` (or `Cmd + Shift + X` on macOS) to open the advanced settings menu. Here you can:
    - **Enable SSH**: Check the box to enable SSH.
    - **Set Username and Password**: Set the desired default username and password for your Raspberry Pi.

4. **Insert the microSD Card**: After the image is flashed, insert the microSD card into your Raspberry Pi and power it on.

Your Raspberry Pi should now boot up with OctoPi (which includes OctoPrint), and you should be able to SSH into it using the credentials you set in the Raspberry Pi Imager.

### Install the Ulendo CaaS Plugin

The [Ulendo-CaaS] plugin can be installed directly from the OctoPrint Plugin Repository. Follow these steps:

1. Open the **OctoPrint Web Interface** by navigating to `http://<your-raspberry-pi-ip>/` in your browser.
   
2. Go to **Settings** -> **Plugin Manager** -> **Get More**.

3. Search for **Ulendo CaaS**, and install it directly from the plugin repository.
---

## Manual Installation

### Step 1: Install Raspberry Pi OS

First, you need to install the Raspberry Pi OS on your Raspberry Pi. Follow these steps:

1. **Download Raspberry Pi Imager**: Go to the [official Raspberry Pi website](https://www.raspberrypi.org/software/) and download the Raspberry Pi Imager.
   
2. **Flash the Image**: Use Raspberry Pi Imager to select the Raspberry Pi OS 64-bit Lite image and write it to your microSD card.

3. **Configure Advanced Settings**: Before flashing the image, press `Ctrl + Shift + X` or `Cmd + Shift + X` to open the advanced settings menu. Here you can:
    - **Enable SSH**: Check the box to enable SSH.
    - **Set Username and Password**: Set the desired default username and password for your Raspberry Pi.

4. **Insert the microSD Card**: After the image is flashed, insert the microSD card into your Raspberry Pi and power it on.

Your Raspberry Pi should now boot up with Raspberry Pi OS 64-bit Lite, and you should be able to SSH into it using the credentials you set in the Raspberry Pi Imager.


### Step 2: Install Octoprint and the CaaS plugin

Once you've logged into the Raspberry Pi via SSH and the device has booted up, follow these steps to install OctoPrint and the CaaS plugin:

Run the following commands to download and execute the installation script:
   ```bash
   cd ~
   curl https://raw.githubusercontent.com/S2AUlendo/UlendoCaaS/main/UlendoCaas-Install.sh > UlendoCaaS-Install.sh
   sudo chmod +x UlendoCaaS-Install.sh
   . ./UlendoCaaS-Install.sh
   ```
Once the installation is complete, OctoPrint and the CaaS plugin should be up and running on your Raspberry Pi. You are all set!


[Ulendo-CaaS]: https://just-the-docs.github.io/just-the-docs/
[Ulendo-CaaS Github]: https://github.com/S2AUlendo/UlendoCaaS