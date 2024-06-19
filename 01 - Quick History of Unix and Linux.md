# Unix

- released in 1969
    - Main developers: Ken Thompson and Dennis Richie (Bell Labs)
    - Unix was created on a Digital Equipment PDP7 and further developed on a PDP11
    - In the 1970's "man pages" were created, initially called "Unix Programmers' Manual"
    - Refer to: https://en.wikipedia.org/wiki/History_of_Unix
- Started using C programming language instead of assembly language
    - The OS written in a higher language made it "portable" (so it can be compiled on other computers)
- Innovations:
    - Computer processes
    - Hierarchy of filesystem
    - Device files
    - a command line interpreter program (shell)
    - many small utility programs (cp, ls, cd, cat, grep, etc.)
        - output of small utilities can be "piped" to other utilities to do more things in combination
        - reduce the need to create large "monolithic" applications, when smaller utilities can be used and reused to create needed functions

## Unix as a Simple System

The original idea of Unix stemmed out of frustration with the alternative "Multics" system. The idea was to simplify a system to run on a "mini-computer" (minimal computer) such as the PDP series. These computers were not sophisticated and did not have a lot of resources. The OS could not have been sophisticated or complex, because the hardware was not capable of running too complex of an OS.  
Unix is so simple that the simplicity has enabled it to stand the test of time for decades, and the concepts and ideas are still in use and completely relevant in our current computing environments today. If you have an ideas such as "Linux/Unix is hard", or "Linux/Unix is complicated", this is due to a lack of information and is certainly not true.

## Unix Features

- Multi-user environment
    - Security and authentication
    - User accounts, groups, and permissions
- Multi-tasking
- Networking (envisioned as OS for remote-access, time-shared machines)

## Unix Drawback and Small Install-base

The drawbacks of Unix-based OS are not technical based, but rather has to do be commercialization and complex licensing. Since the OS was created in a commercial environment, the terms or use and licensing has been subjects of many lawsuits and controversies over the years. In my opinion, commercial interest has played a majour role in having Unix not be adopted as widely as MS-DOS and other operating systems.  
Unix-based OS exist today and are in use in various forms, such as "BSD" licensed versions (FreeBSD, and NetBSD), as well as commercial versions (such as HP-Unix).

# GNU Project and Free Software Foundation

Due to frustrations stemming from the commercialization, issues around licensing, and controversies surrounding copyright for software, a philosophy of "free software" was formed around academia and hacker culture which led to the "Free Software Movement".  
The "Four Essential Freedoms" of free software:

- Freedom to run the programs as you wish for any purpose
- The freedom to study how the program works, and change it so it does your computing as you wish
- The freedom to redistribute copies so you can help your neighbour
- The freedom to distribute copies of your modified versions to others

## GNU Project and FSF

Richard Stallman was a software developer who worked at MIT Artificial Intelligence Lab in 1971. However he had some negative experiences with proprietary software, such as the code that he wanted to work on or fix was locked up. This has seemingly lead to his profound hostility towards proprietary software and Intellectual Property.

- Richard Stallman launched the GNU Project in 1983
    - GNU stands for "GNU is Not Unix", see the "GNU song" for more context of the meaning, for example, this Muppet Show version: https://www.youtube.com/watch?v=cGVdCGxh1IY
    - The GNU Project was to serve as an example of Free Software for the Free Software Movement
    - GNU creates and maintains implementations of many basic utilities, but all software is released with a permissive license (GNU GPL Licenses and other "copy-left" licenses)
        - This also includes the C-Compiler and debuggers required for development work
        - Utilities have the same name and function as Unix utilities
        - The Kernel is called Hurd, but development is stalled and product is unfinished
- Richard Stallman also founded the Free Software Foundation in 1985
    - Non-profit organization focused on supporting and promoting the Free Software Movement
    - mostly intended to employ engineers to write free software for the GNU Project
    - Volunteers have worked on legal and structural issues for the free software movement

The result of the GNU project is many free versions of essential utilities that we use in Linux.

Sources:

- https://en.wikipedia.org/wiki/Free_Software_Foundation
- https://en.wikipedia.org/wiki/GNU
- https://en.wikipedia.org/wiki/GNU_Project

# Birth of Linux

In 1991, Linus Torvalds, a student from Finland, was unsatisfied with the state of software that was available to him for his own personal computer. He used his engineering knowledge and experience to create a new kernel from scratch as a personal project. He cloned many functions of the Unix kernel. Then he released the source code to the public for free.  
![520411e0923479a41cc17d65a0bdc636.png](:/bd746daaf0074791b6c2eb8904519358)

## The GNU/Linux OS

Linux is only the kernel and does not contain any utilities or user programs.

- Kernel is the code that manages the hardware, for example, contains drivers that know how to communicate and utilize the underlying hardware
- Kernel also "abstracts" hardware from software, creating a layered architecture.
    - This means that software becomes "portable" since it is not specifically written for specific hardware. As long as the Kernel is running, the software will theoretically work on any hardware

The GNU Project was working on its own kernel called "Hurd". Hurd is a "Micro-kernel" (many small services that require to maintain synchronicity) so development met some challenges and took some time. The Hurd project is still ongoing and unfinished.  
Linux Torvalds created Linux as a "monolithic kernel" (the kernel is one large program), therefore he managed to develop Linux faster. The GNU Project community decided to adopt the Linux kernel since the project was moving much faster.

For more information see: https://www.gnu.org/home.en.html

* * *
Github Main Page: [https://gorbehnare.github.io/Introduction-to-Linux/](https://gorbehnare.github.io/Introduction-to-Linux/)
