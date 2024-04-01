[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/vcAhwuzK)
# Design & Development of a Modular High-Performance Computer (HPC)
## ELEE1119 Advantage Computer Engineering 2023/24
![Front Case](/ace-2023_-ace_2023_team-1/CaseFront.jpeg) ![Back Case](/ace-2023_-ace_2023_team-1/CaseBack.jpeg)

## Table of Contents
- [File Structure](#file-structure)
- [Video](#video)
- [Introduction](#introduction)
- [Operational Manual](#operational-manual)
- [Contributors](#contributors)
- [License](#license)

## File Structure
```
├── Main
|   ├── hpc_case_design
│   |   ├── design_readme.md
│   |   ├── 3d_printing
│   |   │   ├── cad_files
│   |   │   │   ├── head_shelf_design.blend
│   |   │   │   ├── shelf_design.blend
│   |   │   │   ├── general-shelf
│   |   │   │   │   └── ...
│   |   │   │   ├── head-shelf
│   |   │   │   │   └── ...
│   |   │   │   ├── outer-layer
│   |   │   │   │   └── ...
│   |   │   │   └── renders
│   |   │   │       └── ...
│   |   │   └── stl_files
│   |   │       ├── general-shelf
│   |   │       │   └── ...
│   |   │       ├── head-shelf
│   |   │       │   └── ...
│   |   │       └── outer-layer
│   |   │           └── ...
│   |   └── laser_cutting
│   |       ├── 3vs_files
│   |       │   ├── inner_shelf
│   |       │   │   └── ...
│   |       │   ├── outer_shelf
│   |       │   │   └── ...
│   |       │   └── testCut.3vs
│   |       └── dxf_files
│   |           ├── inner_shelf
│   |           │   └── ...
│   |           ├── outer_shelf
│   |           │   └── ...
│   |           └── testCut.dxf
|   ├── nixos
|   |   └── ...
|   ├── research_folder
|   |  ├── Comparisons
|   |  |   └── ...
|   |  ├── Documentations
|   |  |   └── ...
|   |  ├── Images
|   |  |   └── ...
|   |  └── Researches
|   |      └── ...
|   └── video_dev
|       └── scripts
|           └── ...
└── ...
```
## Video

## Introduction
Welcome to the group project README file for the Advanced Computer Engineering module from module leader Sebastian Blair of Team -1.
This document provides an overview of the Design and Implementation of the High Performance Computing (HPC) Systems project, including an explanation of the steps taken to develop the final products: a prototype, video and documentation demonstrating the collaborative effort and technical approach.
HPC involves using clusters of interconnected servers to perform complex calculations quickly. These clusters are nodes managed by schedulers to optimise resource usage. Supercomputers, essentially vast clusters of computing nodes, significantly outperform individual desktops or servers. LinuxⓇ is the leading operating system for HPC.
It is important to note that although a significant milestone has been reached with the creation of this prototype, there is room for further development and improvements.
For detailed reports, insights, and technical documentation, the documentation is hosted in a separate directory in this repository.

## Operational Manual
### Hardware setup
### Software setup
### Recomandations
Some of the project's next steps include incorporating technologies to improve its capabilities and test its abilities. Integrating SingularityCE can simplify the deployment of complex applications in HPC and scientific computing environments, leveraging containerisation for portability and reproducibility. John the Ripper could enhance security by identifying vulnerabilities in different operating systems. Prometheus and Jaeger will facilitate the monitoring and tracking framework, offering insights into system performance and operational dynamics. Furthermore, these integrations will be relatively easy by taking advantage of Slurm's compatibility with Docker.
Users are encouraged to consult the official documentation linked below for installation guidance on these technologies.

- [SingularityCE Documentation](https://docs.sylabs.io/guides/latest/user-guide/)
- [John the Ripper Documentation](https://github.com/openwall/john/tree/bleeding-jumbo)
- [Prometheus Documentation](https://prometheus.io/docs/prometheus/latest/installation/)
- [Jaeger Documentation](https://www.jaegertracing.io/docs/1.55/getting-started/)

## Contributors
- [@Wertasile](https://github.com/Wertasile)
- [@Cypherpol0](https://github.com/Cypherpol0)
- [@OneWayTicketToHell](https://github.com/OneWayTicketToHell)
- [@WJOchman](https://github.com/WJOchman)
- [@CompEng0001](https://github.com/CompEng0001) - Lecturer

## License
<p xmlns:cc="http://creativecommons.org/ns#" >This work is licensed under <a href="http://creativecommons.org/licenses/by-nc-sa/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY-NC-SA 4.0<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/nc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/sa.svg?ref=chooser-v1"></a></p>