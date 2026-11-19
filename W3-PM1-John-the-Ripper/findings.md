# W3-PM1 – Password Recovery with John the Ripper

## Objective
Extract the password hash from the authorized training PDF, test password candidates with John the Ripper (Jumbo) through the Johnny GUI, and verify the result against the training PDF.

## Procedure
1. Extract the PDF hash using the hash-extraction tool used in the exercise.
2. Open Johnny and load the extracted hash.
3. Start the password-recovery/dictionary attack.
4. Review the result displayed by Johnny.
5. Verify the recovered password by opening the corresponding training PDF.

## Observations
- The supplied screenshot shows the PDF hash loaded in Johnny.
- The Johnny screenshot indicates that 1 of 1 hashes was cracked.
- The recovered password was used to verify access to the corresponding training PDF.

## Evidence
Add the screenshots to the `screenshots/` folder. The README links to the following filenames:

- `Screenshot 2026-11-19 164427.png` – PDF hash extraction
- `Screenshot 2026-11-19 165008.png` – Johnny result
- `Screenshot 2026-11-19 165445.png` – PM1 flag/completion confirmation

## Tools
- John the Ripper (Jumbo)
- Johnny GUI
- PDF hash-extraction tool
- Windows 11

## Notes
Only perform password recovery on files you own or are explicitly authorized to test. Before publishing this repository, remove or redact passwords, full hashes, and challenge flags if they are not approved for public disclosure.
