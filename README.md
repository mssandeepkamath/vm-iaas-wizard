# VM-IaaS-Wizard

⚠️ **Please Note: Not yet started working on this project.**

VM-IaaS-Wizard is a versatile Infrastructure as a Service (IaaS) platform, built using Go (Golang), designed to empower users to create, manage, and interact with virtual machines across different platforms. This platform provides a command-line interface (CLI) for streamlined virtual machine management.

## Table of Contents

- [Overview](#overview)
- [Architecture](#architecture)
- [Key Features](#key-features)
- [Contributing](#contributing)
- [Future Enhancements](#future-enhancements)
- [License](#license)
- [Contact](#contact)

## Overview

VM-IaaS-Wizard is a versatile IaaS solution, written in Go, that caters to virtual machine management across a wide range of platforms. It offers a user-friendly CLI client that connects to a back-end server, allowing users to interact with virtual machines seamlessly.

- **Flexibility**: Designed in Go to work with various virtualization technologies and platforms.
- **Simplicity**: Provides an intuitive CLI, built with Go, for virtual machine management.

## Architecture

![Untitled-2023-09-17-1208](https://github.com/mssandeepkamath/vm-iaas-wizard/assets/90695071/9c6212b8-6d1a-41c0-8fa9-99ef23037136)

- The "CLI Client" represents the command-line interface that users interact with to manage virtual machines.

- The "Backend Server (Gorilla Mux)" is the server component that handles incoming requests from the CLI and communicates with the Type-2 Hypervisor.

- The "Type-2 Hypervisor (e.g., QEMU)" is responsible for creating, managing, and executing virtual machines.

## Key Features

### 1. CLI Client

The heart of VM-IaaS-Wizard is its powerful CLI client, built with Go, which simplifies virtual machine management, making it accessible to both novice and experienced users. With the CLI, you can:

- Create new virtual machines with custom specifications.
- Start and stop existing virtual machines with ease.
- Delete virtual machines that are no longer needed.
- Import, export, and manage virtual machine disk images.
- Configure basic networking for communication between virtual machines and the host system.
- Receive informative error messages that guide you through potential issues for a smooth experience.

The command-line interface (CLI) of VM-IaaS-Wizard is developed using [Cobra](https://github.com/spf13/cobra), a popular library for building command-line applications in Go. Cobra provides a robust framework for creating intuitive and feature-rich CLI commands, making it easier for users to interact with virtual machines.

### 2. Backend Server

The CLI client communicates with a robust back-end server, developed in Go, that handles the heavy lifting of managing virtual machines. The back-end server:

- Integrates seamlessly with various hypervisors, allowing users to manage virtual machines across different platforms.
- Implements an API for communication with the CLI client, enabling easy scripting and automation.
- Provides a secure and reliable environment for virtual machine operations.

The backend server of Minimal-IaaS-Manager is built using [Gorilla Mux](https://github.com/gorilla/mux), a powerful router and dispatcher for building RESTful APIs in Go. Gorilla Mux enhances the capabilities of our backend, enabling seamless communication between the CLI client and the server.

### 3. Type-2 Hypervisor Integration

VM-IaaS-Wizard leverages a Type-2 hypervisor, specifically QEMU, to efficiently execute virtual machines. Hypervisor:

- QEMU supports a wide range of host and guest operating systems, making it suitable for diverse virtualization scenarios.
- QEMU allows users to take snapshots of virtual machine states and create backups, enhancing data safety and management.

VM-IaaS-Wizard leverages a Type-2 hypervisor, specifically [QEMU](https://www.qemu.org/), to efficiently execute virtual machines. QEMU is a powerful open-source emulator and virtualization tool known for its platform compatibility, performance, snapshot capabilities, and versatility.

## Contributing

1. **Fork** the repository.
2. **Clone** your fork locally.
3. **Make changes** and commit.
4. **Push** your changes to your fork.
5. **Open a pull request** with clear details.

Please follow Go's style guide, write clear code and comments, and test your changes.

## Future Enhancements

The project's roadmap outlines upcoming milestones and enhancements:

- **Enhanced Networking**: Implement advanced networking configurations.
- **User Authentication**: Add authentication and authorization for secure access.
- **Security Improvements**: Strengthen security by securing API endpoints.


## License

This Go-based project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

Contact me through [Email](msandeepcip@gmail.com)
