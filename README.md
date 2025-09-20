# Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
## AIM:
To review unallocated space in a disk image, extract data using forensic tools, and understand the digital investigation process.
## REQUIREMENTS
- Autopsy or FTK Imager
- Sleuth Kit (TSK)
- Hex Editor (e.g., HxD)
- Operating System: Windows 10/11 or Linux (Kali preferred)
## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Load into Autopsy or Sleuth Kit]
    B --> C[Identify Unallocated Space]
    C --> D[Scan for Data Signatures]
    D --> E[Carve and Recover Files]
    E --> F[Analyze Recovered Data]
    F --> G[Document Findings in Report]
```
## DESIGN STEPS:
### Step 1 (Acquire Evidence Image):
- Obtain the disk image in ```.dd``` or ```.E01``` format from a trusted forensic acquisition process.
- Verify hash values (MD5/SHA256) to maintain integrity.

### Step 2(Load Image into Forensic Tool):
- Open Autopsy or FTK Imager.
- Create a new case and add the evidence image.

### Step 3(Locate Unallocated Space):
- Navigate to the partition structure view.
- Identify sectors not assigned to any partition (unallocated).
### Step 4(Analyze & Carve Data):
- Use built-in data carving tools to search for file signatures (JPEG, DOCX, PDF, etc.).
- Preview carved files for relevance.
  
## PROGRAM:
| Step | Action                     | Tool Used                   | Output                       |
| ---- | -------------------------- | --------------------------- | ---------------------------- |
| 1    | Load disk image            | Autopsy / FTK Imager        | Partition & unallocated view |
| 2    | Identify unallocated space | Autopsy File System View    | Sector ranges                |
| 3    | Data carving               | Autopsy Data Carving Module | Recovered files              |
| 4    | Export evidence            | Autopsy Export Option       | File copies for analysis     |


## OUTPUT:
Unallocated Space Analysis and Extracted Data Report
1.
<img width="1920" height="1080" alt="Screenshot (6)" src="https://github.com/user-attachments/assets/ee049b8d-e314-4a4e-b27a-548ab04797ac" />
2.
<img width="1920" height="1080" alt="Screenshot (7)" src="https://github.com/user-attachments/assets/bf4f794e-eeeb-4df3-960d-155b09678867" />
3.
<img width="1920" height="1080" alt="Screenshot (9)" src="https://github.com/user-attachments/assets/641f7190-0861-45f6-b8db-a7b90357362d" />
4.
<img width="1920" height="1080" alt="Screenshot (12)" src="https://github.com/user-attachments/assets/fd026986-71d3-428a-983a-3308ea2b43b4" />
5.
<img width="1920" height="1080" alt="Screenshot (13)" src="https://github.com/user-attachments/assets/ba733caf-93bd-4052-8e75-83f595d9db7c" />

6.
<img width="1920" height="1080" alt="Screenshot (16)" src="https://github.com/user-attachments/assets/6ff8cb8d-3c9a-4b93-888a-f8136a5287d2" />

7.
<img width="1920" height="1080" alt="Screenshot (17)" src="https://github.com/user-attachments/assets/44e7e951-fbbf-49ac-a647-4ae0ab47875d" />
8.
<img width="1920" height="1080" alt="Screenshot (19)" src="https://github.com/user-attachments/assets/089f5974-bbd3-46c3-ae65-8d1d15d5b12b" />






## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

