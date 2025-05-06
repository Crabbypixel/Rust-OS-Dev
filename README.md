# Rust-OS-Dev

A simple, non-GUI based Operating System (OS) developed using **Rust**. This project aims to provide a foundational understanding of OS concepts, with a focus on low-level system development.

## Overview

This project is an attempt to build an operating system from scratch using the **Rust programming language**, which offers memory safety and concurrency features that are crucial in OS development. The current implementation is a simple kernel that interacts directly with the hardware and provides basic functionalities. As development progresses, new features like CPU exceptions, double faults, paging, heap allocation, and more will be added.

## Features

- **Kernel Development**: Writing a basic kernel in Rust with minimal dependencies.
- **Non-GUI**: Focus on the core functionalities of an OS without graphical user interface (GUI) support.
- **Memory Management**: Basic implementation of memory allocation (to be extended in future versions).
- **Hardware Interaction**: Direct communication with hardware components (such as the CPU) for low-level operations.
  
## Currently In Progress

- CPU exceptions
- Double fault handling
- Paging (virtual memory)
- Heap allocation
- Improved memory management

## Future Goals

- Implement system calls
- Basic file system support
- Process management (multitasking)
- Interrupt handling
- GUI interface (possibly in the long term)

## Prerequisites

- **Rust**: You need to have Rust installed on your system. Install it from [Rust's official website](https://www.rust-lang.org/tools/install).
- **QEMU** (for emulation): This project can be tested using an emulator like QEMU. Install it from [QEMU's website](https://www.qemu.org/download/).
- **Bootloader**: GRUB (or a similar bootloader) is needed for bootstrapping the kernel.
- **x86_64 System**: The OS is currently targeting x86_64 architecture.

## Setup

1. **Clone the repository**:
    ```bash
    git clone https://github.com/Crabbypixel/Rust-OS-Dev.git
    cd Rust-OS-Dev
    ```

2. **Install dependencies**:
    Follow the installation steps for Rust, QEMU, and any other dependencies you might need as per your OS distribution.

3. **Build the project**:
    ```bash
    cargo build
    ```

4. **Run the OS on QEMU**:
    To run the OS in an emulated environment, use the following command:
    ```bash
    cargo run
    ```

    This will start the OS on QEMU and you can test its basic functionality.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests for bugs, improvements, or new features.

### Steps for contributing:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Make your changes and commit (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a pull request.

## License

This project is open-source and available under the [MIT License](LICENSE).

## Acknowledgements

- Special thanks to [The Rust Programming Language](https://www.rust-lang.org/) for providing an excellent system programming language.
- [OSDev Wiki](https://os.phil-opp.com/) for offering great resources on OS development.
- [QEMU](https://www.qemu.org/) for providing an excellent tool for hardware emulation.

## Disclaimer

This is a learning project and should not be considered for production use. It’s intended to explore operating system development concepts in Rust.

