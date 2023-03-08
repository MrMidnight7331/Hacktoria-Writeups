# ChessMaster
> MrMidnight

-----------------------------------------

### Prologue:
```
This man is a genius. Not because his elo score is at a Chess Grand Master level, but it is about his spy competences. Trained by the bests, his skills outperform every opponent, on the board or on the field. Every tournament he played was screened by our agency, but we didn’t catch his operating mode. This man is clean at first sight. But there’s always a flaw, a little glitch and all the cover disappear in one finger snap.
```


### Mission Briefing:

```
Another message came from the HQ. A top secret has been stolen. Intelligence Service is confident that the “Chessmaster” will be the messenger next days. Nothing unusual about this man, he played chess online for training. But we need to know where the exact location of the transaction will occurs in order to set a interception team. We send you the link of his last chess game record. He was playing the Black and he wins (as usual) https://lichess.org/HENhcRIn
```
### Extras:
```
The password of the Flagfile is the What3Word of the location of the exchange.

Password sample for flagfile: bubble-mobile-car
```

## 1. Download assets

Download the flagfile 
Open the given link

## 2. Chess game

The link given leads us to a chess game on "linchess". First I thought message was hidden inside a chat message like on "chess.com" or something similiar. But then I realized that it could probably be some kind of cipher. Thats led me to google for "chess cipher":

https://incoherency.co.uk/chess-steg/

## 3. Decode

So I then downloaded the PGN of the game: https://lichess.org/game/export/HENhcRIn?evals=0&clocks=0

And copied the moves into the decoder:

```PGN
1. g3 Nf6 2. b4 b5 3. Bh3 g6 4. Bg2 h5 5. c3 Ba6 6. Qa4 Ng4 7. a3 f5 8. Bxa8 Bh6 9. Bg2 Bf8 10. h4 Kf7 11. f3 Nh2 12. Kf2 Kg8 13. c4 Nf1 14. d4 Rh7 15. Be3 c6 16. Ra2 Qc8 17. Bxf1 Rh8 18. Rh3 Bh6 19. Qxb5 Kf7 20. Qa5 Bb7 21. Qc7 Qd8 22. Qa5 Kf8 23. Ke1 e6 24. Bc1 d5 25. Rc2 Na6 26. Rc3 Be3 27. a4 Bf2+ 28. Kxf2 Qc7 29. Qxc7 Ke8 30. Qg7 g5 31. Ke3 Bc8 0-1
```

It reveals a link: https://justpaste.it/ThE_K1nG_1s_M4t

## 4. Geolocation

This link leads to a hidden message with a image:
```
As requested,

We will exchange the document just at side of this giant sculpture.

CM.
```

We can use image.google.com to reverse search the image, which comes out to be "word chess hall of fame": [rev-search](https://lens.google.com/search?p=AfVzNa_fpYa1CHMCWIfuz0Hs-DnBQG4psOHamsMpqQSStINjqs1wYt9qIMgfc2voR5qy6f2f67fB4LbVGjsB6qajU8fAO5SZgdP9LxmZ03J4qcF68DJZAmORhQuYaiH2eYtskAhMVCiu3FWmt4Mb0_jEno9R5JaN-xxlH7O91KVPDvdciNrGay2Uoq8W7OXeyhyqKrUfma2dOjIf1unQMSbrUHa8Wl0VRxs6owc-ewDmIpov8qvAE2uAL9K-sPeHiqX7EFmg25VqPyDMXFMnMfSiyMNvs5CG1mXa4C4JvwT4UMY%3D&ep=gisbubb&hl=en-DE&re=df#lns=W251bGwsbnVsbCxudWxsLG51bGwsbnVsbCxudWxsLG51bGwsIkVrY0tKR0UwTkRCa1l6RTRMVEZpTUdJdE5EZzRZUzA0Tm1SaUxUY3hNREF4WTJFMVpqWmhPQklmT0hwQ2VUTXpkakY2ZFZGaFVVUjFWV2RKVkUxaWJEVm5OMkZCY21KQ1p3PT0iXQ==). With this knowlage, I google the location of "world chess hall of fame": 4652 Maryland Ave #1, St. Louis, MO 63108, USA, and followed the instruction of using whats 3 words to locate the museum:
https://what3words.com/pines.linked.plug

## 5. Getting the password

In the message we got, we read that the password location is around the giant chess piece. Since 4 squares on w3w covers the piece, we have to try each one of them:

1. moth-gallons-press
2. slate-rather-hangs
3. pads-switch-patrol
4. pines-linked-plug

## 6. Getting the flag

The correct password is:
>moth-gallons-press

Now just open the zip and get the card


