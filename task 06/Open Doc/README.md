# NEOFETCH

Neofetch is a fast, highly customizable system information script written in Bash.
The script shows system information alongside an image, your OS logo, or any ASCII file in the terminal. 
Neofetch is designed to be highly customizable, allowing users to display only the information they need, in the format they like.

## Features:

• Supports various operating systems including Linux, macOS, BSD, Windows (via Cygwin/Windows Subsystem for Linux).

• Customizable output format.

• Supports displaying system logos, images, and ASCII art. 

• Lightweight and fast.
    
## Installation

### For Debian/Ubuntu-based distributions:

      sudo apt install neofetch
      
### For Fedora:

       sudo dnf install neofetch
       
### For Arch Linux:

       sudo pacman -S neofetch

### From source:
To install Neofetch manually:

1.Clone the repository:

      git clone https://github.com/dylanaraps/neofetch.git
      
2. Navigate to the Neofetch directory:

       cd neofetch

3. Run the install script:
       
       sudo make install
   

## Usage

Once installed, you can run Neofetch by simply typing:
    
    neofetch
    
To customize the output:

    neofetch --config <path_to_config>

Example output:

    OS: Ubuntu 20.04
    Kernel: 5.4.0-65-generic
    Shell: bash 5.0.17
    Resolution: 1920x1080
    DE: GNOME 3.36.8

## Contribution

If you want to contribute to Neofetch, follow these steps:

1.Fork the repository.

2.Create a new branch.

3.Make your changes and commit them.

4.Push to your branch.

5.Create a pull request.
