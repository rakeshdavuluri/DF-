# Evidence Acquisition Using FTK Imager

## Digital Forensics Lab – Experiment 1

### Experiment Title

**Evidence Acquisition Using AccessData FTK Imager**

---

## Objective

To acquire and preserve digital forensic evidence using **AccessData FTK Imager**.

The experiment demonstrates:

- Volatile memory acquisition
- Physical disk acquisition
- Creation of a forensic disk image
- Evidence verification using hash values

---

## Tool Used

**AccessData FTK Imager 4.7.1.2**

FTK Imager is a digital forensic tool used to acquire and analyze forensic evidence.

---

# 1. Volatile Memory Acquisition

FTK Imager can capture volatile memory (RAM) from a running system.

### Step 1: Open Memory Capture

Select **File → Capture Memory** in FTK Imager.

![Memory Capture](images/10-memory-capture.png)

The Memory Capture window provides options for:

- Destination path
- Destination filename
- Including the pagefile
- Creating an AD1 file

---

# 2. Non-Volatile Memory Acquisition

The physical storage device can be acquired by creating a forensic disk image.

## Step 1: Open Create Disk Image

Open FTK Imager and select:

**File → Create Disk Image**

<img width="1033" height="657" alt="Screenshot 2026-08-09 230512" src="https://github.com/user-attachments/assets/fca3b060-0fa6-4385-9267-617e287245fd" />


---

## Step 2: Select Source Evidence Type

Select **Physical Drive** as the source evidence type.

<img width="575" height="426" alt="Screenshot 2026-07-27 231115" src="https://github.com/user-attachments/assets/8e19bdc6-5fab-460b-8633-d579d0a9a5bc" />

---

## Step 3: Select Physical Drive

Select the required physical drive.

In this experiment, the source drive is:

**SanDisk Cruzer Blade USB Device**

<img width="585" height="428" alt="Screenshot 2026-07-27 231129" src="https://github.com/user-attachments/assets/58f9122a-2d8c-44fe-b008-97b405962b7f" />

---

## Step 4: Enter Evidence Information

Enter the case and evidence information.

The details used in this experiment were:

- **Case Number:** 1
- **Evidence Number:** 1
- **Unique Description:** df
- **Examiner:** Rakesh
- **Notes:** exp1

<img width="515" height="392" alt="Screenshot 2026-07-27 231223" src="https://github.com/user-attachments/assets/66156d2d-ac69-472b-bbf7-af887ddbe231" />

---

## Step 5: Select Image Destination

Specify the location where the forensic image will be stored.

In this experiment:

- **Destination:** `D:\`
- **Image Filename:** `diskimage`
- **Image Fragment Size:** `0 MB`

<img width="505" height="390" alt="Screenshot 2026-07-27 231300" src="https://github.com/user-attachments/assets/53ef6c60-de39-4d47-8e08-e0b1f278bec5" />

---

## Step 6: Configure Image Creation

The image destination is added to the Create Image window.

The option **Verify images after they are created** is enabled to verify the integrity of the acquired image.

<img width="500" height="472" alt="Screenshot 2026-07-27 231312" src="https://github.com/user-attachments/assets/400f37d5-d4af-446d-85e2-434c1e548199" />

---

## Step 7: Start Evidence Acquisition

Click **Start** to begin creating the forensic image.

<img width="470" height="355" alt="Screenshot 2026-07-27 224042" src="https://github.com/user-attachments/assets/78c1d84f-68a0-4513-bc98-f284f74d0eaf" />

The acquisition process displays the source drive, destination and progress.

---

## Step 8: Image Created Successfully

After the acquisition is completed, FTK Imager displays:

**Image created successfully**

<img width="465" height="355" alt="Screenshot 2026-07-27 230225" src="https://github.com/user-attachments/assets/5ba6c13e-7696-4e30-9d10-f2492cc86755" />

---

## Step 9: View Image Summary

The Image Summary contains information about the acquisition, including:

- Case information
- Evidence information
- Source drive information
- Drive geometry
- Acquisition details

<img width="458" height="532" alt="Screenshot 2026-07-27 230201" src="https://github.com/user-attachments/assets/09e527bd-0001-4638-9f14-043ffeed92ab" />

---
## Step 10: Hash Verification

The acquired forensic image was verified using MD5 and SHA1 hash values.

- **MD5 Verify Result:** Match
- **SHA1 Verify Result:** Match
- **Bad Blocks:** No bad blocks found in image

<img width="1600" height="453" alt="WhatsApp Image 2026-08-10 at 9 25 15 AM" src="https://github.com/user-attachments/assets/9d46a3c4-eb1a-41e0-a051-8e34d0eb44fa" />


# 3. Evidence Verification

The acquired image is verified using hash values.

The verification process confirms that the acquired forensic image has maintained its integrity.

### Result

**Hash values are matched.**

---

# 4. Result

The physical USB drive was successfully acquired using **AccessData FTK Imager**.

A forensic disk image was created and successfully verified using hash values.

Therefore, the evidence acquisition process was successfully completed.

---

# 5. Conclusion

FTK Imager provides an effective method for acquiring digital forensic evidence while maintaining evidence integrity.

The experiment demonstrated both memory acquisition and physical disk imaging, followed by verification of the acquired evidence.

---

## Course Information

- **Course:** Digital Forensics Lab
- **Experiment:** 1
- **Program:** CSE
- **Academic Year:** 2024–2025
- **Tool:** AccessData FTK Imager 4.7.1.2

---

## Disclaimer

This experiment is performed for educational and authorized digital forensic investigation purposes only.























































