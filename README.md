# VSDSquadron Mini-INTERN

# TASK 1

# DESCRIPTION:

A development board for RISC-V is the vsdsquadron mini. A 32-bit RISC-V core resides within it. It runs on a 24MHz frequency and contains 16KB of flash memory and 2KB of SRAM. Supporting protocols including SPI, USART, and I2C, the board contains fifteen GPIO pins.

# PROCESS:

The tasks at hand include installing Ubuntu on VMBox, Visual C++, and writing an example of C code along with analyzing RISC assembly code for the sample C code. These are the essential programs for this internship.

Installing Ubuntu on VMBox Open the Ubuntu terminal after installing the tools, then type the command.


Order for Installation of Leafpad apt-get install leafpad $ sudo

 $ cd $ leafpad filename.c & to launch Leafpad

 ![To Open Leafpad](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/5ac9fcc7-2363-4219-ad11-a9aa96f3ba2a)

 # PROGRAM:
 To Find the Sum Of Product

 ![TO FIND THE SUM PROGRAM](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/340df625-8b93-41f0-9fc6-7dbd6e40cea2)

 ![PROGRAM](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/094195cd-567e-46d8-9f0e-b532b6093524)

 # OUTPUT:
 The Output for the program is

 ![OUTPUT](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/24adcd66-17ca-454b-8960-3bb998bf0c58)

 Directing the compilation of RISC-V compiler code $rv64-unknown-elf-gcc-O1 -march=rv64i -mabi=lp64o filename.o filename.c $ -ltr filename.o

 ![To Open the Riscv Compiler](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/c233f032-012e-4414-992b-1fe71633c3f9)

 To view the assembly code, press. $ filename.o riscv64-unknown-elf-objdump-d ------>A lot of code is provided by $ riscv64-unknown-elf-objdump -d filename.o | less ------->offers Reduced Code/main and a way to view the main purpose of the code.

![ASSEMBLY CODE](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/c44881f9-3afd-4aae-a649-c256e9142ffc)

This facilitates navigation by opening the output in the less editor.
Using?main, we search for the keyword main.

![To Find Out Main](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/bba41f05-53f2-43be-be54-6e88f5021fec)

Guidelines for Analyzing Assembly Code RCV64-unknown-elf-gcc-Ofast -mabi=lp64 -march=rv64i -o filename.o filename.c Use $ riscv64-unknown-elf-objdump -d filename.o | less /main

![To command assembly program Ofast](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/17812fb0-9ae1-4a2c-80fb-dd522a90845f)

By utilizing a hexadecimal calculator and deducting the address numbers provided at the leftmost end, let's count the number of instructions that are executed in the main block.
The primary block of instructions consists of fifteen lines.
Let's use an alternative approach to the code compilation. -Ofast should be used in place of -O1.

![Output For Ofast Command](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/eab0fb76-989d-43b8-bb8a-ac86beea2342)

As we can see, there are now just 12 instructions, a decrease in the previous number of instructions.


# TASK 2

o Create a simple C code for the "Crafting a Digital Clock Divider Circuit" project, then use the RISC-V compiler to analyze assembly code instructions.

A circuit known as a clock cycle divider receives an input clock signal and outputs a clock signal with a frequency that is a fraction of the input frequency. This is frequently used to lower the clock signal frequency for different components in digital circuitry.

To create a simple clock cycle divider using a C program that can be compiled with RISC-V GCC, we will simulate the functionality of a digital clock divider circuit in software. This will involve a basic loop that simulates dividing a clock signal by counting cycles.

![leaf pad](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/ee863b93-0174-4ee2-acff-7b266513848d)

# PROGRAM:

Here is a simple C program that demonstrates this concept:

![clock divider program](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/9fa6ee1f-3635-4963-943e-063467305f87)

# EXPLANATION:

1. clock_divider function:

  Takes two parameters: divisor (the factor by which to divide the clock) and cycles (the number of clock cycles to simulate).
  Uses a counter to keep track of the number of cycles.
  Toggles the divided_clock signal whenever the counter reaches the divisor.

2. main function:

  Sets the divisor and cycles values.
  Calls the clock_divider function to perform the simulation.
  Prints out the state of the divided clock signal for each cycle.

# OUTPUT:

The Output for the program is

![clock divider output](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/13a3ae98-1e68-4b4a-903b-0d496485c281)

# Compilation with RISC-V GCC:

To compile this program with RISC-V GCC, follow these steps:

1.Install RISC-V GCC: Make sure you have the RISC-V GCC toolchain installed. You can download and install it from the official RISC-V website or use a package manager if available.

2.Save the Program: Save the above code to a file named clock_divider.c.

3.Compile the Program: Use the following command to compile the program With RISC-V GCC.

![risc v compiler](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/8ef3712c-b363-40f4-83e9-7a61a6c646b7)

Overseeing the RISC-V compiler code compilation $rv64-unknown-elf-gcc-O1 -mabi=lp64o filename.o filename.c -march=rv64i $ -ltr filename.o






















 

 
 


 



