---
layout: default
---

# Symbolic NS-3

Network programs, such as network protocols and applications, play essential roles on the Internet. However, their correctness is difficult to test, because their behaviors depend on their network environments, but the space of all possible network environments is prohibitively large. Symbolic execution, as a powerful program-analysis technique, can systemically and efficiently explore a large space by leveraging the equivalence classes of cases in the space. However, a significant barrier in using symbolic execution to test network programs is the substantial effort of instrumenting and modifying network programs to model their symbolic network environments. This project provides a powerful and general platform of symbolic network environments so that network programs can be more efficiently and easily tested using symbolic execution for various purposes, such as for finding low-probability bugs, and measuring worst-case performance.

This project develops symbolic network environments by leveraging a well-developed and widely used network simulator, NS-3. Specifically, this project extends NS-3 and develops a symbolic network simulator, called SymNS-3, to symbolically test network programs in various symbolic network environments. SymNS-3 is designed to be easy to use: The application program interface (API) of NS-3 will be extended so that a tester can easily and flexibly define a customized symbolic network environment by just calling the APIs in a simulation script without the need to laboriously instrument the NS-3 simulator. SymNS-3 is also designed to be efficient: multiple NS-3 core components will be re-designed in order to significantly reduce the number of explored program execution paths while still generating the correct simulation results

# Code

## [GitHub Repository](https://github.com/JeffShao96/Symbolic-NS3)

# Documents

## Jianfei Shao, Minh Vu, Lisong Xu, ["Symbolic NS-3 for Exhaustive Testing"](document/Sym_NS_3_V1.pdf), Technicial Report, 2020

## Minh Vu, Phuong Ha, and Lisong Xu, ["Efficient Correctness Testing of Linux Network Stack under Packet Dynamics"](https://ieeexplore.ieee.org/abstract/document/9149060), IEEE International Conference on Communications (ICC), June 2020

## Jianfei Shao, Minh Vu, Mingrui Zhang, Lisong Xu, ["Symbolic NS-3 for Efficient Exhaustive Testing"](document/Sym_NS_3_Slides_2021.pdf), Lightning Talk, Workshop on NS-3, June, 2021

## Minh Vu, Lisong Xu, Sebastian Elbaum, Wei Sun, Kevin Qiao, "Efficient protocol testing with temporal uncertain events using discrete event simulator", to appear on ACM Transactions on Modeling and Computer Simulation

# Team

## Prof. Lisong Xu

## PhD Student: Minh Vu

## Master Student: Jianfei Shao

## Master Student: Mingrui Zhang

# Acknowledgement

This project is supported in part by [NSF FMitF](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1918204&HistoricalAwards=false)
