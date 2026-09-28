🔎 Detection of Hidden Data Using StegExpose
Experiment 8
📌 Aim
To use StegExpose to detect possible hidden or steganographic data in digital images. 
EX-08


🛠️ Software Requirements
Java JDK

StegExpose

Windows PowerShell

PNG image files 
EX-08


📖 Introduction
StegExpose is a steganalysis tool used to detect possible hidden information in digital images. It analyzes the statistical properties of images and identifies images that may contain hidden data.

In this experiment, StegExpose was used to analyze a folder containing PNG images. 
EX-08


⚙️ Procedure
Step 1 – Open the StegExpose Folder
The StegExpose folder contains the StegExpose.jar file and the testFolder containing the images.

<img width="549" height="265" alt="1" src="https://github.com/user-attachments/assets/91adc90e-e577-476b-a693-83ed7e6451b0" />

EX-08


Step 2 – Check the Test Images
The images available for analysis were verified using Windows PowerShell.

<img width="562" height="388" alt="2" src="https://github.com/user-attachments/assets/ecea3626-3218-4407-b931-13cdb5da709c" />


Step 3 – Run StegExpose
StegExpose was executed on the testFolder using the following command:

<img width="634" height="317" alt="3" src="https://github.com/user-attachments/assets/15797ec9-15f7-4c2e-8445-8104a4c50fae" />


Step 4 – Save the Analysis Result
The StegExpose output was saved into a text file for documentation.

<img width="614" height="307" alt="4" src="https://github.com/user-attachments/assets/77ab43da-6c6c-4ffe-8cff-36c8abada3ff" />


Step 5 – Generate Detailed Analysis
A detailed CSV report was generated using a threshold value of 0.2.

<img width="634" height="230" alt="5" src="https://github.com/user-attachments/assets/77c8f216-a990-4af3-8685-4960016f92bd" />


Step 6 – Analyze Using Threshold 0.3
StegExpose was also executed using a threshold value of 0.3.

<img width="554" height="237" alt="6" src="https://github.com/user-attachments/assets/e9ca6db0-4887-44f6-b87a-49fd086a1cdd" />
📊 Analysis Results
The StegExpose analysis identified three suspicious PNG images:

Image	Status	Approximate Hidden Data
stego_6666458261_e455d262b5_z.png	Suspicious	114785 bytes
stego_6672108499_85c582a7f9.png	Suspicious	137047 bytes
stego_6672542201_532f70bffe.png	Suspicious	67141 bytes

The results shown in the experiment's PowerShell output indicate that these three images were flagged as suspicious. The detailed CSV analysis also showed the three images as being above the selected stego threshold. 
EX-08 +1


🔍 Observations
StegExpose successfully analyzed the PNG images.

Three images were detected as suspicious.

The analysis produced approximate hidden-data sizes for the suspicious images.

The results were saved in a text file for documentation.

A detailed CSV report was generated using a threshold of 0.2.

The analysis was also performed using a threshold of 0.3.

The same three images were identified as suspicious at the 0.3 threshold. 
EX-08


📁 Output Files
The experiment generated the following analysis files:


stegexpose_result.txt
stegexpose_detailed.csv
These files contain the StegExpose analysis results and detailed statistical information.

📸 Screenshots
The experiment documentation includes screenshots of:

StegExpose folder and testFolder

Test images listed using PowerShell

StegExpose analysis output

Saved stegexpose_result.txt

Detailed CSV analysis

Analysis using threshold 0.3

✅ Result
StegExpose successfully analyzed the images in the test folder and detected three suspicious PNG images. The detailed CSV analysis also showed these three images as being above the selected stego threshold. 
EX-08


🔐 Key Concepts
Digital Forensics · Steganalysis · StegExpose · Hidden Data Detection · Image Analysis · PNG · Statistical Analysis · Steganography

👨‍💻 Experiment Information
Experiment: 08
Topic: Detection of Hidden Data Using StegExpose
Domain: Digital Forensics / Steganalysis
Platform: Windows PowerShell
Tool: StegExpose
