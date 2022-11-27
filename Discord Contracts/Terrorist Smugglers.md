# Terrorist Smugglers (4/8)
> MrMidnight | 26.11.2022 / 10.12.2022

-----------------------------------------

### Mission Briefing:

```
Special Agent @Mr.Midnight , This contract needs to be off the books. For the past two years, the government of China has been after a terrorist organization attacking merchant vessels in the South China Sea. Usually we don’t take on contracts from unfriendly nations to our allies. As this group is clearly engaging in terrorist activities, we’ve made an exception. It is however imperative our allies don’t find out. Below you’ll find a message we pulled from one of the terrorist groups’ members. As this person was arrested in international waters by the US NAVY, the Chinese never got their hands on him. Under the much milder US interrogation tactics, the terrorist won’t give any information. We know from previous intelligence that this group frequently handles arms shipments to finance their operation. We need you to figure out if this message is in relation to a shipment. If so, determine when and where the shipment will take place. Communicate your findings in a direct message to the Overseer on Discord.

00110100 01000110 01000101 01010111 01001010 01000011 01010100 00110011 01000101 01011000 01001111 01000100 01000110 00111001 01000101 00110100 01001011 01000110 01000101 00101101 01000011 01001010 00110000 00110111 00101110 01000011 01000011 00101111 01011000 00110110 00101010 00101111 01000101 00110110 01010001 01000100 01001010 01010000 01000011 01001111 01000001 00110111 01000101 01000001 00110111 01010000 00110011 01000100 01001111 01001010 01000101 01010101 00101110 01000011 01001110 01001100 01000110 00111001 01001011 01000011 01000110 00101010 00110101 01011010 01010000 01000011
```

## 1. Decoding 

The first thing we see is this long string of binary. Lets open up cyberchef and decode it:
>4FEWJCT3EXODF9E4KFE-CJ07.CC/X6*/E6QDJPCOA7EA7P3DOJEU.CNLF9KCF*5ZPC

It returns a string of hash that is unrecogizable. But with Base45 decoding, we can get an somewhat shifted url:
>qebcobk.pbz/f/7ra25nvtkmcd999/gur-flzoby.wct

We can get the correct url by using: https://www.dcode.fr/rot-cipher to decipher the string:
>dropbox.com/s/7en25aigxzpq999/the-symbol.jpg

And we have a dropbox URL that leads to a image we can download.

## 2. Image inspecting 

First lets download the image:
```bash
wget dropbox.com/s/7en25aigxzpq999/the-symbol.jpg
```

The image looks like an white spiral on a red background. If we look closely tho, we find that in the bottom left corner, there is a email address: "mrwhiskers1260@gmail.com". If we send a email with whatever message to the email, we will get this respons:

```
Marly Marlin


Hello,

The shipment will take place on 13.10.2022 at 15:00 local time.

There will be a large blue, somewhat rusty container ship at the docks, named "Mojave".

Cargo is to be unloaded right away and moved to camp, container cover is a load of grains from Ukraine. Use four of our trucks from the warehouse, drivers take the regular route.

Below is the dock we will use this time. As we know, security in our Vietnamese docks is not that good, so it should be a walk in the park.
```

It also contains a image file called "shipment-location.jpg"

## 3. Finding the location

So if we read the text carefully, we find that the place is in "Vietnam" and next to the ocean. So I fired up https://satellites.pro/ and searched along the edge of Vietnam, till I found the exact location of the port we are looking for:

"https://satellites.pro/Vietnam_map#11.312631,108.804989,16"

And the carge-ship we need to search, is right next to the cylinder like building with purpleish roof:

"https://satellites.pro/Vietnam_map#11.303015,108.802392,19"

## 4. Getting the flag
Submit the link to a overseer, and get the card.