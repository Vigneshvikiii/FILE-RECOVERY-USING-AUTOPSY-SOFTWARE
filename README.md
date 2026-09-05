# FILE-RECOVERY-USING-AUTOPSY-SOFTWARE

## Name : Vignesh S

## Reg No : 212223230240

## AIM
To use **Autopsy Digital Forensics Tool** to retrieve deleted files from a disk image.

---

## REQUIREMENTS
- **Operating System**: Windows 10/11, macOS, or Linux
- **Tool**: [Autopsy Digital Forensics](https://www.autopsy.com/)  
- **Test Data**: Disk image file (`disk.dd`, `disk.img`, `.E01`)

---

## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Install Autopsy]
    B --> C[Create New Case in Autopsy]
    C --> D[Add Data Source: Disk Image]
    D --> E["Run File System & Data Recovery Modules"]
    E --> F[Locate Deleted Files in Results]
    F --> G[Recover and Export Deleted Files]
```
## DESIGN STEPS:
### Step 1:
Open Autopsy and create a new case with appropriate case details.

### Step 2:
Add a disk image as a data source and let Autopsy analyze the content.

### Step 3:
Navigate to the "Deleted Files" section in Autopsy and examine or recover the deleted files.

## PROGRAM:
### Install Autopsy
```bash
# Download Autopsy from:
# https://www.autopsy.com/
# Install following the setup wizard.
```
### Create a New Case
```
# File → New Case
# Enter Case Name: Deleted_File_Recovery
# Choose Base Directory: C:\Cases\Deleted_File_Recovery
# Click Finish
```
### Add Disk Image
```
# Add Data Source → Disk Image or VM File
# Browse to: C:\forensics\disk.dd
# Click Next
```
### Run Ingest Modules
```# Select:
# - File System Analysis
# - Keyword Search (optional)
# - Data Recovery / Carving
# Click Finish
```
### Locate Deleted Files
```
# Navigate to 'Deleted Files' section in the tree view
# Review metadata (size, hash, timestamps)
```
### Export Deleted Files
```
# Right-click → Extract File(s)
# Save to: C:\forensics\Recovered_Files\
```

## OUTPUT:
Recovered Deleted File List and Details

<img width="1600" height="899" alt="image" src="https://github.com/user-attachments/assets/251ad5d6-a4dc-4abc-af70-5e62cc28e47a" />

<img width="1600" height="899" alt="image" src="https://github.com/user-attachments/assets/49b2e8fd-67cb-4fdc-94ba-625eb52eef66" />

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/c1efdbd9-411c-434e-aa4e-8ea047c55557" />

<img width="1600" height="899" alt="image" src="https://github.com/user-attachments/assets/05cc9e82-3fd4-4764-bfae-38e16368152c" />

<img width="1600" height="892" alt="image" src="https://github.com/user-attachments/assets/4c349457-1f78-4c5b-a5c6-1b4a8e0e72ea" />

<img width="1600" height="899" alt="image" src="https://github.com/user-attachments/assets/649837c6-0c7d-4bb1-8aac-371c6672b4a7" />

<img width="1600" height="898" alt="image" src="https://github.com/user-attachments/assets/79e81479-c2b3-441b-a6aa-a59d3ea6b9af" />

<img width="1600" height="899" alt="image" src="https://github.com/user-attachments/assets/c8e924df-4588-462c-b866-aa1f01e980e2" />

<img width="1600" height="895" alt="image" src="https://github.com/user-attachments/assets/56a8d55c-7208-4103-80cb-4fac5bcbf323" />

<img width="1600" height="899" alt="image" src="https://github.com/user-attachments/assets/b186bdb0-2f59-43c4-9461-b4d83eb9fda7" />

<img width="1482" height="926" alt="image" src="https://github.com/user-attachments/assets/58e10ef2-4c1d-430f-9705-a4c316341beb" />

## RESULT:
Deleted files were successfully retrieved and analyzed using Autopsy.
