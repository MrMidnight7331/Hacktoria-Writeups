# # Road to Nowhere (Medium)
> MrMidnight

-----------------------------------------

### Mission Briefing:

```
Special Agent K, we’ll be needing your assistance on a geolocation matter. One of our clients, a medium sized European goverment agency, has requested we find a needle in a haystack.

Our client is involved in fighting terrorist groups in Asia and Africa. Recently, they gained access to a Dropbox account filled with map data. Most of these seem to be related to safe houses used by a terrorist organization called “The Meercats”. Indeed a strange name, but nontheless, they mean business.

After having located most safehouses, our client is still struggling to locate a few of them. Since the operation to take down all of these locations needs to be synchronized. There’s an urgent need to identify them all before the next phase can begin.

Below you find an image of what appears to be a village, with a red marker to indicate the exact location. It’s your assignment to find where in the world this is. Currently we have reason to believe this is in Africa or Asia. But, given the organizations’ widespread members, this is only a guess at this time.

Use the coordinates you find as the password to open the ZIP archive. Inside, you find the linkfile to your Contract Card as always. Also, we heard the number 1920 is of importance in this case…

As always. Special Agent K, the contract is yours, if you choose to accept.
```


## 1. Download assets

Download the linkfile
Download the original image:

```bash
wget https://hacktoria.com/wp-content/uploads/2022/08/road-to-nowhere-challenge.jpg
```

## 2. Extract hidden data / bruteforcing

I tried useing yandex and google lense to find informations about this image, but it didnt work. So ill try to reveal information, hidden by "steghide" from this jpg, by using a tool called "stegseek":

```bash
stegseek road-to-nowhere-challenge.jpg
```

Its default wordlist should be "rockyou.txt" and indeed we got ourselves the password, and the secret:

```
StegSeek 0.6 - https://github.com/RickdeJager/StegSeek

[i] Found passphrase: "1920"B)           
[i] Original filename: "location.txt".
[i] Extracting to "road-to-nowhere-challenge.jpg.out".
```

## 2.5 Extract hidden data / password

In the briefing text, we saw the number 1920:

>Also, we heard the number 1920 is of importance in this case…

We can use this as an password to reveal the secret:

```bash
steghide extract -sf road-to-nowhere-challenge.jpg
Enter passphrase: 
wrote extracted data to "location.txt".
```


## 3. Getting the flag

By reading either of the 2 outfiles that we dumped, we can get the content of it which is a coordinate that also acts like an password:

>20.899370,95.118041,16

Now extract the zip and get the card

```
https://bit.ly/3eMaV0v
```