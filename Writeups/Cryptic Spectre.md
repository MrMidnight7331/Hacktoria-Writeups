# Cryptic Spectre
> MrMidnight | 25.04.2023
-----------------------------------------

### Prologue:
```
In a secure, undisclosed location, a high-profile organization’s board members gather for an emergency meeting. The atmosphere is tense as they discuss the recent cyber attack that has left their organization reeling. The attackers managed to infiltrate the organization’s network, exfiltrating sensitive data and leaving behind a trail of destruction. The organization’s reputation is at stake, and the board members are desperate to find answers and bring the perpetrators to justice.

Meanwhile, in a dark corner of the internet, a group of skilled hackers celebrates their latest successful operation. They’ve managed to breach the organization’s defenses, gaining access to valuable information that could be sold to the highest bidder or used to further their own nefarious goals. The group, known only by their ominous moniker, has been operating in the shadows for years, leaving a trail of chaos and devastation in their wake.

Back at the organization’s headquarters, a team of cybersecurity analysts works tirelessly to unravel the mystery of the attack. They sift through countless lines of code, searching for any clues that might lead them to the culprits. Amidst the digital debris, one analyst discovers a crucial piece of evidence: a malware hash associated with the attack. The hash, 9e7053a4b6c9081220a694ec93211b4e, could be the key to unlocking the identity of the threat actor group and the target of their attack.

As news of the discovery spreads, the race is on to analyze the hash and trace its origins. Cybersecurity experts from around the world join forces, pooling their knowledge and resources in an effort to bring the attackers to justice. The stakes are high, and the clock is ticking. Every second that passes brings the hackers one step closer to achieving their ultimate goal, while the organization’s future hangs in the balance.

In this high-stakes game of cat and mouse, only the most skilled and resourceful investigators will succeed in unmasking the threat actor group and uncovering the target of their attack. The fate of the organization and the countless individuals affected by the breach rests in their hands.
```


### Mission Briefing:

```
Greetings, Special Agent K.

We’ve received intel about a recent cyber attack on a high-profile organization. Our analysts have provided us with a malware hash found during the investigation:

9e7053a4b6c9081220a694ec93211b4e

Your mission, should you choose to accept it, is to analyze this hash and determine the Advanced Persistent Threat (APT) group behind it and the target of their attack.

As always, Special Agent K. The Contract is yours, if you choose to accept.
```


### Materials and Answer Instruction:
```
Answer Format
APTgroupnumber_targetoftheattack

Answer Sample
APT43_departmentofjustice
```

## 1. Downloading assets

Proceed to download the flag file

## 2. Hash analyzing

We are given the following hash: 
>9e7053a4b6c9081220a694ec93211b4e

My first instinct was to crack the hash. It seems to be MD5. Tried to use various tools like hashcat & crackstation to crack the hash but it does not work. After a few attempts, I tried to just google for this hash AKA directly copy and paste it into google. Suprizingly, it gave some interesting informations:
https://www.hybrid-analysis.com/sample/4845761c9bed0563d0aa83613311191e075a9b58861e80392914d61a21bad976

By then I have noticed that it was mentionend in the text, that this is the hash from a malware sample. Basicly one should just search for this hash on a maleware analyze. 

Proceeding onwards, by using the information on the website, we can retrieve the name of this malware:
>X-Tunnel

## 3. More enumeration

The mission according to the briefing is to find out which APT group + number used this malware on which target. To get this information, we can just keep using google:
https://community.blueliv.com/#!/discover?tags=xtunnel

The name we identified was:
>Advanced Persistent Threat group, "APT28" also known as "Fancy Bear", "Pawn Storm", the "Sednit Gang" and "Sofacy"

## 4. Searching for the target

Now we have both maleware name, APT number and the nickname for this group. We can search for which company got attacked by them:
[https://www.securityweek.com/xtunnel-malware-specifically-built-dnc-hack-report/amp/](https://www.securityweek.com/xtunnel-malware-specifically-built-dnc-hack-report/amp/ "https://www.securityweek.com/xtunnel-malware-specifically-built-dnc-hack-report/amp/")

```
The XTunnel malware that was used by Russian APT threat actor Fancy Bear to penetrate the Democrat National Committee (DNC) network was specifically designed to work against this target, Invincea researchers say.
```

## 5. Assembling the password

With all the information above, we can assemble the password like this:
>APT28_democratnationalcommittee