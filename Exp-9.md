Experiment 9 – Process Explorer
Aim
To use Process Explorer to examine running processes, analyze CPU and memory usage, inspect process properties, check network activity, and identify potentially suspicious processes. 
EX-09


Software Required
Windows Operating System

Process Explorer (Sysinternals)

Windows Security

Web Browser 
EX-09


Procedure
Step 1 – Download and Extract Process Explorer
Process Explorer was downloaded and extracted into the ProcessExplorer folder.

The folder contained:

procexp.exe

procexp64.exe

procexp64a.exe

Eula.txt 
EX-09
<img width="336" height="203" alt="1" src="https://github.com/user-attachments/assets/54759fea-6827-4c06-8cde-8a7006c8db67" />


Step 2 – Run Process Explorer as Administrator
The procexp64.exe application was executed using Run as administrator.

Process Explorer displayed the running processes in a hierarchical process tree. 
EX-09


Step 3 – Examine Running Processes
The Process Explorer window was examined using the following columns:

Process

CPU

Private Bytes

Working Set

PID

Description

Company Name

The process tree was inspected to identify processes and their resource usage. 
EX-09

<img width="625" height="390" alt="2" src="https://github.com/user-attachments/assets/0734c8eb-a595-4b70-b076-4c6dab3b2386" />

Step 4 – Inspect Process Properties
The svchost.exe process was selected and its Properties window was opened.

The following information was observed:

Property	Value
Process Name	svchost.exe
PID	1944
Description	Host Process for Windows Services
Path	C:\Windows\System32\svchost.exe
User	NT AUTHORITY\SYSTEM
Company	Microsoft Corporation

The executable path was inspected and verified to be located in the Windows System32 directory. 
EX-09

<img width="570" height="356" alt="3" src="https://github.com/user-attachments/assets/9d984f8b-4dd5-4ddd-9bf8-b93f799da724" />

Step 5 – Inspect TCP/IP Activity
The TCP/IP tab of the svchost.exe Properties window was opened.

The following information was inspected:

Local Address

Remote Address

Protocol

State

Service

No TCP/IP connections were displayed for the selected process at the time of inspection. 
EX-09

<img width="401" height="189" alt="4" src="https://github.com/user-attachments/assets/545adc8f-ebf7-48cd-884a-f4194cddc40e" />

Step 6 – Examine CPU and Memory Usage
The CPU, Private Bytes, and Working Set values were examined for the selected svchost.exe process.

The process did not show unusually high CPU usage during the observation. 
EX-09

<img width="671" height="224" alt="5" src="https://github.com/user-attachments/assets/f2d6f4be-01f8-42e9-b7c0-80d3d2872318" />

Step 7 – Online Process Verification
The process name svchost.exe was searched online to understand its purpose.

The search results described svchost.exe as a Windows system process used to host and manage Windows services. 
EX-09


Step 8 – Antivirus Check
Windows Security → Virus & threat protection was opened and examined.

The available scan result showed:

No current threats

0 threats found

Quick scan completed successfully 
EX-09

<img width="365" height="248" alt="6" src="https://github.com/user-attachments/assets/deac92d5-a58c-4a70-9692-734989f5298a" />

Result
Process Explorer was successfully used to examine running Windows processes.

The svchost.exe process was investigated by checking:

Process ID

CPU usage

Memory usage

Description

Company name

Executable path

TCP/IP activity

The investigation showed that the selected svchost.exe process was located in the Windows System32 directory and was associated with Microsoft Corporation. No TCP/IP connections were displayed for the selected process during the inspection. 
EX-09


Conclusion
The experiment demonstrated how Process Explorer can be used for Windows process analysis, resource monitoring, process-property inspection, and basic investigation of potentially suspicious processes.


Sources
