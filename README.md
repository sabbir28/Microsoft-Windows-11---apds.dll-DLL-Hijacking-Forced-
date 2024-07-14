Here is the corrected code with appropriate newline characters:

**Title: Microsoft Windows 11 - 'apds.dll' DLL Hijacking (Forced)**  
**Date: 2023-09-01**  
**Author: Moein Shahabi**  
**Vendor: [Microsoft](https://www.microsoft.com)**  
**Version: Windows 11 Pro 10.0.22621**  
**Tested on: Windows 11_x64 [eng]**  

**Description:**
The HelpPane object in Windows 11 can be exploited to perform DLL hijacking.

**Instructions:**

1. Compile the DLL.
2. Copy the newly compiled DLL "apds.dll" into the "C:\Windows\" directory.
3. Open Command Prompt and execute the following command to test the HelpPane object:
   ```powershell
   [System.Activator]::CreateInstance([Type]::GetTypeFromCLSID('8CEC58AE-07A1-11D9-B15E-000D56BFE6EE'))
   ```
4. If successful, the DLL will be hijacked.
