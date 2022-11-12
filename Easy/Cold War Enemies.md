# Cold War Enemies (Easy)
>MrMidnight

----------------------

### Intro TEXT

```
Greetings Special Agent K. Perhaps you remember our old friend Maksim Kotova? After his capture in Panama he was more than willing to cooporate for reduced sentences.

Following up on the leads he’s given us until this point has resulted in the arrest of several high ranking officials and members of various underground organizations. One of his more promising leads, is a military parts smuggling operation organized by one of Maksim’s former Cold War friends, Vasili Semenov.

Semenov is quietly making a fortune selling Russian military spare parts for scraps to the highest bidder. A lot of these parts aren’t even spares in the literal sense of the word. These parts are all brought together through various air bases around Russia and the world, then routed to a central air base. Where they’re exchanged for cash.

Given the current sticky situation around Russian activity. Not to mention the limited jurisdiction of our client. You are tasked with finding the air base where these sales take place.

The old man wasn’t very much into modern technology, so all we have for you is a sattilite image of the air base. Other items found, are sent to a forensics lab by our client.

Finding the Air Base will lead you to the password for unlocking your link-file.
```

### Sample password

```
Password format sample, no caps:

country-governate-district-airbasename-air-base
```


## 1. Download assets

Download the full size image:

```bash
wget https://hacktoria.com/wp-content/uploads/2022/09/cold-war-enemies-target.jpg
```

Download the link file


## 2. Target info
Via a tool like [Yandex](https://yandex.com/images/)we can reverse search the image. The output of that reveals: "Russia’s Air Base In Syria". By googling that, the first result is [Khmeimim Air Base](https://en.wikipedia.org/wiki/Khmeimim_Air_Base)with the wikipage, we can collect the infos for our password:

```
country=syria
governate=latakia
district=jableh
airbasename=khmeimim-air-base
```

>syria-latakia-jableh-khmeimim-air-base

## 3. Get the flag
Just unzip the password file and visit the link.

```
https://bit.ly/3DAZZNB
```