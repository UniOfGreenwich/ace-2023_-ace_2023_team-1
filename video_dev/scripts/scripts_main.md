### 2- System Design and Architecture

* Design and architecture  
To develop the system’s design and architecture, we had to work with components provided by the university. We were provided with 10 ASUS CS-8 motherboards, 10 SD cards, multiple 220W PSUs and a 5-port switch.

To meet the modular criteria of the project, a single module consists of four nodes, three containing a motherboard with its corresponding PSU, and the fourth node being the head node which holds the single board computer and the switch. Consider Figure 1.

Due to the switch having 5 ethernet ports, 3 ports are taken by the motherboards; one port is taken by the single board computer, leaving an extra ethernet port to allow the entire HPC module to be connected to another copy of the HPC module in a daisy chain configuration. This daisy chain can be extended to multiple copies of the HPC. Consider Figure 2.

* NixOS why, what tried what failed  
NixOS was initially selected as the operating system due to its reproducible and declarative nature. Using Rufus, the system was loaded onto a bootable SD card. During the installation of various packages, an error occurred with the Samba package — a critical component for network communication — because an incompatible version was downloaded for the system's architecture. Attempts to resolve this included rolling back the system, which did not give the desired results, and cleaning dependencies, but this step inadvertently removed essential components, halting system progress. The group had to consider either transitioning to a new OS or reinstalling NixOS. A comparative analysis of NixOS, Ubuntu, and Arch Linux was conducted to inform the decision.

* OS Comparisons  
Given the limited progress made and NixOS's complexity, the decision was made to switch to an alternative operating system, with Ubuntu being the selected replacement. This choice was influenced by Ubuntu's user-friendly nature, making it a practical option for those new to Linux, as well as its broad accessibility. It has efficient package management via APT and DEB systems and offers stable releases with extended support. Additionally, its substantial documentation and supportive community simplify troubleshooting. Ubuntu also emphasises security in system integration and has a wide repository containing over 60,000 packages, further validating its selection.

### 25- Future Work

* SingularityCE  
Another next step that could be taken would be to implement Singularity. Singularity is a container platform designed for high-performance computing (HPC), scientific computing, and data-intensive tasks. It allows users to create portable, reproducible computing environments by encapsulating software, libraries and data in a single package. Singularity provides security by allowing containers to run without granting users elevated privileges primarily because it runs containers with the privileges of the user who launches them rather than requiring root or administrative privileges. It supports integration with existing HPC resources and workflows, such as Slurm, offering compatibility with various container formats, such as Docker, through conversion tools.