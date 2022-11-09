---
description: ISSC242 Hardening Operating Systems
---

# ☝ WEEK 1 SECTION 1: Hands-On Demonstration



## SECTION 1: Hands-On Demonstration&#x20;

### Part 1. Group Policy&#x20;

&#x20;

1. the updated policy settings for the new PasswordGPO (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (3) (1).png" alt=""><figcaption></figcaption></figure>

### Part 2. User and Group Administration&#x20;

1. members of the Managers group (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

1. members of the HumanResources group (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

1. members of the ShopFloor group (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

### Part 3. Resource Management&#x20;

1. updated share permissions for the MGRfiles folder (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

1. updated share permissions for the HRfiles folder (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

1. updated share permissions for the SFfiles folder (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (5) (1).png" alt=""><figcaption></figcaption></figure>

### Part 4. Practical Application

1. access test text file for HRUser01 (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

1. access test text file for SFManager (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

## SECTION 2: Applied Learning&#x20;

### Part 1. User and Group Administration&#x20;

1. the two new users within the Contractors OU (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

### Part 2. Group Policy&#x20;

1. the new Password Policy for the yourname\_PasswordGPO (screen capture):&#x20;

<figure><img src=".gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

1. the new Account Lockout Policy for the yourname\_PasswordGPO (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

### Part 3. Resource Management&#x20;

1. the contents of the CoreFiles directory (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

1. the updated Security permissions for the yourtown directory (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

### Part 4. Practical Application&#x20;

1. the result of Part 4, Step 3 (screen capture):&#x20;

<figure><img src=".gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

2\. description of the results of Part 4 for the ANewuser account;&#x20;

<figure><img src=".gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

3\. explanation of the results of Part 4 for the ANewuser account;&#x20;

{% code overflow="wrap" %}
```
When the workstation was shutdown, it lost its connection with 172.30.0.1, therefore loosing its access.
```
{% endcode %}

## SECTION 3: Lab Challenge and Analysis&#x20;

### Analysis and Discussion&#x20;

1. Use the Internet to research the SYSTEM account. Why is it necessary to include this account with full control on a directory?&#x20;

{% code overflow="wrap" %}
```
SYSTEM account unlike a user has no acces, no password, but does allow the use of local services to access files.
```
{% endcode %}

### Tools and Commands&#x20;

1. Using the icacls utility, document the command that will give the ANewuser account write access to the your school folder.&#x20;

```powershell
icacls.exe C:\CoreFiles\AMU /grant ANewuser:W
```
