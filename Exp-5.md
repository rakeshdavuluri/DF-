# Ex. No. 5 – Use Autopsy to Create a Case and Import Evidence

## Digital Forensics Lab

### Aim

To create a forensic case using Autopsy and import a forensic disk image as evidence for digital forensic analysis.

---

## Software Used

- Autopsy 4.23.1
- Windows
- Digital Forensic Disk Image (.E01)

---

## Case Information

| Property | Details |
|---|---|
| Case Name | laptop theft |
| Case Number | case-001 |
| Examiner | Rakesh |
| Evidence Image | 4Dell Latitude CPi.E01 |
| Timezone | Asia/Calcutta |
| Autopsy Version | 4.23.1 |

---

## Description

Autopsy is an open-source digital forensics platform used for analyzing and extracting data from digital devices.

In this experiment, a new forensic case was created in Autopsy and the forensic image `4Dell Latitude CPi.E01` was imported. Ingest modules were configured to analyze the evidence and extract forensic artifacts.

An HTML forensic report was also generated after the analysis.

---

# Procedure

## 1. Create a New Case

Autopsy was opened and a new case was created.

The case information was entered as follows:

- Case Name: `laptop theft`
- Case Number: `case-001`
- Examiner: `Rakesh`

<img width="968" height="586" alt="1" src="https://github.com/user-attachments/assets/563ce303-a9f3-4a2b-97d0-17955e33c28f" />

---

## 2. Select Host

A new host was generated based on the data source name.

<img width="1070" height="672" alt="2" src="https://github.com/user-attachments/assets/b7a90959-a959-483a-a286-6f326b7bed45" />
---

## 3. Select Data Source

The forensic evidence image was selected as the data source.

**Evidence:**

`4Dell Latitude CPi.E01`

<img width="1072" height="668" alt="3" src="https://github.com/user-attachments/assets/624bda3a-8f7b-4c5c-8bca-a109d483b9ca" />

---

## 4. Configure Ingest Modules

The required ingest modules were configured for forensic analysis.

The selected modules included:

- Recent Activity
- Hash Lookup
- File Type Identification
- Extension Mismatch Detector
- Embedded File Extractor
- Picture Analyzer
- Email Parser
- Encryption Detection
- Interesting Files Identifier
- Central Repository
- PhotoRec Carver
- Virtual Machine Extractor

<img width="1072" height="672" alt="4" src="https://github.com/user-attachments/assets/4dabe86d-0580-4b60-b037-596ca121b4a5" />

---

## 5. Analyze Evidence

After the evidence was added, Autopsy processed the forensic image using the configured ingest modules.

The results were displayed in the Autopsy interface.

<img width="1711" height="897" alt="5" src="https://github.com/user-attachments/assets/7fad27c8-906a-4b11-86f9-eb375d816852" />

---

## 6. Generate Report

After the analysis was completed, the **Generate Report** option was selected.

The **HTML Report** module was selected to generate the forensic report.

<img width="937" height="571" alt="6" src="https://github.com/user-attachments/assets/b688ce18-307f-41a9-b4c9-dac5f3cdf765" />

---

## 7. View Generated Report

Autopsy generated an HTML forensic report containing information about the case and analyzed evidence.

<img width="1008" height="842" alt="7" src="https://github.com/user-attachments/assets/79b54210-d3fb-43e4-9803-c95a637edb88" />
---

## 8. Report Generation Completed

The report generation process was completed successfully and the HTML report was saved in the Reports directory.

<img width="902" height="542" alt="8" src="https://github.com/user-attachments/assets/4879bb09-44f1-48b7-9511-7a2e2131fd7f" />

---


---

# Evidence Information

| Property | Details |
|---|---|
| Case Name | laptop theft |
| Case Number | case-001 |
| Examiner | Rakesh |
| Data Source | 4Dell Latitude CPi.E01 |
| Sector Size | 512 Bytes |
| Timezone | Asia/Calcutta |
| Autopsy Version | 4.23.1 |

---

# Analysis Performed

The forensic image was analyzed using Autopsy ingest modules.

The analysis included:

- File Type Identification
- Hash Lookup
- Extension Mismatch Detection
- Embedded File Extraction
- Picture Analysis
- Email Parsing
- Encryption Detection
- Interesting Files Identification
- Recent Activity Analysis
- File Carving

---

# Result

The forensic disk image was successfully imported into Autopsy and analyzed using the configured ingest modules.

Various forensic artifacts were extracted and categorized by Autopsy.

An HTML forensic report was successfully generated containing the case and analysis information.

---

# Conclusion

The experiment successfully demonstrated how to create a forensic case in Autopsy, import a forensic disk image, configure ingest modules, analyze the evidence, and generate an HTML forensic report.

---

# Experiment Workflow

```text
Create New Case
       ↓
Enter Case Information
       ↓
Select Host
       ↓
Select Data Source
       ↓
Import 4Dell Latitude CPi.E01
       ↓
Configure Ingest Modules
       ↓
Analyze Evidence
       ↓
Generate HTML Report
       ↓
Review Report
       ↓
Complete
