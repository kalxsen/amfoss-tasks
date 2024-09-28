# Neofetch Directory Structure

The directory structure of Neofetch is quite simple and includes the following main components:
```
neofetch/
├── ascii/                   
│   ├── linux.txt
│   ├── macos.txt
│   └── windows.txt
├── functions/               
│   ├── os.sh
│   ├── kernel.sh
│   ├── shell.sh
│   ├── resolution.sh
│   └── ...
├── configs/                 
│   └── config.conf
├── neofetch                 
├── Makefile                 
└── README.md
```
## Explanation:

* __ascii/__: This folder stores the ASCII art logos that Neofetch displays. Each file corresponds to a different OS or platform.
  
* __functions/__: This is where all the major functionality for system detection is located. Each file is dedicated to collecting a specific type of system information (e.g., OS, resolution, kernel).
  
* __configs/__: This contains user-customizable configuration files. These config files allow users to define what information they want to display and in what format.
  
* __neofetch__: This is the main script that is executed when running Neofetch in the terminal.
  
* __Makefile__: The Makefile is used to install Neofetch from source.                  
