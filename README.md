# Metadata-Extraction-using-ExifTool-log2timeline-and-Hidden-Data-Search-using-Steganography-Tools
### NAME : G LEKASRI
### REGISTER NUMBER : 212223100025
## AIM:
To extract metadata, perform timeline analysis, and search for hidden data using forensic tools like ExifTool, log2timeline, and steganography detection tools.

## DESIGN STEPS:
### Step 1:
Use exiftool to extract metadata from files such as images, documents, and videos.

### Step 2:
Use log2timeline and plaso to create and analyze event timelines from system logs and file metadata.

### Step 3:
Apply steganography detection tools like steghide, zsteg, or binwalk to uncover hidden data in media files.

## PROGRAM:
Metadata and Timeline Forensics, Steganography Analysis Steps
# A. Using ExifTool – for file metadata

 Install:
```
sudo apt update
sudo apt install exiftool -y
```
 Extract metadata from a file:
```
exiftool image.jpg
```
 Batch process a folder:
```
exiftool -r /path/to/folder
```
Useful flags:

-G: Show metadata group

-time:all: Show only timestamps

-GPSLatitude -GPSLongitude: Extract GPS data

![screenshot 1](https://github.com/user-attachments/assets/4f57f5b7-ac2b-45aa-9ceb-a122dc815f74)

# install log2timeline
```
sudo apt install plaso -y
```
```
sudo apt install steghide -y
```
# Embed data
```
steghide embed -cf /home/kali/Downloads/wallpaper.jpg -ef /home/kali/Downloads/secret.txt
```
![screenshot 2](https://github.com/user-attachments/assets/50b65e90-c8eb-44d9-9020-0934f1199fa6)


Extract hidden data:
```
steghide extract -sf hidden.jpg
```
![screenshot 3](https://github.com/user-attachments/assets/336fe9c0-7971-4bad-8a86-262408070d09)

# Using binwalk – for file analysis

```
sudo apt install binwalk -y
binwalk suspicious.jpg
```
![screenshot 4](https://github.com/user-attachments/assets/ec0dd452-d6ab-44af-82c1-27e4a5a88403)

## OUTPUT:
Extracted Metadata, Timeline Events, and Hidden Data Detection Results
![screenshot 5](https://github.com/user-attachments/assets/0b0c81dd-9b40-4d87-a71d-770186b4d0a7)

## RESULT:
Metadata was successfully extracted, timeline analysis was completed, and hidden data was identified using steganography tools.

