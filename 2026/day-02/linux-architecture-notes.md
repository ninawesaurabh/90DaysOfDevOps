# The core components of Linux (kernel, user space, init/systemd)
# Kernel
* A kernel is the core part of an operating system. It acts as a bridge between software applications and the hardware of a computer.
* The kernel manages system resources, such as the CPU, memory and devices, ensuring everything works together smoothly and efficiently.
* It handles tasks like running programs, accessing files and connecting to devices like printers and keyboards.
* An Operating System includes the kernel as its core, but also provides a user interface, file system management, network services and various utility applications that allow users to interact with the systemapplications that allow users to interact with the system.
* Facilitates communication between hardware and user applications.
* Ensures efficient and secure multitasking.
* Manages system stability and prevents unauthorized resource access.

# User space
User space is the memory area and execution context where all user applications, system libraries, and utilities run with limited privileges. It is a protected environment separated from the core operating system, known as kernel space, to ensure system stability and security.

# init/systemd
init is the traditional name for the first process started by the kernel (PID 1), which is responsible for initializing the rest of the system. In most modern Linux distributions, the init program is a symbolic link to the systemd executable, which acts as the system and service manager.

# How processes are created and managed
The Linux kernel manages processes by tracking their state, priority, and resources. Users and system administrators interact with these processes using various command-line tools:

# Process States
Processes transition through several states during their lifecycle: 
* Running (R): The process is either currently executing on the CPU or is ready to run.
* Sleeping (S): The process is waiting for an event (e.g., I/O completion, a signal).
* Stopped (T): The process has been paused, usually by a job control signal.
* Zombie (Z): The process has terminated, but its entry still remains in the process table until the parent process collects its exit status via wait().

# What systemd does and why it matters
Systemd is a system and service manager for Linux operating systems that acts as the initialization (init) system to bootstrap user space and manage processes, typically running as the first process (PID 1). It is the default in almost all modern Linux distributions

# Why it matters in Linux:
* Faster Boot Times: By starting services in parallel, systemd significantly reduces the time it takes for a system to become usable.
* Standardization: It provides a unified, consistent way to manage services, networking, and system configurations across different Linux distributions.
* Improved Stability & Monitoring: If a service crashes, systemd can automatically restart it. It also prevents "ghost" processes by tracking them via cgroups.
* Better Troubleshooting: The centralized journalctl tool allows administrators to filter logs by time, service, or priority, making it easier to diagnose system issues.
* Easy Configuration: It uses declarative unit files (simple text files) to define how services should run, replacing complex shell scripts.

# Common Linux commands:
* ls: Lists the contents of a directory, including files and subdirectories.
Example: ls -l shows a detailed, long-format list of contents.
* cd: Stands for "change directory" and is used to navigate the file system.
Example: cd /home/username changes to a specific absolute path, while cd .. moves one directory up.
* pwd: Stands for "print working directory" and displays the full path of your current location in the file system.
Example: pwd might output /home/user/Documents.
* mkdir: Creates a new directory (folder) in the specified location.
Example: mkdir new_projects creates a directory named "new_projects" in the current location.
* cat: Short for "concatenate," this command reads the contents of a file and displays them on the terminal screen, which is useful for quickly viewing small files.