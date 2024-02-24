# <u> **OS PACKAGES DESCRIPTION** </u>

## 1. <u> Packages in use </u>

* <u> Vim: </u>
Vim stands for "Vi IMproved" and is a free, open-source text editing program made available for UNIX-like systems in 1991. It can be used in plain text mode or with a visual interface and works on all types of computers and devices. Learning to use Vim is relatively easy, but it requires constant practice. It is celebrated for its speed, efficiency, and power, partly due to its compact size that allows it to run directly in a command window (although it also has a graphical version). One of the main reasons for its efficiency is that it can be used without drop-down menus or a mouse, using only keyboard shortcuts, such as pressing "d" to delete text, "c" to change it, "f" to search for something and so on. Street. Combining these shortcuts with numbers allows one to do the same thing multiple times. Also, doubling a command, like "yy", can do something across the entire page.
Vim doesn't take up much space in a computer's memory, making it expandable. There are various plugins to extend the functionalities. The best way to configure it is through the .vimrc file, which can be opened and configured using Vim.

* <u> Wget: </u>
Wget is a software program developed by the GNU Project that allows users to download content and files from different internet servers. Its name stands for World Wide Web and "get," indicating its function to fetch and download data through several protocols, including FTP, SFTP, HTTP, and HTTPS.
This utility is written in portable C programming language, so runable on any Unix-based system. It's also adaptable to other widely used operating systems like Mac OS X, Microsoft Windows, and AmigaOS, among others.

* <u> Git: </u>
It is a widely used, open-source, free-distributed version control system (VCS) that focuses on the content within files instead of the file's attributes. It ensures security through SHA-256 encryption and maintains a comprehensive log of information, making it ideal for efficiently managing projects of any size. Designed for software development, Git monitors modifications in source code, emphasising quick performance, the integrity of data, and collaborative support. This allows several developers to contribute to the development process in a non-linear fashion simultaneously.

* <u> DNSMASQ: </u>
Dnsmasq is a compact tool that helps manage small network setups by providing DNS, DHCP, and network boot services. It's designed to use minimal resources, making it ideal for routers and firewalls with limited capacity. Dnsmasq is compatible with various operating systems, including Linux, Android, *BSD, and Mac OS X, and comes pre-installed on many Linux distributions. Its features include local DNS caching and forwarding, secure DNS query validation through DNSSEC, and comprehensive DHCP support for both IPv4 and IPv6, including network booting capabilities. Additionally, Dnsmasq can serve as an authoritative DNS server, automatically integrate DHCP lease information into DNS, and support router advertisements for IPv6 configurations. It's highly configurable, allowing unused features to be excluded to minimize its system footprint further.

* <u> Syslinux: </u>
Syslinux is a boot loader designed for the Linux operating system, specifically for use with the MS-DOS/Windows FAT filesystem. Its primary purpose is simplifying the initial Linux installation process and help create boot disks for rescue and other specific uses. When a computer starts, Syslinux loads the Linux kernel from a default LINUX image file on the boot disk. The key feature of Syslinux is its flexibility; it doesn't require preknowledge of the kernel files as long as they are in the disk's root directory. Syslinux also supports using initial ramdisks (initrd) and the bzImage kernel format, enhancing its utility for various booting scenarios.

* <u> Pxelinux: </u>
A PXE install server is a special setup that lets other computers in your network start up (boot) and install a Linux operating system directly over the network. This means you don't need to use CDs, DVDs, or floppy disks to get the Linux installation files onto each computer.

## 2. <u> Packages considered but not in use </u>

* <u> Pxecore: </u>

* <u> Calc: </u>

* <u> Openssh: </u>
It is the open-source version of the SSH (Secure Shell) protocol. It is mainly utilised for securely managing systems, transferring files, and facilitating communication across the internet or other unsecured networks. It secures user passwords, identities, and all transmitted data through encryption, safeguarding against unauthorised interception and theft.

* <u> Gcc: </u>
The GNU Compiler Collection (GCC) is a free, open-source compiling and development tool available on multiple operating systems, including Linux and Windows. It supports a wide range of programming languages, especially C and C++.
Being a versatile toolchain, it processes code from compilation to generation of executable files. Preprocess, compile, assemble and link code, integrating external libraries to produce executables. Used primarily in the Linux ecosystem, it is an integral part of compiling most software, including the Linux kernel. GCC's GPL version 3 license grants broad software freedoms bolstered by a strong support network of a large community of developers and contributors. Its modular design improves maintainability, facilitates debugging, and makes it easy to add new features.

