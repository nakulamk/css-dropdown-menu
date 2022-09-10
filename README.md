# css-dropdown-menu
▪ Waits for interrupt from user.

Interrupt handling –
The occurrence of an event is usually signaled by an interrupt. The interrupt can either
be from the hardware or the software. Hardware may trigger an interrupt at any time by sending a signal to the CPU. Software triggers an interrupt by executing a special operation called a system call (also called a monitor call).
When the CPU is interrupted, it stops what it is doing and immediately transfers execution to a fixed location. The fixed location (Interrupt Vector Table) contains the starting address where the service routine for the interrupt is located. After the execution of interrupt service routine, the CPU resumes the interrupted computation.
Interrupts are an important part of computer architecture. Each computer design has its own interrupt mechanism, but several functions are common. The interrupt must transfer control to the appropriate interrupt service routine
 interrupt
  Processor
  Storage Structure
Stored at a fixed location
Computer programs must be in main memory (RAM) to be executed. Main memory is the large memory that the processor can access directly. It commonly is implemented in a semiconductor technology called dynamic random-access memory (DRAM). Computers provide Read Only Memory(ROM), whose data cannot be changed.
All forms of memory provide an array of memory words. Each word has its own address. Interaction is achieved through a sequence of load or store instructions to specific memory addresses.
A typical instruction-execution cycle, as executed on a system with a Von Neumann architecture, first fetches an instruction from memory and stores that instruction in the instruction register. The instruction is then decoded and may cause operands to be fetched from memory and stored in some internal register. After the instruction on the operands has been executed, the result may be stored back in memory.
IVT
 Interrupt Service Routine

Ideally, we want the programs and data to reside in main memory permanently. This arrangement usually is not possible for the following two reasons:
1. Main memory is usually too small to store all needed programs and data permanently. 2. Main memory is a volatile storage device that loses its contents when power is turned off.
Thus, most computer systems provide secondary storage as an extension of main memory. The main requirement for secondary storage is that it will be able to hold large quantities of data permanently.
The most common secondary-storage device is a magnetic disk, which provides storage for both programs and data. Most programs are stored on a disk until they are loaded into memory. Many programs then use the disk as both a source and a destination of the information for their processing.
The wide variety of storage systems in a computer system can be organized in a hierarchy as shown in the figure, according to speed, cost and capacity. The higher levels are expensive, but they are fast. As we move down the hierarchy, the cost per bit generally decreases, whereas the access time and the capacity of storage generally increases.
In addition to differing in speed and cost, the various storage systems are either volatile or nonvolatile. Volatile storage loses its contents when the power to the device is removed. In the absence of expensive battery and generator backup systems, data must be written to nonvolatile storage for safekeeping. In the hierarchy shown in figure, the storage systems above the electronic disk are volatile, whereas those below are nonvolatile.
An electronic disk can be designed to be either volatile or nonvolatile. During normal operation, the electronic disk stores data in a large DRAM array, which is volatile. But many electronic-disk devices contain a hidden magnetic hard disk and a battery for backup power. If external power is interrupted, the electronic-disk controller copies the data from RAM to the magnetic disk. Another form of electronic disk is flash memory.
I/O Structure
A large portion of operating system code is dedicated to managing I/O, both because of its importance to the reliability and performance of a system and because of the varying nature of the devices.
Every device have a device controller, maintains some local buffer and a set of special purpose registers. The device controller is responsible for moving the data between the peripheral devices.
