# Y86Dis
## Introduction: 
	Welcome to my Y86 disassembler. This application is used to read in Y86 .obj files, or files still in their hexadecimal encoding of the Y86 assembly language and translate them to readable y86 code files for the user. 
## Authors: 
	This project was developed by Joseph Joyce and Jacob Mazzarese.
## Description of Equipment/ List of Materials:
* y86dis.cpp – this is the C++ source file containing all the code for this assignment, it reads in the name of a .obj file in the directory and outputs the disassembled contents of the file.
* makefile – this file is used to tie together the dependencies of the overall project; it also serves to remove unneeded output files during the testing stage of development. When typing the “make” command into the terminal the user compiles the entire project and cleans out non-essential files.
* prog1.obj – this is the default file in the directory used to demonstrate the function of the disassembler. You will need to add your own .obj files to run them.
## Code Example:
	Below is an excerpt from the y86dis.cpp file displaying the detR method. The method in it’s entirety has not been included, but this excerpt is sufficient to show how it functions. The method is passed a string that is only one character in length. The method processes the string through an if-else if ladder that assigns and then returns the register name associated with the character. If the character doesn’t correspond to any register an error message is returned.
	std::string detR(std::string rA) {
   if (rA == "0") {
     return "%rax";
   }
   else if (rA == "1") {
      return "%rcx";
   }
   else if (rA == "2") {
        return "%rdx";
   }
…	
…
…
   else {
        return "ERROR OCCURED";
   }
}

## Installation use:
	**Requirements**
To install and use this program you need to have terminal software such as PuTTY and file handling software such as WinSCP to run the commands and download the files from the project. If you don’t already have this software on your machine follow the links below and get comfortable using both before moving forward.
* [PuTTY:](https://www.putty.org/)
* [WinSCP:](https://winscp.net/eng/docs/guide_install)
	**Instructions**
1.	After these are installed, and you’re familiar in their use, copy all the included files from the Y86Dis folder into the directory you wish to use the application.
2.	Navigate to this directory inside of PuTTY or other terminal based software.
3.	Type and enter “make” to compile and clean the project.
4.	Type “./y86dis” and press enter.
5.	Type “prog1.obj” and press enter. This will output the disassembly of prog1.obj to the terminal. To test another file you would just type and enter the filename during this step.
6.	If you wish to disassemble other Y86 .obj files either copy them here or write them here using your favorite text editor and use steps 4 through 6 to run them.
## FAQ’s:
	Q: Can I use other file handling software besides WinSCP?
	* Yes.
## Troubleshooting:
	[Email](joycejk1@appstate.edu) the support team for additional help.
## License
[MIT](https://github.com/JosephJoyce535/Y86Dis/blob/gh-pages/LICENSE)
	
