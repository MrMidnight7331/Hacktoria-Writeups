
# Lost at Sea (Easy)
> MrMidnight

-------------------

### Intro TEXT

```
Greetings Special Agent K. Yesterday at exactly 22:34 EET we lost contact with our surveillance ship “Narwhal”. A distress signal was sent out, right after this all communication was lost. The Narwhal was operating in the Black Sea, keeping an eye on Russian submarine and aerial activity.

Although she looks like a regular fishing trawler, the Narwhal, built in 2018, was outfitted with state of the art equipment. Housing a crew of 10, including a 4 PAX intervention unit of our best and brightest from the H.M.I.U (Hacktoria Maritime Intervention Unit).

Our allies in the British Royal Navy were kind enough to respond immediately. They were able to retrieve the Narwhals’ distress beacon. This is a device that automatically logs the last ten event, using the many sensors on board. This quick log entry is written to the SD card inside a waterproof tube, outfitted with a flotation device and GPS beacon. After the data is written, the beacon ejects and keeps afloat on the surface.

This prevents any signal delay from external antennas not being fast enough. Now, there’s a catch with this beacon. The log-file is written to an encrypted archive. The password for this log-file is set by the captain and communicated over encrypted channels, changing daily to prevent enemy forces capturing the correct code.

Somehow, the signal was lost right before the captain was able to relay the new password. This is human error, the password would normally be communicated right before being changed. This leaves us with our current situation. We don’t know the password, you’ll have to find a way to unlock the log-file.

This will give us insight into how the Narwhal sunk and allow us to begin the recovery. Given the hostile situation, it’s imperative we find the exact location of the Narwhal.
```

## 1. Download assets
Download the Ship Logbook file

## 2. Analyze Intro
So I tried using classic tools like zip2john or hashcat but it doesnt seem to work. The solution must be somewhere else, but since we are given an "Intro Text" we should  analyze that.

After im done reading the text ive noticed that  "Narwhal" is the ships name and was build in 2018. Maby the password is the name of the ship. The text also stated a clue: "Somehow, the signal was lost right before the captain was able to relay the new password. This is human error". Which supports the idea of having the solution in the text.

## 3. Getting the flag
The password is:

>Narwhal2018

```bash
cat datadump-probe
```

```
LOCATION:       44.470394, 32.264429
HEADING:        NNE 32
SPEED KN:       7 knots
SPEED KMPH:     12,964
EVENT 01:       DETECTED SE 132 3.00S
EVENT 02:       INCOMING SE 132 2.51S
EVENT 03:       INCOMING SE 132 2.15S
EVENT 04:       WARNING IMPACT SE 132 1.45S
EVENT 05:       WARNING IMPACT SE 132 1.25S
EVENT 06:       IMPACT IMMINENT SE 132 USET-80
EVENT 07:       IMPACT IMMINENT SE 132 USET-80
EVENT 08:       WRITING DATADUMP TO DISK
EVENT 09:       EJECTING PROBE BEACON KMZ784S
EVENT 10:       STLK UPLOAD https://bit.ly/3DVvwJM
```

```
https://bit.ly/3DVvwJM
```