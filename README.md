# Windows-Forensic-Examiner-Build 
Files for building an offline Windows forensic examiner


**Purpose:** Offline collection of third-party forensic and analysis binaries to support building a Windows forensic examiner in environments with restricted outbound access.  
**Intended use:** Defensive/forensic only. Use only on systems you own or have explicit authorization to examine.  

## Contents

This repository contains the following third-party binaries (all are bundled *as distributed*; no modifications unless explicitly noted) along with their license/attribution information.

### Included Tools


- **jq**  
  - **License:** MIT (code); documentation is CC-BY-3.0. MIT license text should be included. 

- **7-Zip**  
  - **License:** Mostly LGPL-2.1-or-later (with the “unRAR restriction” on some parts) plus some BSD components; the LZMA SDK is public domain. Redistribution in binary form must reproduce the relevant license information. 

- **ILSpy**  
  - **License:** MIT. MIT license text included. 

- **x64dbg**  
  - **License:** GPLv3. Redistribution requires compliance with GPLv3 (include the full license text and source availability notice). 

- **NirSoft Utilities** (e.g., BrowsingHistoryView, ChromeCacheView)  
  - **License/Terms:** Freeware. Executables must remain unmodified; redistribution is allowed only under the original terms (non-commercial, no alteration). A summary notice should live in `third_party_licenses/nirsoft_freeware_notice.txt`. 

- **EZ Tools (Eric Zimmerman)**  
  - **License:** MIT. Include the MIT license text. 

- **Detect It Easy (DiE)**  
  - **License:** MIT. Include the MIT license text. 

- **PEStudio (Basic / Free edition)**  
  - **License/Terms:** Offered “as-is” with no warranty for the basic (free) version. Do not include the professional edition without a valid license. Include the author’s disclaimer and clarify only the free/basic edition is bundled. 



## Integrity

Each binary has its expected SHA256 hash recorded in `hashes.txt`. Run your preferred hashing tool to verify if you have any doubt about corruption or tampering.

Example (PowerShell):

```powershell
Get-FileHash .\jq\jq.exe -Algorithm SHA256
# Compare output to entry in hashes.txt

