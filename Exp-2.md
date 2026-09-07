# Digital Forensics – Recover Deleted or Damaged Files Using TestDisk

## 📌 Experiment No. 2

### Title
**Recover Deleted or Damaged Files from a Storage Device Using TestDisk**

---

## 🎯 Objective

To recover missing or deleted partitions and repair a corrupted file system using **TestDisk**, a data recovery and disk repair utility.

---

## 📝 Description

TestDisk is used to recover lost partitions, repair corrupted partition structures, and restore damaged file-system boot sectors.

In this experiment, TestDisk is used to:

- Detect the available storage devices.
- Identify the partition table type.
- Analyze the current partition structure.
- Search for missing partitions.
- Verify recovered partitions and files.
- Recover the missing partition.
- Repair the damaged NTFS boot sector.
- Write the recovered partition structure to the disk.

---

## 🛠️ Requirements

- TestDisk
- Storage device / disk image
- Computer or virtual machine
- Administrator/root privileges

---

## 🔄 Procedure

### 1. Create a Log File

Start TestDisk and select **Create** to create a log file containing technical information and messages generated during the recovery process.

Press **Enter** to continue. :contentReference[oaicite:0]{index=0}
<img width="652" height="517" alt="1" src="https://github.com/user-attachments/assets/bda28a6d-9210-4f48-bb3b-0f3d62bf0373" />



### 2. Select the Disk

Select the hard drive containing the missing or damaged partition using the **Up/Down arrow keys**.

Press **Enter** to proceed. :contentReference[oaicite:1]{index=1}
<img width="645" height="517" alt="2" src="https://github.com/user-attachments/assets/194c44b9-c5da-4083-a0db-3ef13af6fb8f" />

### 3. Select Partition Table Type

TestDisk displays the available partition table types.

Select the default partition table type detected by TestDisk and press **Enter**. :contentReference[oaicite:2]{index=2}
<img width="647" height="512" alt="3" src="https://github.com/user-attachments/assets/3c79e31b-be27-402a-8ae9-be2d202380ac" />



### 4. Analyze the Partition Structure

Select **Analyse** to examine the current partition structure and search for lost partitions.

Press **Enter** to continue. :contentReference[oaicite:3]{index=3}
<img width="657" height="518" alt="4" src="https://github.com/user-attachments/assets/af8f268c-b6e0-4d81-9cd8-67c0d7dfe295" />


### 5. Perform Quick Search

Select **Quick Search** to search for missing partitions.

TestDisk can display the discovered partitions during the search. In the experiment, the missing logical partition **Partition 3** was detected. :contentReference[oaicite:4]{index=4}
<img width="647" height="510" alt="5" src="https://github.com/user-attachments/assets/47bf017f-3ea6-4675-a167-576d6c58d196" />
### 6. Verify the Files

Highlight the detected partition and press **P** to list its files.

The directories and files can be checked to verify that the correct partition has been found. :contentReference[oaicite:5]{index=5}
<img width="642" height="517" alt="6" src="https://github.com/user-attachments/assets/74e33e1f-4df6-455f-a5c7-b8d2e73fc8e4" />
### 7. Perform Deeper Search

If a partition is still missing, select **Deeper Search**.

Deeper Search checks backup boot sectors and other file-system information to locate additional partitions. :contentReference[oaicite:6]{index=6}

<img width="646" height="515" alt="7" src="https://github.com/user-attachments/assets/e3c87e41-798c-4fc9-a55b-5fa527d1a05f" />

### 8. Identify the Correct Partition

TestDisk may display multiple partitions with different statuses.

Partitions marked **D (Deleted)** are not recovered unless their status is changed. The correct partition should be identified by listing and verifying its files. :contentReference[oaicite:7]{index=7}


<img width="637" height="515" alt="8" src="https://github.com/user-attachments/assets/c82a5936-4ab7-426f-9880-9b0c31d35c93" />


### 9. Change Partition Status

After verifying the files, change the required partition status from:

`D (Deleted) → L (Logical)`

using the **Left/Right arrow keys**. :contentReference[oaicite:8]{index=8}
<img width="661" height="507" alt="9" src="https://github.com/user-attachments/assets/b4b71bc1-5388-4bfa-8a97-4eb5aa3fcb65" />

### 10. Write the Partition Table

After confirming that all required partitions are correctly listed, select **Write**.

Press **Enter**, confirm with **Y**, and select **OK** to write the recovered partition structure to the disk. :contentReference[oaicite:9]{index=9}


<img width="642" height="516" alt="10" src="https://github.com/user-attachments/assets/744458b2-cc2a-412f-8027-c7acb96dcd6a" />

### 11. Repair the NTFS Boot Sector

If the NTFS boot sector is damaged but the backup boot sector is valid, select **Backup BS**.

Press **Enter**, confirm with **Y**, and select **OK** to copy the backup boot sector over the damaged boot sector. :contentReference[oaicite:10]{index=10}

### 12. Restart the Computer

After the recovery process is completed, TestDisk requires the computer to be restarted for the changes to take effect.

Press **Enter** and reboot the computer. :contentReference[oaicite:11]{index=11}

---

## 🔑 Important TestDisk Options

| Option | Purpose |
|---|---|
| **Create** | Creates a recovery log |
| **Analyse** | Analyzes the current partition structure |
| **Quick Search** | Searches for lost partitions |
| **Deeper Search** | Performs a deeper partition search |
| **P** | Lists files in the selected partition |
| **Write** | Writes the recovered partition structure |
| **Backup BS** | Restores the NTFS boot sector from its backup |
| **Quit** | Returns to the previous menu |

---

## 📊 Recovery Workflow

```text
Start TestDisk
      ↓
Create Log
      ↓
Select Disk
      ↓
Select Partition Table Type
      ↓
Analyse
      ↓
Quick Search
      ↓
Verify Partitions & Files
      ↓
Is Partition Missing?
   ↙          ↘
 Yes           No
  ↓             ↓
Deeper Search   Write
  ↓             ↓
Verify Files   Recover
  ↓
Change Status
D → L
  ↓
Write Partition Table
  ↓
Repair NTFS Boot Sector
  ↓
Restart Computer
