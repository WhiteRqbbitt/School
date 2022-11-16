---
description: ISSC242 Hardening Operating Systems Week 1
---

# ☝ Implementing Access Controls with Windows Active Directory



## SECTION 1: Hands-On Demonstration&#x20;

### Part 1. Group Policy&#x20;

&#x20;

1. The updated policy settings for the new PasswordGPO (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (3) (1) (1).png" alt=""><figcaption></figcaption></figure>

### Part 2. User and Group Administration&#x20;

1. members of the Managers group (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

2\. Members of the HumanResources group (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (1) (2).png" alt=""><figcaption></figcaption></figure>

3\. Members of the ShopFloor group (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (7) (1).png" alt=""><figcaption></figcaption></figure>

### Part 3. Resource Management&#x20;

1. Updated share permissions for the MGRfiles folder (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

2\. Updated share permissions for the HRfiles folder (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

3\. Updated share permissions for the SFfiles folder (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (5) (1).png" alt=""><figcaption></figcaption></figure>

### Part 4. Practical Application

1. Access test text file for HRUser01 (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (6) (1).png" alt=""><figcaption></figcaption></figure>

2\. Access test text file for SFManager (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

## SECTION 2: Applied Learning&#x20;

### Part 1. User and Group Administration&#x20;

1. The two new users within the Contractors OU (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (12) (1).png" alt=""><figcaption></figcaption></figure>

### Part 2. Group Policy&#x20;

1. The new Password Policy for the yourname\_PasswordGPO (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

2\. The new Account Lockout Policy for the yourname\_PasswordGPO (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

### Part 3. Resource Management&#x20;

1. The contents of the CoreFiles directory (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

2\. The updated Security permissions for the yourtown directory (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (4) (2).png" alt=""><figcaption></figcaption></figure>

### Part 4. Practical Application&#x20;

1. The result of Part 4, Step 3 (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (3) (1).png" alt=""><figcaption></figcaption></figure>

2\. Description of the results of Part 4 for the ANewuser account;&#x20;

<figure><img src=".gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

3\. Explanation of the results of Part 4 for the ANewuser account;&#x20;

When the workstation was shutdown, it lost its connection with 172.30.0.1, therefore loosing its access.

## SECTION 3: Lab Challenge and Analysis&#x20;

### Analysis and Discussion&#x20;

1. Use the Internet to research the SYSTEM account. Why is it necessary to include this account with full control on a directory?

SYSTEM account unlike a user has no access, no password, but does allow the use of local services to access files.

### Tools and Commands&#x20;

1. Using the icacls utility, document the command that will give the ANewuser account write access to the your school folder.&#x20;

```powershell
icacls.exe C:\CoreFiles\AMU /grant ANewuser:W
```
