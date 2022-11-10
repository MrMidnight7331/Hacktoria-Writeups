# The Butcher (Easy)

> MrMidnight

-----------------------------

### Intro TEXT

```
Greetings, Special Agent K. As you might have heard in the news over the past few months. The city of Berlin in Germany is being plagued by a serial killer, nicknamed “The Butcher”.

As the name implies, this individual butchers his victims and disposes their body parts all over the city. Autopsy reports conclude that the weapon for disposal is most likely a meat cleaver.

The total body count currently sits at 18 people, mostly women and younger men. All victims were traveling alone at night, mostly through quiet areas, when they were last seen.

Fortunately, yesterday the German police raided an apartment in the city center of Berlin. Neighbors had complained about a stale, metal like smell coming from the apartment. Upon closer inspection, the police found large quantities of plastic sheets, blood traces of several victims and an assortment of meat cleavers.

Since the apartment was rented out to an individual who had used a fake ID, the police has hit a dead end in trying to find the killer. They did however retrieve several files from a personal laptop, including a large, encrypted archive.

In the same location as the archive was stored, a file named “password” was found. However, this just contained a bunch of HEX values. We need you to make sense of this file, perhaps it leads to the password for the archive.

As always, Special Agent K. The contract is yours, if you choose to accept.
```

## 1. Get the assets

We are given a link file and a password file:

Download the linkfile
Download the password file:

```bash
wget https://hacktoria.com/wp-content/contracts/items/password-the-butcher
```

## 2. Cracking the hash
The password we were given is encoded in "Hex" we can decode it by using [CyberChef](https://gchq.github.io/CyberChef/#recipe=From_Hex('Auto'))

 Output of the decoding isnt human readable. But we can use "Detect file type" module to decect what kind of file it is:

```
File type:   MPEG-3 audio
Extension:   mp3
MIME type:   audio/mpeg
```

Knowing that its a mp3 file, lets save the output from hex and name it voice.mp3

## 3. Getting the flag
We can use a mediaplayer like "vlc" to play the mp3. By listening to the audio, we  can write down letters by letters which is the password for the linkfile zip:

```
fgjkaergnadrmgkhngadrgle
```

```
https://bit.ly/3EyudkI
```