📱 Android Forensic Data Extraction using AFLogical OSE
Experiment 7
📌 Aim
To use AFLogical OSE (Open Source Edition) to perform logical extraction of forensic data from an Android device and recover information such as SMS messages and call logs. 
EX-07


🎯 Objectives
Understand Android logical data extraction.

Configure the Android Debug Bridge (ADB) environment.

Connect an Android device to a computer.

Install and use AFLogical OSE.

Extract SMS messages from an Android device.

Extract call log information.

Examine the extracted forensic data. 
EX-07


🛠️ Software and Hardware Requirements
Windows Operating System

Android Smartphone

AFLogical OSE

Android Debug Bridge (ADB)

Android Platform Tools

Java Development Kit (JDK)

USB Cable

USB Debugging enabled on the Android device

Text editor for viewing extracted data 
EX-07


📖 Introduction
AFLogical OSE is an Android forensic data extraction tool used for performing logical acquisition of information from Android devices.

It can extract different types of user data, including:

📞 Call logs

💬 SMS messages

👤 Contacts

📩 MMS-related information

The extracted information can be examined as part of a digital forensic investigation. 
EX-07


⚙️ Procedure
Step 1 – Prepare AFLogical OSE
The AFLogical OSE application package was obtained and placed in a working folder on the computer. The folder contained the application package required for installation on the Android device.
<img width="1233" height="695" alt="1" src="https://github.com/user-attachments/assets/88f013b9-ebcd-4767-95c6-369c2fe8a69b" />

Step 2 – Verify Java Installation
Java was installed and verified using the command line. The Java environment was successfully detected and was ready for use with the Android forensic tools. 
EX-07
<img width="956" height="216" alt="2" src="https://github.com/user-attachments/assets/7fc8d3fd-3680-45d4-bdea-be3f905005fb" />


Step 3 – Verify Android Debug Bridge
Android Platform Tools were configured on the computer. ADB was successfully detected and was ready to communicate with the Android device.
<img width="1192" height="362" alt="3" src="https://github.com/user-attachments/assets/b714c86a-c1f0-4f9c-98a2-b49d4711e3f5" />

Step 4 – Connect Android Device
The Android device was connected to the computer using a USB cable. USB Debugging was enabled, and the device was successfully detected by ADB.
<img width="1076" height="235" alt="4" src="https://github.com/user-attachments/assets/a107d2f2-3431-455e-b743-6f985fd6518a" />

Step 5 – Install AFLogical OSE
The AFLogical OSE application was installed on the connected Android device. The installation completed successfully. 
EX-07
<img width="1190" height="207" alt="5" src="https://github.com/user-attachments/assets/e092818d-2fef-4dda-bc42-0ad93877bdb4" />


Step 6 – Extract Android Forensic Data
AFLogical OSE was used to obtain logical forensic information from the Android device. The extracted data included SMS messages and call logs and was saved on the computer for further examination. 
EX-07
<img width="2172" height="151" alt="6" src="https://github.com/user-attachments/assets/15374eb7-6525-4b23-93f8-4833a3a5bb7e" />


Step 7 – Examine Call Log Data
The extracted call log information was examined. The recovered records contained information such as:
<img width="1747" height="132" alt="7" src="https://github.com/user-attachments/assets/f136fe77-13ed-4a37-80c2-4a6d4be2ebb0" />

Phone numbers

Call duration

Call date and time

Call type

Contact information

Other available call-related metadata 
EX-07


Step 8 – Examine SMS Data
The extracted SMS information was examined. The recovered records contained:
<img width="1907" height="985" alt="8" src="https://github.com/user-attachments/assets/4f09aa40-06a6-48f6-9c61-ef6a7a1206bf" />

Sender/recipient address

Message content

Date and time

Message identifiers

Message status

Service information 
EX-07


Step 9 – Detailed Examination
The extracted forensic records were further examined to understand the available information. The SMS records contained detailed metadata and message contents, demonstrating the usefulness of logical acquisition for Android forensic examination. 
EX-07

<img width="1910" height="1078" alt="9" src="https://github.com/user-attachments/assets/9a86550f-fcf1-4be9-8ac1-8099f2963dbf" />

🔍 Observations
Java was successfully installed and detected.

Android Platform Tools were successfully configured.

ADB successfully detected the connected Android device.

AFLogical OSE was successfully installed.

Logical forensic data was successfully extracted.

Call log information was recovered.

SMS information was recovered.

The extracted information contained useful metadata for forensic analysis. 
EX-07


📊 Result
AFLogical OSE was successfully used to perform logical extraction from an Android device. The experiment successfully recovered call logs and SMS messages, which were examined as part of the forensic analysis. 
EX-07


📸 Screenshots / Evidence
The experiment documentation contains screenshots showing:

AFLogical OSE application package

Java installation verification

ADB version verification

Connected Android device

AFLogical OSE installation

Forensic data extraction

Extracted call-log information

Extracted SMS data

Detailed examination of extracted records

These screenshots are documented throughout the experiment, particularly on pages 2–6 of the lab document.

🔐 Forensic Note
This experiment demonstrates logical acquisition for forensic examination. Any extraction should be performed only on an Android device for which you have appropriate authorization.

📚 Key Concepts
Android Forensics · Digital Forensics · Logical Acquisition · AFLogical OSE · ADB · Android Platform Tools · SMS Forensics · Call Log Analysis

👨‍💻 Experiment Information
Experiment: 07
Topic: Use AFLogical OSE to Extract Data from an Android Device
Domain: Digital Forensics / Android Forensics

