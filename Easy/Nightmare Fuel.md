# Nightmare Fuel (Easy)
> MrMidnight 

----------------------------------------------------------------

### Intro TEXT

```txt
Greetings Special Agent K. Yesterday evening around 2100 hours, two officers of the New York Police Department entered the premise of an abandoned building in Brownsville New York. Neighbors had complained about strange sightings. Supposedly a woman had been squatting inside the building.

Reports also state that over the course of the two years the building has been abandoned, several residents of the surrounding houses had complained about junkies occupying the building. Often making terrible screeching like noises during the night.

Normally, this would not get the attention of the NYPD, however, a neighbors’ security camera had caught several people entering the building, but never seen them emerge. Upon closer inspection, a neighbor reported that all windows were closed and intact. Her security camera had also been on the whole time, surveying the only entrance to the building.

This eventually got the NYPD to investigate the building. While clearing rooms, the officers noticed someone moving around at the end of a hallway. Upon repeated calls and commands, the individual retreated behind a door. Both officers approached the door and told the person to come out. After a few seconds, we could see a woman move past the door frame.

Unresponsive to any commands given by the officers, they continued their search. Never to find the woman again. The officers called for backup and had a team of twelve officers and a K-9 unit sweep the building.

Nobody was ever found. Even the dog didn’t find a trail. Which is odd, given all the smells clearly lingering around an old building like that. Strangely enough, upon inspecting the body cam footage, the audio appeared to be missing entirely.

We need you to take a look at the video and see what you can find.

As always, Special Agent K, the contract is yours. If your choose to accept.
```


## 1. Download the given files

Download "Officer 1 Bodycam"
Download "Linkfile"

## 2. Investigating the video file

Watching the video didnt show any importent content. But by using "exiftool" on the video file, we can see a string of password under the "Comments" field:

```bash
exiftool bodycam-officer-1.mp4
```

```
ExifTool Version Number         : 12.49
File Name                       : bodycam-officer-1.mp4
Directory                       : .
File Size                       : 1189 kB
File Modification Date/Time     : 2022:10:11 20:09:34+02:00
File Access Date/Time           : 2022:11:10 00:00:00+01:00
File Inode Change Date/Time     : 2022:10:11 20:09:34+02:00
File Permissions                : -rw-r--r--
File Type                       : MP4
File Type Extension             : mp4
MIME Type                       : video/mp4
Major Brand                     : MP4 Base Media v1 [IS0 14496-12:2003]
Minor Version                   : 0.2.0
Compatible Brands               : isom, iso2, avc1, mp41
Media Data Size                 : 1184500
Media Data Offset               : 48
Movie Header Version            : 0
Create Date                     : 0000:00:00 00:00:00
Modify Date                     : 0000:00:00 00:00:00
Time Scale                      : 1000
Duration                        : 10.50 s
Preferred Rate                  : 1
Preferred Volume                : 100.00%
Preview Time                    : 0 s
Preview Duration                : 0 s
Poster Time                     : 0 s
Selection Time                  : 0 s
Selection Duration              : 0 s
Current Time                    : 0 s
Next Track ID                   : 2
Track Header Version            : 0
Track Create Date               : 0000:00:00 00:00:00
Track Modify Date               : 0000:00:00 00:00:00
Track ID                        : 1
Track Duration                  : 10.50 s
Track Layer                     : 0
Track Volume                    : 0.00%
Matrix Structure                : 1 0 0 0 1 0 0 0 1
Image Width                     : 1920
Image Height                    : 1080
Media Header Version            : 0
Media Create Date               : 0000:00:00 00:00:00
Media Modify Date               : 0000:00:00 00:00:00
Media Time Scale                : 15360
Media Duration                  : 10.50 s
Media Language Code             : und
Handler Description             : VideoHandler
Graphics Mode                   : srcCopy
Op Color                        : 0 0 0
Compressor ID                   : avc1
Source Image Width              : 1920
Source Image Height             : 1080
X Resolution                    : 72
Y Resolution                    : 72
Bit Depth                       : 24
Color Profiles                  : nclx
Color Primaries                 : BT.709
Transfer Characteristics        : BT.709
Matrix Coefficients             : BT.709
Buffer Size                     : 0
Max Bitrate                     : 902476
Average Bitrate                 : 902476
Video Frame Rate                : 30
Handler Type                    : Metadata
Handler Vendor ID               : Apple
Encoder                         : Lavf59.27.100
Comment                         : fh453n3fk45b384gm$&%#fjksdfmo94853ff
Image Size                      : 1920x1080
Megapixels                      : 2.1
Avg Bitrate                     : 902 kbps
Rotation                        : 0

```
>fh453n3fk45b384gm$&%#fjksdfmo94853ff

## 3. Getting the flag
We unzip the linkfile with our password and visit the given link:

```
https://bit.ly/3fYWbvM
```