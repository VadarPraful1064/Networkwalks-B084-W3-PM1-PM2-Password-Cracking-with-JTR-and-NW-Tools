# W3-PM2 – Password Recovery with NetworkWalks Tools

## Objective
Extract a PDF password hash with the NetworkWalks Hash Calculator and test candidate passwords using the NetworkWalks Password Cracker.

## Procedure
1. Open the NetworkWalks Hash Calculator and select the PDF option.
2. Select the authorized training PDF and extract its hash.
3. Copy the extracted PDF hash into the NetworkWalks Password Cracker.
4. Run the dictionary attack.
5. Review the attempt count and match result.
6. Verify the result by opening the corresponding training PDF.

## Observations
- The Hash Calculator screenshot shows an extracted PDF hash.
- The displayed PDF information includes Revision R4, Version V4, and a 128-bit key length.
- The Password Cracker screenshot shows 91 of 100 candidates tried and a successful match.
- The recovered password was used to verify access to the corresponding training PDF.

## Evidence
Add the screenshots to the `screenshots/` folder. The README links to the following filenames:

- `Screenshot 2026-11-19 165338.png` – NetworkWalks Hash Calculator
- `Screenshot 2026-11-19 165421.png` – NetworkWalks Password Cracker result
- `Screenshot 2026-11-19 165035.png` – PM2 flag/completion confirmation

## Tools
- NetworkWalks Hash Calculator
- NetworkWalks Password Cracker
- Microsoft Edge
- Windows 11

## Notes
Only test files you own or are explicitly authorized to test. Before publishing this repository, remove or redact passwords, full hashes, and challenge flags if they are not approved for public disclosure.
