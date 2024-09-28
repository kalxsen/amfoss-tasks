# Neofetch Documentation

## Overview

Neofetch is a command-line tool written in Bash that displays information about your system next to your operating system's logo. The tool is often used for showing off desktop configurations and making system information aesthetically pleasing.

## Features:

Information Displayed:
* OS
* Kernel version
* Shell
* Resolution
* Desktop Environment (DE) and Window Manager (WM)
* Theme and Icons
* Uptime, memory, CPU, and more.

* Customization:
Neofetch allows users to control exactly what information is displayed and how it is formatted. Users can define what should be displayed in a configuration file (`config.conf`), making it highly adaptable to any setup.

* Supported Platforms: Neofetch works on Linux, macOS, Windows (via WSL or Cygwin), BSD, Solaris, Android (via Termux), and many other platforms.

## Code Overview:

The main functionality of Neofetch is divided into several modules that handle different types of system information:

* Main Script (neofetch): This is the entry point for running the program. It initializes and manages the flow of the script by calling the appropriate functions for gathering system information.

* Functions (functions/): This directory contains the different functions that collect information about the system. Each function corresponds to a specific category like get_kernel, get_os, get_resolution, etc.
        os.sh: Handles detection and printing of the operating system name and version.
        kernel.sh: Retrieves the current kernel version of the system.
        shell.sh: Gets the user's shell and version.
        resolution.sh: Finds and prints the current screen resolution.

Key Functions:

* print_info(): This function is responsible for collecting all system information and formatting it for display.
* get_logo(): This retrieves and formats the ASCII logo that corresponds to the detected OS.
*   detect_os(): This function detects the operating system, its version, and outputs them to the terminal.
* get_uptime(): Retrieves and displays system uptime.

These functions use tools like `uname`, `lsb_release`, `xdpyinfo`, and other standard utilities to gather system information. Each function outputs data in a readable and aesthetic format.

## Usage Examples:

To run Neofetch with a custom configuration file:

    neofetch --config /path/to/custom_config.conf
   
To suppress certain fields (e.g., CPU or RAM):

    neofetch --disable cpu ram