* <u> Bat: </u>
Bat, or "a cat clone with wings", has similar functionality to cat, awk, more and sed, i.e. concatenating files together, but more visually appealing with more extra context and colourful results. To quickly preview the contents of a text file without opening it in an extensive application, often concatenate one file to nothing. The command is Git-compatible by default. In a Git repository with the --diff command, it is possible to display only changes from the latest commit. It also allows highlighting a series of lines in a file, not the syntax, but marks each line with a filled box.

* <u> Feh: </u>

* <u> Lsd: </u>

* <u> Nixpkgs-fat: </u>

* <u> Nix-output-nonltor: </u>

* <u> Nix-prefetch-github: </u>

# Updates

Initially, the NixOS operating system was considered and downloaded onto the laptop of one of the group members. Subsequently, Rufus was used to convert it into a bootable SD card. The card was then inserted into a Raspberry Pi 4 SBC, and it was booted. The network configuration has been started and, since it is a declarative system, some packages have been downloaded including: vim, lwd, git, openssh, gcc, bat, calc, bc, dox2unix, feh, file, lsd, nixpkgs-fat, nix-output-nonltor, nix-prefetch-github.
During the installation of samba, to ensure communication and collaboration between the network, an error occurred: "a 'x86_64-linux' with features {} is required to build '/nix/store/58fz02g4p6f3y177nwfkwyqmzzmcm1r0-builder.pl .drv', but I am a 'aarch64-linux' with features {benchmark, big-parallel, gccarch-armv8-a, kvm, nixos-test}". Two approaches were attempted to try to resolve the generated error. We tried to roll back the system a few generations back, but since this didn't work and the error was not resolved, it was considered to clean the system of some dependencies. Unfortunately, some of the dependencies that were eliminated were still needed, so at that point, the group had to decide what to do next. Considering the progress achieved so far, the time remaining, and the difficulty of the operating system, it was decided to use a different one. The systems considered were two imperatives: Debian and Ubuntu; the final choice fell on the Debian derivative system, Ubuntu.
UBUNTU 20.04.6 LTS (focal) was chosen as it has long-term support and supports PXE. The image and the installer were downloaded and deployed in the Raspberry Pi 4 SBC, and the network was configured.
Since it is necessary to create a computer cluster, it was necessary to create a remote directory with all the operating system information accessible to other devices to retrieve information for system deployment.

# References
- [Vim: What is it and Why to use it?](https://www.loginradius.com/blog/engineering/vim-getting-started/) [Accessed: 17/02/2024];
- [What Is the Wget Command and How to Use It (12 Examples Included)](https://www.hostinger.com/tutorials/wget-command-examples/) [Accessed: 17/02/2024];
- [Version Control Systems](https://teachingmaterial.github.io/ELEE1149-Lectures/content/VersionControlSystems/versionControlSystem.html) [Accessed: 17/02/2024];
- [What is OpenSSH?](https://www.ssh.com/academy/ssh/openssh#what-is-openssh?) [Accessed: 17/02/2024];
- [GCC](https://www.incredibuild.com/integrations/gcc#:~:text=What%20is%20GCC%3F-,The%20GNU%20Compiler%20Collection%2C%20commonly%20known%20as%20GCC%2C%20is%20a,Go%2C%20Fortran%2C%20and%20D.) [Accessed: 17/02/2024];
- [Drop the Linux cat command for bat](https://www.redhat.com/sysadmin/linux-bat-command#:~:text=Bat%2C%20known%20as%20%22a%20cat,on%20Linux%20concatenates%20files%20together.) [Accessed: 17/02/2024];
- [Dnsmasq](https://thekelleys.org.uk/dnsmasq/doc.html) [Accessed: 24/02/2024];
- [focal (1) syslinux.1.gz](https://manpages.ubuntu.com/manpages/focal/man1/syslinux.1.html#description) [Accessed: 24/02/2024];
- [PXEInstallMultiDistro](https://help.ubuntu.com/community/PXEInstallMultiDistro#:~:text=A%20PXE%20install%20server%20allows,%2C%20boot%20floppy%20images%2C%20etc.) [Accessed: 24/02/2024];