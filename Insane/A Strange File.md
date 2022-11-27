# A Strange File (Insane)
> MrMidnight

-----------------------------------------

### Mission Briefing:

```
Greetings Special Agent K. During a raid of our allies in the country of Oman, several computers and server equipment were confiscated.

The authorities of Oman spent the past week analyzing the data that resides on this hardware. However, they were not able to make sense of all the data.

This is where we come in. The Overseer of Hacktoria has agreed to a no-cure no-pay assignment for the government of Oman. If we manage to figure out what the file they’ve sent us means, we take on several additional contracts in the future, at very favorable terms.

A little more information about this file. It was found in a folder named “meeting location”. It had several text files in it, that all had written details about locations and people.

There was one file however, that the Oman authorities were not able to convert to text. This is the file you find below. Please make sense of it and report your findings Special Agent.

As always, Special Agent K. The contract is yours, if you choose to accept.
```
### Extras:
```
For this contract you will need to use the website https://what3words.com/

The password to open the flagfile consists of (lowercase letters):

country-district-city-areadialcode-what-three-words-business-type

Sample password:

italy-veneto-verona-045-hot-pasta-sauce-paper-mill
```

## 1. Download assets

Download the Strange File
Download the Cardfile

## 2. Decoding

In the strange-file we extracted, we can find a very long string of HEX. The hex is been seperated in 2 different ones via a empty line between them. Cyberchef couldnt manage to decrypt it, but when I tried to convert the HEX into image, I got 2 different ones from the 2 HEXes.

In the first one, we can see a satelite image and the second one, probably a screenshot from google streetview.

## 3. Gathering intel

In the second image we've extracted, we can notice a string of Arabic written on the wall, narrowing our search to: 

```
Algeria, Bahrain, Chad, Comoros, Djibouti, Egypt, Iraq, Jordan, Kuwait, Lebanon, Libya, Mauritania, Morocco, Oman, Qatar, Saudi Arabia, Somalia, Sudan, Syria, Tunisia, United Arab Emirates, Yemen
```

I bought a intel from the discord server and got the following:
>1.  Gaddafi would never wash his car here

Using google I found out that "Gaddafi" was a Libyan revolutionary, politician and political theoris. 
This means that our search further narrows down to "Lybia"

## 4. Finding the location

I opened up google maps and searched through every single gas-station in Lybia, till I found one that matches the satilite location: https://www.google.com/maps/place/%D9%85%D8%AC%D8%AF%D9%8A+%D8%BA%D8%B3%D9%8A%D9%84+%D8%A7%D9%84%D8%B1%D8%AD%D9%84%D8%A9%E2%80%AD/@30.1794822,10.4523144,156m/data=!3m1!1e3!4m5!3m4!1s0x124cc96ede14def1:0xf09995c13d91075d!8m2!3d30.1794584!4d10.4525203

Additionaly on google streetview, we can find the exact wall on the second image.

Now using "whats3words" to search for the gas-station:  "مجدي غسيل الرحلة" and click on the exact sqare, where the satelite image has its cross on: 
https://what3words.com/definitive.doorpost.thickness

>definitive.doorpost.thickness

## 5. Getting the flag

WIth some further googling and look at google maps, we are able to find all the information we needed for the password:

- country = libya
- district = nalut
- city = dirj
- areadialcode = 47
- what-three-words = definitive.doorpost.thickness
- business-type = car wash

> libya-nalut-dirj-47-definitive-doorpost-thickness-car-wash