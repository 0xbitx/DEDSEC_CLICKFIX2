
<p align="center">
<img src="https://github.com/user-attachments/assets/de666051-e8a0-4be8-8dc9-61e35d6765e4", width="300", height="300">
</p>

<h1 align="center">DEDSEC_CLICKFIX2</h1> 
<h4 align="center">DEDSEC_CLICKFIX2 is a Linux-based social engineering tool that delivers payloads using a deceptive software activator method</h4>

### DESCRIPTION
CLICKFIX is a social engineering tool designed to deploy malware using a deceptive technique known as the ClickFix attack. The tool creates a fake software activator page to trick the victim into thinking they need to activate legitimate software on their system. Behind the scenes, when the victim interacts with the fake activator (e.g., by clicking a button to "activate" the software), the page then displays a message instructing the user to open a PowerShell and paste the copied content. If the victim follows the instructions, the payload is executed, granting the attacker control or executing malicious code on the target system. This method leverages the trust in software activation processes to bypass user suspicion and deliver the malware effectively. The dropper script, once executed, attempts to disable AMSI (Antimalware Scan Interface) and Windows Defender protections to evade detection. It then creates a quarantined temporary folder that is excluded from Windows Defender scans, downloads an executable (payload.exe) from https://domain.com/, runs it hidden in the background, and subsequently removes all traces of its activity to maintain stealth. This behavior is consistent with advanced staged malware droppers, ensuring the payload is deployed without alerting the victim or security systems.

### Features:

  * Custom Links: Create your own malicious payload links and make them appear legitimate using a flexible link builder.
  * Templates: Choose from a list of pre-made, realistic-looking URLs (e.g., popular software) to mask your payload.
  * Link Masker: Apply the DEDSEC-style masking technique to cloak your real link behind a convincing front, increasing the chances of the victim clicking and following through.
  * Tunnel Integration: Quickly expose your local page to the internet using built-in Cloudflare tunneling.
  * Advanced Staged Malware Dropper
    
### SCREENSHOT 
<p align="center">
<img src="https://github.com/user-attachments/assets/b4ab34e0-cb8b-4e47-ae65-a6b4fd9d93b5", width="500", height="500">
<img src="https://github.com/user-attachments/assets/3e2f3fde-335c-41c6-8f13-c68e1420f98e", width="500", height="500">
</p>

### Create an API Key
1. Create Temporary Email [Tempmail](https://www.emailnator.com/) (Optional)
1. Register a [T.LY Account](https://t.ly/register)
2. Create an [API Token](https://t.ly/settings#/api)
   
### INSTALLATION
    * git clone https://github.com/0xbitx/DEDSEC_CLICKFIX2.git
    * cd DEDSEC_CLICKFIX2
    * sudo pip3 install requests psutil tabulate tqdm
    * chmod +x dedsec-clickfix
    * sudo ./dedsec-clickfix

### TESTED ON FOLLOWING
* Kali Linux 
* Parrot OS 
* Ubuntu

## Support

If you find my work helpful and want to support me, consider making a donation. Your contribution will help me continue working on open-source projects.

**Bitcoin Address: `36ALguYpTgFF3RztL4h2uFb3cRMzQALAcm`**

<h1 align="center"> DISCLAIMER </h1>

<h4 align="center">I'm not responsible for anything you do with this program, so please only use it for good and educational purposes. </h4>



