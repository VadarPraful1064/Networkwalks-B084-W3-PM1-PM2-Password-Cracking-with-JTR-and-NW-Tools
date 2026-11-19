# NetworkWalks B084 – Week 3: Password Recovery with John the Ripper & NetworkWalks Tools

**Cybersecurity Internship | Batch B084 | Week 3**  
**Modules:** W3-PM1 and W3-PM2  
**Environment:** Windows 11

## Overview

This repository documents my Week 3 practical work on password recovery for institute-provided, password-protected PDF training files.

- **W3-PM1:** Extracted PDF password-verification data and performed an offline dictionary/password-recovery test using John the Ripper (Jumbo) with the Johnny GUI.
- **W3-PM2:** Extracted the PDF hash with the NetworkWalks Hash Calculator and tested candidates with the NetworkWalks Password Cracker.

> **Authorization:** All testing documented here was performed only on training files supplied for the internship. Use these techniques only on files you own or have explicit permission to test.

## Repository Structure

Keep the filenames and folder names below exactly as written so the screenshots display correctly in this README.

```text
NetworkWalks-B084-Week3-Password-Recovery/
│
├── README.md
│
├── W3-PM1-John-the-Ripper/
│   ├── findings.md
│   └── screenshots/
│       ├── 01-pm1-pdf-hash-extraction.png
│       ├── 02-pm1-johnny-cracking-result.png
│       └── 03-pm1-flag-captured.png
│
├── W3-PM2-NetworkWalks-Tools/
│   ├── findings.md
│   └── screenshots/
│       ├── 01-pm2-hash-calculator.png
│       ├── 02-pm2-password-cracker-result.png
│       └── 03-pm2-flag-captured.png
│
└── Final-Report/
    └── week-3-report.md
```

## W3-PM1 – Password Recovery with John the Ripper

### Objective

Extract the password-verification data from the authorized PM1 encrypted PDF, test password candidates with John the Ripper, and verify that the recovered password opens the correct PDF.

### Workflow

1. Extract the PDF hash from the authorized training PDF.
2. Load the hash into Johnny, the graphical interface for John the Ripper.
3. Start the password-recovery process.
4. Review the result in Johnny.
5. Open the corresponding training PDF and verify access.

### Evidence

**1. PDF hash extraction**

Save the OnlineHashCrack PDF Hash Extractor screenshot as:

`W3-PM1-John-the-Ripper/screenshots/01-pm1-pdf-hash-extraction.png`

![PM1 – PDF hash extraction](W3-PM1-John-the-Ripper/screenshots/01-pm1-pdf-hash-extraction.png)

**2. John the Ripper / Johnny result**

Save the Johnny screenshot as:

`W3-PM1-John-the-Ripper/screenshots/02-pm1-johnny-cracking-result.png`

![PM1 – Johnny cracking result](W3-PM1-John-the-Ripper/screenshots/02-pm1-johnny-cracking-result.png)

**3. PM1 flag captured confirmation**

Save the PM1 completion/flag screenshot as:

`W3-PM1-John-the-Ripper/screenshots/03-pm1-flag-captured.png`

![PM1 – Flag captured confirmation](W3-PM1-John-the-Ripper/screenshots/03-pm1-flag-captured.png)

### PM1 Findings

- PDF hash extraction was completed.
- Johnny displayed a successful result for the loaded PDF hash.
- The screenshot evidence showed 1 of 1 hashes cracked.
- The recovered password was checked against the corresponding training PDF.

## W3-PM2 – Password Recovery with NetworkWalks Tools

### Objective

Use the NetworkWalks Hash Calculator and Password Cracker to extract and test the PDF password hash for the PM2 training file.

### Workflow

1. Open the NetworkWalks Hash Calculator and select the PDF option.
2. Load the authorized PM2 training PDF and extract its hash.
3. Copy the extracted `$pdf$` hash into the NetworkWalks Password Cracker.
4. Run the provided dictionary attack.
5. Review the attempt count and successful-match message.
6. Open the corresponding training PDF and verify access.

### Evidence

**1. NetworkWalks Hash Calculator**

Save the Hash Calculator screenshot as:

`W3-PM2-NetworkWalks-Tools/screenshots/01-pm2-hash-calculator.png`

![PM2 – NetworkWalks Hash Calculator](W3-PM2-NetworkWalks-Tools/screenshots/01-pm2-hash-calculator.png)

**2. NetworkWalks Password Cracker result**

Save the Password Cracker screenshot as:

`W3-PM2-NetworkWalks-Tools/screenshots/02-pm2-password-cracker-result.png`

![PM2 – NetworkWalks Password Cracker result](W3-PM2-NetworkWalks-Tools/screenshots/02-pm2-password-cracker-result.png)

**3. PM2 flag captured confirmation**

Save the PM2 completion/flag screenshot as:

`W3-PM2-NetworkWalks-Tools/screenshots/03-pm2-flag-captured.png`

![PM2 – Flag captured confirmation](W3-PM2-NetworkWalks-Tools/screenshots/03-pm2-flag-captured.png)

### PM2 Findings

- The Hash Calculator identified the encrypted PDF and extracted a PDF hash.
- The displayed hash information included Revision R4, Version V4, and 128-bit key length.
- The Password Cracker screenshot showed a successful match after 91 of 100 candidate attempts.
- The recovered password was checked against the corresponding training PDF.

## Key Learnings

- A PDF hash is password-verification data used by a compatible tool to test candidate passwords; it is not the plaintext password.
- A dictionary attack tests a list of candidate passwords against the extracted hash.
- A successful match should be verified by opening the exact PDF from which the hash was extracted.
- Keep PM1 and PM2 evidence separate because they refer to different exercises and files.
- Weak or predictable passwords may be discovered when they appear in the tested candidate list.

## Tools Used

| Tool | Purpose |
|---|---|
| Windows 11 | Lab operating system |
| OnlineHashCrack PDF Hash Extractor | PM1 PDF hash extraction |
| John the Ripper (Jumbo) | Offline password-candidate testing |
| Johnny GUI | Graphical interface for John the Ripper |
| NetworkWalks Hash Calculator | PM2 PDF hash extraction |
| NetworkWalks Password Cracker | Browser-based dictionary attack |
| Microsoft Edge | Accessing browser-based tools |

## Final Report

Add your summary and reflections to `Final-Report/week-3-report.md`.

## Responsible Use and Privacy

This repository is for education and authorized security training. Do not test files without permission. Do not upload confidential PDFs or sensitive documents to third-party tools.

**Important before making this repository public:** The screenshots supplied for this exercise visibly contain recovered password text and challenge flags. Blur or crop those values before uploading the screenshots publicly, and remove full hashes, personal information, and any information the training provider expects to remain private. The README image links above assume you have saved sanitized versions using the exact filenames shown.

## Acknowledgement

Thanks to **NetworkWalks Academy** and the Week 3 instructors for the cybersecurity training exercises and practical learning resources.

## Reference

The repository structure and documentation approach were inspired by:

[Networkwalks B084 – W3 PM1 & PM2 Password Cracking with JTR and NetworkWalks Tools](https://github.com/realuwes/Networkwalks-B084-W3-PM1-PM2-Password-Cracking-with-JTR-and-NW-Tools)
