# NetworkWalks B084 – Week 3: Password Recovery with John the Ripper & NetworkWalks Tools

**Cybersecurity Internship | Batch B084 | Week 3**  
**Modules:** W3-PM1 and W3-PM2  
**Environment:** Windows 11

## Overview

This repository documents my Week 3 practical work on password recovery for authorized, institute-provided PDF training files.

- **W3-PM1:** PDF hash extraction and password recovery using John the Ripper (Jumbo) with the Johnny GUI.
- **W3-PM2:** PDF hash extraction and dictionary attack using NetworkWalks Hash Calculator and Password Cracker.

> **Authorization:** These exercises were performed on training files for the internship. Use password-recovery techniques only on files you own or have explicit permission to test.

## Repository Structure

**Important:** The screenshot filenames below are the original filenames of the six images you uploaded. Keep these names unchanged when adding them to GitHub.

```text
NetworkWalks-B084-Week3-Password-Recovery/
│
├── README.md
│
├── W3-PM1-John-the-Ripper/
│   └── screenshots/
│       ├── Screenshot 2026-11-19 164427.png
│       ├── Screenshot 2026-11-19 165008.png
│       └── Screenshot 2026-11-19 165445.png
│
├── W3-PM2-NetworkWalks-Tools/
│   └── screenshots/
│       ├── Screenshot 2026-11-19 165338.png
│       ├── Screenshot 2026-11-19 165421.png
│       └── Screenshot 2026-11-19 165035.png
│
└── Final-Report/
    └── week-3-report.md
```

## W3-PM1 – Password Recovery with John the Ripper

### Objective

Extract the PDF hash from the authorized training PDF, test password candidates using John the Ripper, and verify the recovered password against the PDF.

### Workflow

1. Extract the PDF hash using the PDF hash-extraction tool.
2. Load the extracted hash into Johnny.
3. Start the password-recovery process.
4. Review the result in Johnny.
5. Verify access by opening the corresponding training PDF.
   
Practical Evidence
1. OnlineHashCrack – PDF Hash Extraction

<img width="1917" height="1027" alt="Screenshot 2026-11-19 164427" src="https://github.com/user-attachments/assets/7d2a3c3e-4e96-4a5d-bf16-3d4f11319fe9" />


2. Johnny – John the Ripper Password Recovery Result

<img width="1915" height="1078" alt="Screenshot 2026-11-19 165008" src="https://github.com/user-attachments/assets/df435e56-cc1d-48d2-bf5b-786f176db4e0" />


3. NetworkWalks – PM1 Flag Captured Confirmation

<img width="1917" height="1078" alt="Screenshot 2026-11-19 165029" src="https://github.com/user-attachments/assets/aac21729-f2de-4f47-b7f2-1ccd6b18b71e" />

PM1 Findings
- PDF hash extraction was completed.
- Johnny displayed a successful result for the loaded PDF hash.
- The screenshot shows 1 of 1 hashes cracked.
- The recovered password was checked against the corresponding training PDF.
W3-PM2 – Password Recovery with NetworkWalks Tools
Objective
Use the NetworkWalks Hash Calculator and Password Cracker to extract and test the PDF password hash for the PM2 training file.
Workflow
1. Open NetworkWalks Hash Calculator and select the PDF option.
2. Load the authorized PM2 training PDF and extract its hash.
3. Copy the extracted hash into NetworkWalks Password Cracker.
4. Run the provided dictionary attack.
5. Review the attempt count and successful-match message.
6. Verify access by opening the corresponding training PDF.
Practical Evidence
1. NetworkWalks – Hash Calculator

<img width="1917" height="1026" alt="Screenshot 2026-11-19 165338" src="https://github.com/user-attachments/assets/41bf0edb-7f8a-4f19-a864-6677adbc6529" />


2. NetworkWalks – Password Cracker Result

<img width="1916" height="1031" alt="Screenshot 2026-11-19 165421" src="https://github.com/user-attachments/assets/ea50034b-8fb4-4613-98ba-a0c80e8cc5e1" />


3. NetworkWalks – PM2 Flag Captured Confirmation

<img width="1915" height="1078" alt="Screenshot 2026-11-19 165445" src="https://github.com/user-attachments/assets/cf374c40-a9d3-4df0-ae49-285395b3e872" />


PM2 Findings
- The Hash Calculator extracted a hash from the encrypted PDF.
- The displayed hash information included Revision R4, Version V4, and 128-bit key length.
- The Password Cracker screenshot showed a successful match after 91 of 100 candidate attempts.
- The recovered password was checked against the corresponding training PDF.
Tools Used
Tool	Purpose
Windows 11	Lab operating system
OnlineHashCrack PDF Hash Extractor	PM1 PDF hash extraction
John the Ripper (Jumbo)	Offline password-candidate testing
Johnny GUI	Graphical interface for John the Ripper
NetworkWalks Hash Calculator	PM2 PDF hash extraction
NetworkWalks Password Cracker	Browser-based dictionary attack
Microsoft Edge	Accessing browser-based tools


Key Learnings
- A PDF hash is password-verification data used by a compatible tool to test candidate passwords; it is not the plaintext password.
- A dictionary attack tests a list of candidate passwords against the extracted hash.
- A successful match should be verified by opening the exact PDF from which the hash was extracted.
- Keep PM1 and PM2 evidence separate because they refer to different exercises and files.
- Weak or predictable passwords may be discovered when they appear in the tested candidate list.
Final Report
Add your overall summary and learning reflections to Final-Report/week-3-report.md.
Responsible Use and Privacy
This repository is for education and authorized security training. Do not test files without permission or upload confidential documents to third-party tools.

Before making this repository public: The supplied screenshots visibly contain recovered password text and challenge flags. Blur or crop those values if they are not approved for public sharing. Also protect full hashes, personal information, and any other restricted training information.
Acknowledgement
Thanks to NetworkWalks Academy and the Week 3 instructors for the cybersecurity training exercises and practical learning resources.
