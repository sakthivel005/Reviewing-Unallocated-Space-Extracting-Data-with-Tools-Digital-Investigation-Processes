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

<img width="1919" height="1079" alt="Screenshot 2025-09-20 160611" src="https://github.com/user-attachments/assets/d63ab883-61fd-4e35-bc0e-aaade930d68b" />

<img width="1919" height="1079" alt="Screenshot 2025-09-20 160833" src="https://github.com/user-attachments/assets/12515c39-c308-46df-83bd-9ceb182cb769" />

<img width="1064" height="544" alt="Screenshot 2025-09-20 162819" src="https://github.com/user-attachments/assets/849fe9e8-2fcf-42a0-983f-b443fe3e7be0" />

<img width="1919" height="1079" alt="Screenshot 2025-09-20 162530" src="https://github.com/user-attachments/assets/8de124c1-963c-40e8-98ef-325f67f16535" />


<img width="1919" height="1079" alt="Screenshot 2025-09-20 162620" src="https://github.com/user-attachments/assets/e3ee6898-6c7d-4350-96ae-412badfd2fd4" />

<img width="1919" height="1079" alt="Screenshot 2025-09-20 162736" src="https://github.com/user-attachments/assets/78f2c1ae-32f2-4822-84ec-36d917fa3c8f" />

<img width="1919" height="1079" alt="Screenshot 2025-09-20 162853" src="https://github.com/user-attachments/assets/414f436a-debf-4d64-967b-1cf45a6a9377" />


## OUTPUT:
Unallocated Space Analysis and Extracted Data Report

## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.
