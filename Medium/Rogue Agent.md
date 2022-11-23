# Rogue Agent (Medium)
> MrMidnight

-----------------------------------------

### Mission Briefing:

```
Greetings Special Agent K. We have a request on our hands from our friends over at the CIA. In September of 2021, one of their operatives went missing in action. Upon further investigation, it was discovered this operative went rogue and started a smuggling business for the Russians. Mostly dealing in complex electronics, which have become difficult to come by for Russians after sanctions began.

The agent we’re looking for is named Valentino Maggi. Born in Brooklyn New York on 18.05.1987. Valentino is one of five sons of the Maggi family, who moved to the United States during World War II. Having grown up a middle class lifestyle, his father a car salesman and mother working as an elementary school teacher. Valentino was recruited into the CIA during his time as a student at Columbia University.

Most of his 10 years in active service were spent as an analyst working out of Langley. Recently though, in August of 2020, Valentino moved to oversees work. Being stationed in Italy as a liaison officer for the Italian foreign intelligence agency “Agenzia Informazioni e Sicurezza Esterna”.

Doing stellar work, right up until the point he went missing. Prompting an extensive investigation into his whereabouts. Documents were eventually found on his computer, recovered using forensics tools to recover deleted files. These indicate a heavy involvement with the Russian underground. Acquiring much needed microelectronics for the Russian government.

And that is where your task begins, Special Agent K. One of the files recovered from Valentino’s computer, is an image with a text file. We believe this to be the current location of Valentino Maggi. Locate the safehouse, so local authorities can raid the premises.

As always, Special Agent K. The contract is yours, if you choose to accept.
```
### Sample password:
```
Find out the location and construct the password using the instructions below. This will allow you to open your linkfile and retrieve the Contract Card.

Password Instruction: country-town-coordinate

Password Example: spain-madrid-12.345678-12.345678
```

## 1. Download assets

Download the original image
Download the Cardfile


## 2. Searching for the image

First I tried to reverse search this image with yandex and google lense, but I couldnt manage to find any useful articles or geolocations. The the briefing text also wasnt very helpful. Further attempts was to inspect the image via exiftool and trying to extract hidden files with stegseek. All of that without success. At the end I remembered a challange ive done ealier this day, which was hidden information written inside a image file.

So I tried to read the "code" of the image with a text editor like vim and found a suspicious string of code that doesnt fit to the rest of the image (most of all because of coloring from neovim, since its not as "blue" as others).

>æÊäÄÒÂZäÂÖÒÜÂÆZhh\djrljhZdb\`jnphf


## 3. Decoding

With the hash in hand, we can use cyberchef to decode the hash: https://cyberchef.org/#recipe=Rotate_right(1,false) it turns out to be "rotate right"

>serbia-rakinac-44.259654-21.057843
## 4. Getting the flag

Use this password to unzip the file and get the card
```
