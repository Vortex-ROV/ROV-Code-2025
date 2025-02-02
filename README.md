# Vortex ROV Code Repository 2025

Welcome to the **2025** repository for the Vortex ROV software! This README will guide you through the prerequisites, file structure, and key functionalities of the ROV's software—specifically **ROV control** and **streaming OAK-D video/depth frames for measurements** during mission tasks.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Repository Structure](#repository-structure)

## Introduction

The Vortex ROV software (2025 version) is responsible for managing the ROV's onboard systems, including:
- **Navigation & Control:** Precise control of thrusters and movement.
- **Video Streaming:** Real-time streaming from an OAK-D camera for situational awareness.
- **Depth Sensing & Measurements:** Streaming depth frames from the OAK-D camera to support accurate measurements during mission tasks.

These capabilities ensure that the ROV effectively supports mission objectives, allowing operators to visualize underwater environments and gather critical data for inspection, sample collection, and other competition-related or research tasks.

## Installation

To set up the ROV software on your development environment, follow these steps:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Vortex-ROV/ROV-Code.git
   cd ROV-Code
   ```

2. **Create and Activate a Virtual Environment:**

   It's a good practice to use a virtual environment to manage dependencies. Run the following commands to create and activate one:

   - On macOS/Linux:
     ```bash
     python3 -m venv venv
     source venv/bin/activate
     ```

   - On Windows:
     ```bash
     python -m venv venv
     venv\Scripts\activate
     ```
     
3. **Install Packaged Dependencies:**
   ```bash
   pip install .
   ```

4. **Run the ROV Software:**
   ```bash
   python main.py
   ```

## Repository Structure

- **`/src`:** Core source code for navigation, control, and sensor data processing (including OAK-D video and depth handling).
- **`/tests`:** Test cases to validate the software's functionality and performance.
- **`main.py`:** Main script used to launch the ROV software.
- **`ROV.toml`:** Configuration file for packaging the ROV code.
