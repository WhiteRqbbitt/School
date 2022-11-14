---
description: ISSC242 Hardening Operating Systems Week 2
---

# 🧠 Using Access Control Lists to Modify File System Permissions on Windows Systems

## **SECTION 1: Hands-On Demonstration**

### _**Part 1. View Existing ACLs on a Windows System**_

1. original permissions for the Shopfloor group in the SFfiles directory (screen capture):
   1.

       <figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>
2. original permissions for the HumanResources group in the HRfiles directory (screen capture):
   1.

       <figure><img src=".gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>
3. original permissions for the Managers group in the MGRfiles directory (screen capture):
   1.

       <figure><img src=".gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

### _**Part 2. Modify ACLs using Icacls.exe**_

1. compare the results of the icacls.exe command with the ACLs you documented in Part 1 of this lab: I have compared!
2. compare the results of the icacls.exe command after modifying the ACLs: I have compared this also!
3. icacls.exe results for updated SFfiles directory permissions (screen capture):
   1.

       <figure><img src=".gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>
4. icacls.exe results for updated HRfiles directory permissions (screen capture):
   1.

       <figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>
5. icacls.exe results for updated MGRfiles directory permissions (screen capture):
   1.

       <figure><img src=".gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

### _**Part 3. Validate ACL Settings**_

1. modified New Text Document in the SFfiles directory (screen capture):
2. modified New Text Document in the HRfiles directory (screen capture):
3. modified New Text Document in the MGRfiles directory (screen capture):

## **SECTION 2: Applied Learning**

### _**Part 1. Modify a Script to Add a New User**_

1. the new user account in Part 1 of the script (screen capture):

### _**Part 2. Modify a Script to Add a New Group**_

1. modifications to Part 2 of the script (screen capture):

### _**Part 3. Modify Permissions Using a Script**_

1. current contents of the TargetWindows01 C: drive (screen capture):

### _**Part 4. Create Directories Using a Script**_

1. modifications to Part 4 of the script (screen capture):
2. contents of the new LabDocuments2 directory (screen capture):
3. the permissions for the ISSA01 security group (screen capture):
4. members of the ISSA01 security group (screen capture):

## **SECTION 3: Challenge Questions**

### _**Analysis and Discussion**_

1. Explain how the principle of least privilege can be used in a corporate setting to protect corporate resources.

### _**Tools and Commands**_

1. Research ACLs on the Internet and determine what permissions are required to rename existing files.