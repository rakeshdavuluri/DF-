Experiment 10 – Use Ghidra to Disassemble and Analyze Malware Code
Aim
Ghidra is a software reverse-engineering framework used to disassemble and analyze binary programs.

This experiment demonstrates how to create a Ghidra analysis project, import a binary file, perform automatic analysis, examine the imported program, and inspect assembly-level information to understand the program's behavior.

Safety Note: Use only benign or controlled sample binaries for this laboratory exercise. Do not execute unknown malware on a normal personal computer. 
EXP-10


Requirements
Ghidra

Java Runtime Environment

Windows / Linux / macOS system

Isolated virtual machine (recommended)

Benign or controlled sample binary

GitHub repository 
EXP-10


Procedure
Step 1 – Open Ghidra
Launch Ghidra on the system.

The Ghidra startup screen displays:

Ghidra Version: 11.4.2

Java Version: 25 
EXP-10

<img width="480" height="275" alt="1" src="https://github.com/user-attachments/assets/6221bc3f-74a2-40e8-ab8b-46bf9c05e282" />

Step 2 – Create a New Project
From the Ghidra project window:


File → New Project
Create a new analysis project. 
EXP-10

<img width="484" height="317" alt="2" src="https://github.com/user-attachments/assets/8c678bc2-6f5a-4cea-aa3e-1b1eb4c0af3f" />

Step 3 – Select Project Type
Select:


Non-Shared Project
Then click Next.

A non-shared project is used for individual laboratory analysis. 
EXP-10

<img width="493" height="268" alt="3" src="https://github.com/user-attachments/assets/56489caf-879e-45d8-ae30-15960f1330ec" />

Step 4 – Open the Ghidra Project
The Ghidra project was created successfully.

The project name used for the experiment was:


hackverse_ctf
From the project window, select:


File → Import File
to import the binary. 
EXP-10

<img width="486" height="297" alt="4" src="https://github.com/user-attachments/assets/a6755231-0308-4d62-8833-71a5a93c8a31" />

Step 5 – Select the Binary File
Browse to the location containing the sample file and select:


binary1 (1)
The selected binary is prepared for import into the Ghidra project. 
EXP-10

<img width="550" height="279" alt="5" src="https://github.com/user-attachments/assets/11611a76-c3dc-4c17-9893-758202e2451d" />

Step 6 – Import the Binary
The Import dialog detects the binary as:

Format: Executable and Linking Format (ELF)

Language: x86:LE:64:default:gcc

Program Name: binary1 (1)

Click OK to import the binary. 
EXP-10
<img width="612" height="389" alt="6" src="https://github.com/user-attachments/assets/2523f16e-fcbc-4a7a-8f46-96b55ca289b5" />


Step 7 – View Import Results
Ghidra displays the Import Results Summary.

The summary provides information about:

Program

Processor

Address size

Functions

Symbols

Data

Other detected properties of the imported binary 
EXP-10

<img width="502" height="397" alt="7" src="https://github.com/user-attachments/assets/ef6ef45f-7da5-4cdd-8be2-8b42dd24be58" />

Step 8 – Start Analysis
After importing the binary, Ghidra opens the CodeBrowser and asks whether binary1 (1) should be analyzed.

Select:


Yes
to start automatic analysis. 
EXP-10
<img width="620" height="242" alt="8" src="https://github.com/user-attachments/assets/b05e80ac-9532-45dd-a563-a04852445e11" />


Step 9 – Configure Analysis
The Analysis Options window is displayed.

The available analyzers are enabled using the standard analysis configuration.

Click:


Analyze
to begin processing the binary. 
EXP-10

<img width="620" height="305" alt="9" src="https://github.com/user-attachments/assets/faa0d17d-1f60-4424-a66c-6c059ba7edaa" />

Step 10 – Analyze the Binary
After analysis, Ghidra CodeBrowser displays the analyzed binary.

The following components can be examined:

Program tree

Listing

Assembly instructions

Functions

Decompiler area

The analyzed program can then be examined to understand its low-level behavior. 
EXP-10

<img width="603" height="302" alt="10" src="https://github.com/user-attachments/assets/64dd521f-a576-41c9-8304-1a6b06684321" />

Result
The binary file was successfully imported and analyzed using Ghidra.

A Ghidra project named:


hackverse_ctf
was created, and the:


binary1 (1)
ELF file was imported successfully.

Automatic analysis was performed, and the resulting program information, assembly instructions, functions, and analysis views were displayed in Ghidra CodeBrowser. 
EXP-10


Conclusion
The experiment successfully demonstrated the basic process of loading, disassembling, and analyzing a controlled binary using Ghidra. 
EXP-10


Tools Used

Ghidra 11.4.2
Java 25
ELF Binary
x86-64 Architecture
Ghidra CodeBrowser
Safety
This experiment should be performed only with benign or controlled binaries, preferably inside an isolated virtual machine. Unknown malware should not be executed on a personal or production system. 
EXP-10



Sources
