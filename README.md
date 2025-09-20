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
<img width="1919" height="1079" alt="Screenshot 2025-09-20 112102" src="https://github.com/user-attachments/assets/20dcd79d-d7b2-4adb-8472-5d88693898f3" />

<img width="972" height="571" alt="Screenshot 2025-09-20 112639" src="https://github.com/user-attachments/assets/4708e5f8-95eb-44bd-8643-dca492bb11cc" />


<img width="981" height="583" alt="Screenshot 2025-09-20 112711" src="https://github.com/user-attachments/assets/b929f126-9300-463c-9fba-b2c9991bea17" />


<img width="1069" height="652" alt="Screenshot 2025-09-20 112737" src="https://github.com/user-attachments/assets/00d2b52d-587d-404f-a9db-d227ee8a28cc" />


<img width="1077" height="675" alt="Screenshot 2025-09-20 112758" src="https://github.com/user-attachments/assets/cb4ffbe9-52c6-4634-8105-fe1a48d460e9" />

<img width="1081" height="671" alt="Screenshot 2025-09-20 112900" src="https://github.com/user-attachments/assets/51afe89a-4884-4352-ab72-af201bb163f1" />


<img width="1919" height="1079" alt="Screenshot 2025-09-20 113110" src="https://github.com/user-attachments/assets/344c94b1-1bd6-4be1-959b-741f8820424b" />


<img width="1919" height="1078" alt="Screenshot 2025-09-20 113313" src="https://github.com/user-attachments/assets/f6b94f13-ee4f-4730-a072-13319870fe9f" />


<img width="1919" height="1079" alt="Screenshot 2025-09-20 113419" src="https://github.com/user-attachments/assets/afa161e2-5f07-4402-b776-cfcecf208080" />

<img width="1919" height="1079" alt="Screenshot 2025-09-20 113628" src="https://github.com/user-attachments/assets/b70da430-c224-46fd-ab72-5448adfa4210" />

## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.
