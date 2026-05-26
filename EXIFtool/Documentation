# ExifTool — Read The Hidden Data In Files

Every file you send reveals more than you think.

## What is ExifTool?
Free open-source tool used to read, write, and
edit metadata hidden inside files like images,
videos, PDFs, and documents.

## What is Metadata?
Hidden data inside a file.
You can't see it — but it's there.

A photo you took contains:
→ Your GPS location
→ Date & time taken
→ Camera model & brand
→ Device serial number
→ Software used to edit it
→ Your real name sometimes

## Installation
sudo apt install exiftool -y

## Commands
exiftool image.jpg               read all metadata
exiftool -GPSLatitude image.jpg  get GPS latitude
exiftool -GPSLongitude image.jpg get GPS longitude
exiftool -Model image.jpg        get camera model
exiftool -DateTime image.jpg     get date & time
exiftool -Author document.pdf    get author name
exiftool -all= image.jpg         remove all metadata
exiftool -all= /path/to/folder/  remove from all files
exiftool *.jpg                   scan all jpg files
exiftool -csv image.jpg          export as CSV

## Sample Output
File Name         : photo.jpg
Camera Model      : iPhone 14 Pro
GPS Latitude      : 31.5204 N
GPS Longitude     : 74.3587 E
Date/Time         : 2024:03:15 14:23:11
Software          : Adobe Lightroom
Author            : Saad

## Use Cases
→ Extract hidden GPS from photos (OSINT)
→ Find who created a document
→ Remove metadata before sharing online
→ Digital forensics investigations
→ Bug bounty & pentesting recon
→ Protect your own privacy

## Privacy Tip
Before posting any photo online:
exiftool -all= yourphoto.jpg
This removes ALL hidden data.

"Every photo tells a story.
ExifTool reads the one
you didn't mean to share."

⚠️ Only use on files you own or have permission to analyze.
