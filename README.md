# OpenCR Firmware Update for TurtleBot3

This repository contains firmware binaries and update tools for the **OpenCR board** used in TurtleBot3 robots (Burger, Waffle) and OpenManipulator with ROS Noetic.

## 📁 Directory Structure

### `opencr_update.tar.bz2`
Compressed archive containing the firmware update tools and binaries.

### `opencr_update/`
Extracted folder with the following contents:

| File | Purpose |
|------|---------|
| `burger_noetic.opencr` | Firmware for TurtleBot3 Burger (ROS Noetic). |
| `burger_turtlebot3_core.ino.bin` | Core firmware for Burger. |
| `waffle_turtlebot3_core.ino.bin` | Core firmware for Waffle. |
| `waffle_turtlebot3_core_noetic.ino.bin` | ROS Noetic core firmware for Waffle. |
| `open_manipulator_noetic.opencr` | Firmware for OpenManipulator (ROS Noetic). |
| `open_manipulator_turtlebot3_core_noetic.ino.bin` | Combined firmware for OpenManipulator + TurtleBot3 (Noetic). |
| `opencr_ld_shell_x86` | Firmware loader executable for x86-based Linux. |
| `update.sh` | Shell script to flash firmware to OpenCR board.

## 🚀 How to Flash Firmware

1. Connect OpenCR to your PC via USB.
2. Give execute permissions:
   ```bash
   chmod +x opencr_ld_shell_x86 update.sh
