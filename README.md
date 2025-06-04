## Running an Unsigned Installer on Windows

When you attempt to launch an unsigned installer, Windows SmartScreen may show a warning dialog titled **“Windows protected your PC”** (or “Windows SmartScreen prevented an unrecognized app from starting”). Follow these steps to bypass the warning safely:

### 1. Click “More info”
- In the SmartScreen dialog, click the **More info** link below the warning text.  
- This expands additional details: the file name and “Publisher: Unknown” (or the developer’s name, if partially registered).

### 2. Click “Run anyway”
- After confirming the source is legitimate, click **Run anyway**.  
- This bypasses SmartScreen for this session and allows the installer to start.

### 3. Acknowledge the UAC prompt
- If User Account Control (UAC) appears (“Do you want to allow this app to make changes to your device?”), click **Yes**.  
- The installer will now launch normally.

---

## Why You See This Message (And Why It’s Not a Virus)

- **No digital signature (certificate).**  
  Windows SmartScreen flags executables lacking an official code-signing certificate. Certificates require identity verification and incur a cost. If a developer skips this step, SmartScreen warns you that it can’t confirm the publisher’s identity.

- **It’s a security precaution, not evidence of malware.**  
  SmartScreen alerts you whenever it cannot verify an app’s publisher. As long as you obtained the installer from a source you trust, clicking **Run anyway** is generally safe. This is not a virus warning but a reminder that the file lacks a trusted signature.
