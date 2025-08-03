# Windows-Forensic-Examiner-Build (Binaries and Scripts Collection)
Files for building an offline Windows forensic examiner


**Purpose:** Offline collection of third-party forensic and analysis binaries to support building a Windows forensic examiner in environments with restricted outbound access.  
**Intended use:** Defensive/forensic only. Use only on systems you own or have explicit authorization to examine.  

## Contents

This repository contains the following third-party binaries (all are bundled *as distributed*; no modifications unless explicitly noted) along with their license/attribution information.

### Included Tools

- **jq**  
  - **License:** MIT (code). MIT license included. :contentReference[oaicite:5]{index=5}

- **7-Zip**  
  - **License:** LGPL-2.1-or-later (with noted component restrictions, e.g., unRAR) and some BSD components; LZMA SDK is public domain. License text included. :contentReference[oaicite:6]{index=6}

- **ILSpy**  
  - **License:** MIT. MIT license included. 

- **dnSpy**  
  - **License:** GPLv3. Comply with GPLv3 when redistributing the binary—full license text included and a notice in `dnspy/README_LICENSE_NOTICE.md`. :contentReference[oaicite:8]{index=8}

- **NirSoft Utilities** (e.g., BrowsingHistoryView, ChromeCacheView)  
  - **License/Terms:** Freeware. Executables are unmodified; redistribution is allowed only non-commercially and must respect their original terms. A summary notice is in `third_party_licenses/nirsoft_freeware_notice.txt`. 

- **EZ Tools (Eric Zimmerman)**  
  - **License:** MIT. Includes forensic collection and analysis utilities. MIT license included. :contentReference[oaicite:10]{index=10}

- **Detect It Easy (DiE)**  
  - **License:** MIT. MIT license included. :contentReference[oaicite:11]{index=11}

- **PEStudio (Basic / Free edition)**  
  - **License/Terms:** Offered “as-is” with no warranty. Free/basic edition is acceptable to bundle; do not include the professional edition without appropriate paid licensing. Author’s disclaimer included. :contentReference[oaicite:12]{index=12}


## Integrity

Each binary has its expected SHA256 hash recorded in `hashes.txt`. Run your preferred hashing tool to verify if you have any doubt about corruption or tampering.

Example (PowerShell):

```powershell
Get-FileHash .\jq\jq.exe -Algorithm SHA256
# Compare output to entry in hashes.txt

