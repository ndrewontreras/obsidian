
Design for Moore's Law

### Section 1.4 Under The Covers

***page 19***

**datapath** - the component of the processor that performs arithmetic operations

**control** - the component of the processor that commands the datapath, memory, and i/o devices according to the instructions of the program 

***page 21-22***
**cache memory** -> small, fast memory acting as a buffer for DRAM memory, built using SRAM

**instruction set architecture** - high-level languages, abstraction  

**application binary surface** - combination of both the instruction set and operating system interface provided to application programmer

**implementation** - basically hardware that obeys architecture abstraction (code)

**volatile memory** - storage that retains data only if receiving power (i.e. DRAM)

**nonvolatile memory** - storage that retains data even after lost of power, i.e. DVD disk 


### 1.5 Technologies for Building Processors and Memory

***pg 25***

**transistor** - on/off switch controlled by an electrical signal

**VLSI (very large-scale integrated circuit)** - a device holding thousands to millions of transistors

**silicon** - a natural element that is also a semiconductor 

**semiconductor** - a substance that does not conduct electricity well

**die (chip)** - individual rectangular section that is cut from a **wafer**, more informally known as chips

**Five classic components of a computer** - input, output, memory, datapath, and control (datapath and control sometimes are called the processor). Data is inputted, kept in memory, goes through processor where the control component controls the data along a certain datapath, returned back to memory and ready to be outputted

**ubiquitous** - appearing and found everywhere

### Section 1.6 Performance

**response time (execution time)** - the total time required for a computer to complete a task (i.e. disk access, memory accesses, I/O activities, etc.), individual users are the focused group  

**throughput/bandwidth** -  a measure of performance, total amount of work done in a period of time, i.e. datacenter managers are interested in increasing bandwidth

**CPU execution time** - time CPU spends in computing a task, not including I/O wait time or running other processes/tasks.

**User CPU time** - time CPU spent in program 

**System CPU time** - time CPU spent doing tasks for program but outside of program (performing tasks on behalf of the program)

**clock cycle (tick)** - time for one clock period, usually the processor clock, which almost all systems are constructed with to determine when events take place and runs in discrete time intervals, which run at a constant rate

**clock period** - the length of each cycle 

**clock rate** - inverse of clock period, e.g. 4 gigahertz

**clock cycles per instruction (CPI)** - average # of clock cycles per instruction for a program or program fragment

**instruction count** - the # of instructions executed by a program 

CPU time = instruction count X CPI X clock cycle time && (instruction count X CPI) / clock rate

These formulas are somewhat useful due to them separating the three key factors that affect performance

### 1.7 The Power Wall

***Key take away from this section***: Over the past 30 years, both the clock rate and power consumption have increased in parallel. However, over the last few years, designers have begun reducing the power needed per transistor for logic transition (0 -> 1 -> 0)

***Power Leakage*** - In many servers, leakage current flows even when transistor is off, and is responsible for 40% of the energy consumption. So even increasing the amount of transistors will only increase power dissipation.
\
### 1.8 The Sea Change


"cores" - word for processor

Today programmers must know how to manipulate their code to take full advantage of having multiple processors. This will have to happen contiously as more processors are added to multicore processors

**Parallelism** - 

pipelining - an elagant technique that runs programs faster by overlapping the execution of instructions 

instruction level parallelism - where the *parallel* nature of the hardware is abstracted away so the programmer and the compiler can think of the hardware as executing instructions sequentially

it is now expected to be able to parallel program, had been the "third rail" of computer architecture

parallel programming is by definition, performance programming

programmer must divide the application so that each processor does the same/similar amount of work to maximize response time and such, known as ***reducing communication and synchronization overhead***

Refer to page 45 to review summary of incoming topics associated with parallelism

### 1.9 Real Stuff: Benchmarking the Intel Core i7

workload - the specified set of programs and tasks a computer user runs; a typical workload will also specify relative frequencies






