## StrixOS

StrixOS is a minimal, custom operating system designed from scratch. It's built with low-level programming in mind, using assembly language and C to create a lightweight and efficient OS. StrixOS is aimed at developers and hobbyists who want to explore operating system concepts, low-level hardware interaction, and bootloader design. The system is designed to run on a virtual machine (QEMU) but can also be adapted for physical hardware.

### Features
- **Custom Bootloader**: A simple bootloader written in assembly that loads the kernel into memory and starts the OS.
- **Minimal Kernel**: A basic kernel written in assembly and C to handle basic input/output and system functions.
- **Filesystem Support**: Basic file system operations for handling files within the OS environment.
- **Hardware Abstraction**: Interaction with hardware components such as keyboard, screen, and storage devices through direct hardware access.
- **Command Line Interface (CLI)**: A simple and interactive command line for user input and system control.

### Technologies Used
- **Assembly Language**: For the bootloader and other low-level components.
- **C Programming**: For the kernel and other system utilities.
- **QEMU**: For running StrixOS in a virtual machine.
- **Makefile**: To manage the build process and automate the compilation.

### Getting Started

To get started with StrixOS, clone the repository and build the OS using the following steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yucchannel/strix.git
   cd strix
   ```

2. Build the bootloader and kernel:
   ```bash
   cd bootloader
   make
   cd ../kernel
   make
   ```

3. Combine the bootloader and kernel into an OS image:
   ```bash
   cat boot.bin kernel.bin > strix.img
   ```

4. Run the OS using QEMU:
   ```bash
   qemu-system-i386 -drive file=strix.img,format=raw
   ```

### Contributing

Feel free to contribute to the development of StrixOS by submitting issues or pull requests. We welcome contributions from developers, hobbyists, and anyone interested in low-level programming and operating system development.

### License

StrixOS is released under the MIT License. See the [LICENSE](LICENSE) file for more information.

### about this character > ~(___('U')

This character is a snake named SHELL.

---

This description gives an overview of the StrixOS project, including its purpose, features, technologies, and instructions for getting started. If you want to use it on your GitHub repository, just replace the placeholder with your actual repository link and adjust any details specific to your project.
