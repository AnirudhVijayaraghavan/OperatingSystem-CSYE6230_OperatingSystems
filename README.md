# To run
- Go inside the kernel folder -> run "make run" command
- Purpose of the Operating System
The primary purpose of our operating system (OS) is to serve as the fundamental interface between the computer hardware and the applications that run on it. In essence, our OS manages and coordinates hardware resources—such as the CPU, memory, storage, to mainly ensure that the user has a secure and familiar CLI like linux.
Our OS has the basic commands available in the linux kernel, as shown in the screenshot file (mv, cp, del, mkdir, cls).
Explanation of the Implemented Functions
In the implemented version of our minimal operating system, the following core functions have been addressed:
1.	Bootloader and Initialization:
The OS begins with a small piece of code, called the bootloader, which runs immediately after power-on. Its function is to prepare the hardware environment (such as setting up memory segments and registers) and load the main OS kernel into memory. Without the bootloader, the system would not know where to find and launch the operating system’s core code.
2.	Basic Console Output:
A simple print function enables the OS to write characters or messages directly to the video memory. This is crucial for providing immediate feedback to the user and debugging system behavior. Here we have auto-loaded some print statements we used for debugging.
3.	Memory and Resource Setup:
Even at an early stage, the OS code must handle basic memory operations and resource allocation. While the current implementation may not include advanced memory management or paging, it ensures a consistent execution environment so that kernel code runs reliably.

## Commands to try out :
- ls : Command to list files after kernel load 
- mkdir <foldername> : Command to create a folder directory
- cd <foldername> & cd ..) : Command to change directory and go into and back out of a folder 
- cat testfile.txt : Command to create a sample file (testfile.txt) inside the created testfolderscreenshot 
- cp testfile.txt testfilecopy.txt : Command to copy testfile.txt into a new file testfilecopy.txt 
- mv testfile.txt testfilenew.txt : Command to rename one file to another name / move file
- del textfilenew.txt : Command to delete a file
- cls : Command to clear screen
