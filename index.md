---
layout: default
---



This project develops sym-ns-3 for efficient exhaustive testing, where we need to exhaustively test a network protocol or a network application, for all possible cases. Exhaustive testing is useful if we need evaluate all possible performance, find the worst-case performance, or detect bugs of a network protocol or application.


# Motivation

Network programs, such as network protocols and applications, play essential roles on the Internet. However, their correctness is difficult to check, because their behaviors depend on their network environments, but the space of all possible network environments is prohibitively large. Symbolic execution, as a powerful program-analysis technique, can systemically and efficiently explore a large space of cases by leveraging the equivalence classes of cases. However, a significant barrier in using symbolic execution to test network programs is the substantial effort of instrumenting and modifying network programs to model their symbolic network environments. This project provides a powerful and general platform of symbolic network environments, called sym-ns-3, by extending a well-developed and widely-used network simulator, [ns-3](https://www.nsnam.org/), and leveraging a powerful symbolic execution platform, [s2e](https://github.com/S2E/s2e). 


# Goals

sym-ns-3 is designed for efficient exhaustive testing. It is designed to be easy to use: current ns-3 users can easily learn sym-ns-3 and write sym-ns-3 scripts to symbolically test a network protocol or program. sym-ns-3 is also designed to be efficient: multiple ns-3 components have been or will be re-designed to improve the test efficiency.


# Code and Tutorials

sym-ns-3: [code repository with instructions](https://github.com/JeffShao96/Symbolic-NS3)

First Exhaustive Testing Example: [code](https://github.com/JeffShao96/Symbolic-NS3/blob/master/ns-3-dev/scratch/symDemo.cc), [instruction](https://github.com/JeffShao96/Symbolic-NS3/blob/master/README.md#41-first-exhaustive-testing-example)

TCP Exhaustive Performance  Evaluation Example: [code](https://github.com/JeffShao96/Symbolic-NS3/blob/master/ns-3-dev/scratch/tcp-demo.cc), [instruction](https://github.com/JeffShao96/Symbolic-NS3/blob/master/README.md#42-tcp-exhaustive-performance-evaluation)

Whole Network IP Reachability  Example: [code](https://github.com/JeffShao96/Symbolic-NS3/blob/master/ns-3-dev/scratch/reachabilitySymEx.cc), [instruction](https://github.com/JeffShao96/Symbolic-NS3/blob/master/README.md#43-whole-network-ip-reachability)

More Efficient IP Reacjability Example: [code](https://github.com/JeffShao96/Symbolic-NS3/blob/master/ns-3-dev/scratch/IPEfficientSymEx.cc), [instruction](https://github.com/JeffShao96/Symbolic-NS3/blob/master/README.md#44-more-efficient-ip-reachability)

The design and examples of sym-ns-3 are described in our WNS 2022 [[paper](https://doi.org/10.1145/3532577.3532604)],  [[slides](document/Sym_NS_3_Slides_2022.pdf)], and [talk](link will be added soon). 

# Documents

Jianfei Shao, Minh Vu, Mingrui Zhang, Asmita Jayswal, Lisong Xu, "Symbolic NS-3 for Efficient Exhaustive Testing: Design, Implementation, and Simulations", Research Paper, [Workshop on ns-3 (WNS3)](https://www.nsnam.org/research/wns3/wns3-2022/program/), June, 2022 [[paper](https://doi.org/10.1145/3532577.3532604)] [[slides](document/Sym_NS_3_Slides_2022.pdf)]

Minh Vu, Lisong Xu, Sebastian Elbaum, Wei Sun, Kevin Qiao, "Efficient protocol testing with temporal uncertain events using discrete event simulator", ACM Transactions on Modeling and Computer Simulation, Volume 32, Issue 2, April 2022  [[paper](https://doi.org/10.1145/3490028)]

Jianfei Shao, Minh Vu, Mingrui Zhang, Lisong Xu, "Symbolic NS-3 for Efficient Exhaustive Testing", Lightning Talk, [Workshop on ns-3 (WNS3)](https://www.nsnam.org/research/wns3/wns3-2021/program/), June, 2021 [[slides](document/Sym_NS_3_Slides_2021.pdf)]

Minh Vu, Phuong Ha, and Lisong Xu, "Efficient Correctness Testing of Linux Network Stack under Packet Dynamics", IEEE International Conference on Communications (ICC), June 2020 [[paper](https://ieeexplore.ieee.org/abstract/document/9149060)]

Jianfei Shao, Minh Vu, Lisong Xu, "Symbolic NS-3 for Exhaustive Testing", Technical Report, 2020 [[paper](document/Sym_NS_3_V1.pdf)]

# Team

Prof. Lisong Xu

PhD Student: Minh Vu

Master Student: Jianfei Shao

Master Student: Mingrui Zhang

Undergraduate Student: Asmita Jayswal


# Impact

The project has provided and will continue  to provide several students with trainings in network simulation, network protocols, software testing, symbolic execution, and technical writing and presentations. 

sym-ns-3 being developed in this project will likely enable the networking community to more efficiently test network protocols for measuring worst-case performance or finding low-probability bugs in a large test space. 

# Contact

If you have any questions, please feel free to contact us. 
* [Jianfei Shao](mailto:jianfei.shao@huskers.unl.edu?subject=SymbolicNS3)
* [Lisong Xu](mailto:xu@unl.edu?subject=SymbolicNS3)


# Acknowledgement

This project is supported in part by [NSF FMitF Track II](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1918204&HistoricalAwards=false)
