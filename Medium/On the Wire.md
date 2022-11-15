# On the Wire (Medium)
> MrMidnight

-----------------------------------------

### Mission Briefing:

```
Greetings Special Agent K. One of our field agents in Malaysia managed to physically breach the office of a corrupt politician. Doubling as a mole for a Chinese criminal enterprise, mostly smuggling endangered animals. In this case their evil business involves shark fin trade and other exotic food items.

During the breach, our agent successfully obtained several pieces of information on the organization. Currently this does not include their name, as they only communicate using anonymous messages and codenames.

We hope that the information, which includes pictures, floorplans, data dumps and packet captures. Will lead to a more complete picture of this organization. We know that the Malaysian government will be exceptionally happy to get this criminal enterprise out of its borders.

All data has been divided over several agents. Your segment for this contract is the analysis of a packet capture file. Figure out what is being communicated and find the message that matters. This message will lead to your Contract Card.

As always. Special Agent K, the contract is yours, if you choose to accept.

[](https://hacktoria.com/wp-content/contracts/items/on-the-wire.zip)
```

## 1. Download assets

Download the packet capture

## 2. Examining pcap

We can analyze the pcap file via wireshark:

```bash
wireshark on-the-wire.pcapng
```

I tried filtering out stuff with different filters but non worked. Since the "link" we get everytime for the card is in https, I started the search function with: "Ctrl+F". Selected the filter to "String" and searched for "https":

```
33621	101.217157988	10.0.2.15	10.0.2.3	DNS	104	Standard query 0x676d A https://pastebin.com/raw/U7zb8Kyh OPT
```

We didnt get an bit.ly link but this one instead:
>https://pastebin.com/raw/U7zb8Kyh

## 3. Getting the flag

By visiting the url we found, we can see the bit.ly link we are searching for:

```
https://bit.ly/3qyrf7t
```