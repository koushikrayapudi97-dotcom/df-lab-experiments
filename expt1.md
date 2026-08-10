# df lab experiments
# Experiment 1: Evidence Acquisition Using AccessData FTK Imager

## Aim

To acquire a forensic disk image from a physical storage device using AccessData FTK Imager and verify the integrity of the acquired image using MD5 and SHA1 hash values.

## Software Used

- AccessData FTK Imager 4.7.1.2
- Windows

## Introduction

FTK Imager is a computer forensic tool developed by AccessData. It is used for acquiring and analyzing digital forensic evidence.

FTK Imager can acquire:

- Volatile memory (RAM)
- Non-volatile memory such as hard disks and USB drives
- Physical drives
- Logical drives
- Image files
- Contents of folders
- CDs/DVDs

In this experiment, a physical USB storage device was acquired and converted into a forensic disk image.

## Procedure

### Step 1: Open FTK Imager

Open **AccessData FTK Imager 4.7.1.2**.

Navigate to the option for creating a disk image.


### Step 2: Select Evidence Source

Select **Physical Drive** and click **Next**.


Select the physical drive that needs to be acquired.

The device used in this experiment was:

**SanDisk Cruzer Blade USB Device**

Click **Finish**.



### Step 4: Select Image Type

Select **Raw (dd)** and click **Next**.



### Step 5: Enter Evidence Information

The following evidence information was entered:

- Case Number: 1
- Evidence Number: 1
- Unique Description: DF
- Examiner: koushik
- Notes: EXP 1

Click **Next**.



### Step 6: Select Image Destination

The image was saved in the following destination:

`D:\3-1\Digital Forensics`

Image Filename:

`diskimage`

Image Fragment Size:

`0 MB`


### Step 7: Create Image

The source and destination information were displayed.

The option **Verify images after they are created** was selected.

Click **Start** to begin the acquisition.



### Step 8: Image Acquisition

FTK Imager started creating the forensic image from the physical drive.



### Step 9: Image Verification

After acquisition, FTK Imager verified the created forensic image.

The verification process checks the integrity of the acquired image using hash values.


### Step 10: Verification Result

The verification result showed:

- MD5 Verify Result: **Match**
- SHA1 Verify Result: **Match**
- Bad Blocks: **No bad blocks found in image**



### Step 11: Image Summary

The image summary provided details about the acquired physical drive.

Important information included:

- Source Type: Physical
- Drive Model: SanDisk Cruzer Blade USB Device
- Drive Interface Type: USB
- Source Data Size: 59112 MB
- Sector Count: 121061376
- Bytes per Sector: 512



### Step 12: Hash Verification

The image summary showed that the computed and reported hash values matched.

**MD5:**

`9f1f7659712cde7bc536dd82f341b5ce`

**SHA1:**

`abaca319c85c310078f410c02f6b11951af63334`

Both verification results were **Match**.


## Result

The physical USB drive was successfully acquired using **AccessData FTK Imager 4.7.1.2** and converted into a **Raw (dd) forensic image**.

The acquired image was successfully verified using MD5 and SHA1 hash values.

## Verification Results

| Parameter | Result |
|---|---|
| Image Type | Raw (dd) |
| Source | Physical Drive |
| Device | SanDisk Cruzer Blade USB Device |
| Source Size | 59112 MB |
| MD5 Verification | Match |
| SHA1 Verification | Match |
| Bad Blocks | No bad blocks found |

<img width="1903" height="1070" alt="Screenshot 2026-08-07 213619" src="https://github.com/user-attachments/assets/86c5c1f6-137d-41d9-9f40-879dc3c363d0" />
<img width="1906" height="961" alt="Screenshot 2026-08-08 220516 - Copy" src="https://github.com/user-attachments/assets/070efa6d-f9ab-4561-8fd2-b4189ca2d487" />
<img width="730" height="590" alt="Screenshot 2026-08-08 221322" src="https://github.com/user-attachments/assets/a4c16845-344f-4394-acfe-e5279425bdd0" />
<img width="735" height="541" alt="Screenshot 2026-08-08 221633" src="https://github.com/user-attachments/assets/4d213950-cf13-4b1e-9eeb-f4b1fe836304" />
<img width="621" height="574" alt="Screenshot 2026-08-08 221808" src="https://github.com/user-attachments/assets/93d6e238-7ec2-45dc-8d4f-10d787638c0d" />
<img width="658" height="449" alt="Screenshot 2026-08-08 225419" src="https://github.com/user-attachments/assets/52bec948-a1ea-4f48-aaaf-1dd4dfa8684e" />
<img width="643" height="536" alt="Screenshot 2026-08-08 230159" src="https://github.com/user-attachments/assets/724d6b84-92b9-4652-8c4a-48b14cba20ae" />
<img width="1919" height="1016" alt="Screenshot 2026-08-08 230315" src="https://github.com/user-attachments/assets/50b49f85-1691-4039-8594-d681929e4814" />
<img width="472" height="364" alt="Screenshot 2026-08-09 210638" src="https://github.com/user-attachments/assets/a6626753-609d-46a3-a6bf-08ee987cbae7" />
