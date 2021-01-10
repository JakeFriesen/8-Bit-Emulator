8-Bit Computer Emulator
Jake Friesen
Updated: 2020-11-14
-------------------

NOTE: This emulator uses windows specific console commands, so please run this emulator on a windows computer.

HOW TO USE:
There are 5 premade input tests that can be run with the batch files in this folder, named "TestOutput#".
Running any of these batch files will do two things:
1. The assembly, which can be found in the "TestInput#.asm" files, are run through the customasm assembler,
and the resulting binary is put into the file "input.txt"
2. The emulator is run, which will parse the "input.txt" file and load the binary, then execute the program on the console.
To change any of the input programs, simply open up the assembly files and change any values as required.
If you want more real-time feedback for the assembler success, please use the website assembler, and click "assemble"
This will show any issues that are in the assembly if any, and will output the resulting binary with annotations.

TEST INPUTS:
Below is a list of what each test input program is attempting to do, and what the expected outcome of the program is.
1. Add 30 + 12: This program will attempt to add 30 + 12, and then halt the program. This should only take a few seconds to perform. 
When halted, the console will give a prompt saying that the program has finished execution.
2. Subtract 30 - 12: This program will attempt to subtract 30 - 12, and then halt the program.This should only take a few seconds to perform. 
When halted, the console will give a prompt saying that the program has finished execution.
3. Infinitely add 1: This program will continually add one to the A register, and output the value. 
This program will NOT automatically halt, so closing the window while it is running is fine.
4. Produce fibonacci sequence: This program will produce the fibonacci sequence from 0 to 233, and then jump back to the beginning.
This program will NOT automatically halt, so closing the window while it is running is fine.
5. Multiply 4 x 5: This program will multiply 4 by 5, and then halt. This requires many addition operations, 
so it is expected to take a bit longer (~25 seconds). When halted, the console will give a prompt saying that the program has finished execution.

NOTES ON EXECUTION:
the main sections to look at when evaluating the program execution are as follows:
- the output (lower right), which will show the 'displayed' value of the computer
- the program counter (upper right), which will show if the program is executing sequentially or jumping
- Flags register (second from top right), which will show if the carry or zero flags are set.

THE WEBSITE:
Ultimately the intention is to implement this code onto a website so that anyone can assemble and emulate this 8-bit computer,
without having to download anything. In the meantime, the website is setup with placeholders for the visualizer, and the console 
visualizer can only execute one program. The assembler however is fully operational online.
To run the website, simply click on any of the .html file to run on localhost. Please note however that the assembler DOES NOT WORK
if run on localhost, and must be hosted. I suggest using a local webserver (I have been using "Web Server for Chrome"). Choose to host
the folder titled "356 website", and then go the the ip and click on the folder "web" if prompted.