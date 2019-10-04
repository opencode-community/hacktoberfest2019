# Linux kernel

![Linux](https://www.kernel.org/theme/images/logos/favicon.png)

#### History
#### The Linux kernel was conceived and created in 1991 by [Linus Torvalds](https://en.wikipedia.org/wiki/Linus_Torvalds) for his personal computer and with no cross-platform intentions, but has since expanded to support a huge array of computer architectures, many more than other operating systems or kernels. Linux rapidly attracted developers and users who adopted it as the kernel for other free software projects, notably the GNU Operating System, which was created as a free, non-proprietary operating system, and based on UNIX as a by-product of the fallout of the Unix wars.
#### The Linux® kernel is the main component of a Linux operating system (OS) and is the core interface between a computer’s hardware and its processes. It communicates between the two, managing resources as efficiently as possible.

#### The kernel is so named because—like a seed inside a hard shell—it exists within the OS and controls all the major functions of the hardware, whether it’s a phone, laptop, server, or any other kind of computer.

# What the kernel does
#### The kernel has 4 jobs:

- #### Memory management: Keep track of how much memory is used to store what, and where
- #### Process management: Determine which processes can use the CPU, when, and for how long
- #### Device drivers: Act as mediator/interpreter between the hardware and processes
- #### System calls and security: Receive requests for service from the processes

# Where the kernel fits within the OS
#### To put the kernel in context, you can think of a Linux machine as having 3 layers:

- #### The hardware: The physical machine--the bottom or base of the system, made up of memory (RAM) and the processor or central processing unit (CPU), as well as I/O devices such as storage, networking, and graphics. The CPU performs computations and reads from, and writes to, memory.
- #### The Linux kernel: The core of the operating system (See? It’s right in the middle). It’s  software residing in memory that tells the CPU what to do.
- #### The processes (aka "user processes"): These are the running programs that the kernel manages. Processes are what collectively make up user space and are also known as user processes, regardless of whether or not a user interacts with them directly. For example, web servers run as user processes. Something else interesting to note is that the kernel also allows these processes/servers to communicate with each other (known as inter-process communication, or IPC).

#### Code executed by the system runs on CPUs in 1 of 2 modes: kernel mode or user mode. Code running in the kernel mode has unrestricted access to the hardware, while user mode restricts access to the CPU and memory to the system call interfaces. As briefly mentioned earlier, a similar separation exists for memory (kernel space and user space). These two small details form the base for some complicated operations like privilege separation for security to building containers and virtual machines.

#### This also means that if a process fails in user mode, the damage is limited and can be recoverable by the kernel. However, because of its access to memory and the processor, a kernel process crash can crash the entire system. Since there are safeguards in place and permissions required to cross boundaries, user process crashes can’t cause too many problems. That’s the idea, anyway.

&nbsp;

![Architecture](https://www.researchgate.net/profile/Daniel_Aarno/publication/230995988/figure/fig3/AS:669418908569620@1536613313780/Architecture-of-the-standard-Linux-kernel.png)
#### Architecture of the standard Linux kernel

### Refrerence links

| Reference | Link |
| ------ | ------ |
| Developer | [Linus Torvalds ](https://en.wikipedia.org/wiki/Linus_Torvalds) |
| GitHub | [linux.git](https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git) |
| Written in | C and assembly |
| OS family | Unix-like |
