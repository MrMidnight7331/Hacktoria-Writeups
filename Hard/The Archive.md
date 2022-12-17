# # The Archive (Hard)
> MrMidnight

-----------------------------------------

### Mission Briefing:

```
Greetings Special Agent K. As you might know, the end of the year is always signified with a massive uptick in cyber attacks. Particularly DDoS and Ransomware attacks are commonplace during this time of the year. It’s also the time of the year for agencies worldwide, to crack down on the criminal enterprises destroying the downtime of IT personnel everywhere.

Our good friends over at the FBI have done just that. Yesterday morning around 0400 UTC they were able to seize a warehouse full of C2 servers, crypto miners and an entire scam call-center rolled int one.

During this bust, several laptops of key individuals were confiscated. There was however one laptop of which the owner was able to wipe the disk, right as the raid was happening. The FBI was able to recover most of the files, but is left puzzled at several of them.

You might already feel this one coming. One of these archives was sent our way to be investigated. Find out what you can about the file inside the archive. It seems to have been damaged beyond the point of recovery, but the FBI has hopes our best and brightest can uncover something.

As always, Special Agent K. The contract is yours, if you choose to accept.
```
### Extras:
```
The password starts with “flag-“

MD5 Checksum for The Archive: 2625ae7c180080e580551347831362d7
```

## 1. Download assets

Download the Archive
Download the Flagfile

## 2. Dont get confused

First extract the Archive zip

Both the md5checksum and the HEX in the extracted Archive flag are rabbitholes. If you convert the HEX into a image you'll only recieve a useless rickroll picture. Whats really importent is the FILENAME.

## 3. Decode the cipher

We will use the "cipher-identifier" from [decode.fr](https://www.dcode.fr/cipher-identifier)to analyze the name of the extracted file: psvoxkwo8mm

It will suggest the following decipher method:

- Youtube Link ?
- Affine Cipher
- Mono-alphabetic Substitution
- Cipher Disk/Wheel
- Geohash
- ACII Shift Cipher
- Base 58
- Base62 Encoding
- Substitution Cipher

After trying around, we see that by using ACII Shift Cipher, it return with a valid decrypted message: filename.cc

## 4. Getting the card

By visiting the domain "filename.cc", it will download a zip called: "passarch-mf28f2ukn2vh723f2f23.zip" unzip it and read the content:

```
flag-gh32398D#C*$C#)*$V3405hv3j524952
```

Now unzip the cardfile and get the card!