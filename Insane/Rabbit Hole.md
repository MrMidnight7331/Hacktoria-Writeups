# Rabbit Hole (Insane)
> MrMidnight

-----------------------------------------

### Mission Briefing:

```
Greetings Special Agent K. Today we have a special Contract. At the time of writing, 06.12.2022 at 19:48 EET, Hacktoria is now one year old. The first ever Monthly Capture the Flag event was announced roughly one year ago, between 06 and 15.12.2021. Meaning this was the week that the idea for “Story Driven OSINT Capture the Flag Exercises” was born.

To thank everyone who’s been a part of this journey and celebrate the birthday of Hacktoria, I present you with the “Rabbit Hole” Contract. The name stems from the OSINT term “Rabbit Hole”, where the investigator chases after suspected leads and clues, not knowing if or where they will end. Or… If they’re even real.

This Contract will take you through almost all disciplines covered in Hacktoria events and Contracts so far, with the inclusion of some new concepts as well. Only limited by the exclusion of steps that would be too fragile to stay online permanently. For example, the art gallery in the Mona Lisa Heist, would be too unpredictable for a permanent Contract. As a guideline, I can say this Contract is comprised of 10 steps in total. Various steps will hint to where you are, using the step number in filenames.

With the first step for this Contract, I present you the first ever complete archived screenshot of the Hacktoria website. Made on 15.12.2021 at 14:04:04. I hope you enjoy this Contract, and all those to come in the future. Thank you for being part of this.

As always, Special Agent K. The Contract is yours, if you choose to accept.
```
### Extras:
```
Password instruction flagfile:

-   Species from step 03
-   Social handle from step 06
-   Username from step 08
-   Country and Streetname from step 10

Example password:

galeocerdo-cuvier-dodgy_malaka08-logmein-germany-hamburger-d-strasse
```

## 0. Download assets

Download the original Image


## 1. Step

If we examin the given image correctly, we will find a URL at the bottom coner:

```
hacktoria.com/wp-content/contracts/items/rabbithole/dmehuf/step2.zip
```

## 2. Step

Extract the zip file and we will recieve a text file, containing the following hash:

```
(9:=6 :? 2 D6?D6 6249 >@C?:?8 >2C<D E96 368:??:?8 @7 Q2 ?6H 52JQ J6E[ 2D E9:D =2DE J62C 92D D@F?565 E96 562E9 <?6== @7 2? 6C2 5:D2DEC@FD E@ E96 H6=72C6 2?5 92AA:?6DD @7 >2?<:?5 :? >2?J H2JD[ D@ E96 }6H *62C ;FDE 52H?:?8 AC@>:D6D 2? 6A@49 @7 F?A2C2==6=65 6?=:89E6?>6?E 2?5 @AA@CEF?:EJ 7@C >2?<:?5 E@ C64@FA 9:D =@DD6D DF776C65 E9C@F89 :8?@C2?46[ @C H:==7F= 2?5 56=:36C2E6 DF3DE:EFE:@? @7 >2?VD 32D6 56D:C6D 2?5 56DECF4E:G6 H:== 7@C E96 s:G:?6 (:== 2?5 !6C764E !=2? @7 v@5[ 9:D rC62E@CP (62C:=J 5C:G6]8@@8=6]4@> 92G6 E96 52JD 5C28865 3J[ H9:=6 A=@ED 2?5 4@F?E6C A=@ED 4@>A=:42E65 2?5 >F=E:A=:65 >2?VD F?D@=G23=6 AC@3=6>D] (6 92G6 H2E4965 H:E9 2 9@CC@C :>A@DD:3=6 E@ C6AC6DD[ >2?VD :?67764EF2= 2EE6>AED E@ 6IEC:42E6 9:>D6=7 7C@> E96 EC62496C@FD BF:4<D2?5D @7 5646AE:G6 Q28C66>6?EDQ 2446AE65 :? 2AA2C6?E 8@@5 72:E9[ @?=J E@ 36 CFE9=6DD=J EC2>A=65 F?56C 7@@E H96? E96:C 6G:= AFCA@D6 92D 366? 249:6G65]

V2h5IGRvIHdlIHNheSB0aGUgdGlkZSBoYXMgbm93IHR1cm5lZD8gQmVjYXVzZSBhbGwgbWFua2luZCBlbnNsYXZlZCBvciBzdGlsbCBjYXBhYmxlIG9mIHJlY292ZXJpbmcgdGhlaXIgbG9zdCBoZXJpdGFnZSBvZiBmcmVlZG9tIGJlZ2luIHRvIHNlZSBmb3IgdGhlbXNlbHZlcyB0aGUgZW5vcm1pdHkgb2YgdGhlaXIgZm9sbHkgaW4gdHJhbnNncmVzc2luZyBsYXdzIGFsbC1wb3dlcmZ1bCB0byBwcm9tb3RlIHRoZWlyIHBlcnNvbmFsIHByb2dyZXNzIGFuZCBjb25zZXF1ZW50IHBvc3Nlc3Npb24gb2YgYWxsIHRoZXkgbW9zdCBlYXJuZXN0bHkgbmVlZCBhbmQgZGVzaXJlISBXaGVuIHdpbGwgTWFuIGNlYXNlIGhpcyByaWRpY3Vsb3VzIGF0dGVtcHRzIHRvIG9ic3RydWN0IHRoZSBvcmRlcmx5IHByb2Nlc3NlcyBvZiBwcm9ncmVzc2l2ZSBkZXZlbG9wbWVudCBhcyBzZXQgaW4gbW90aW9uIGF0IHRoZSBjb21tZW5jZW1lbnQgb2YgaGlzIHNvam91cm4gb24gdGhlIHBsYW5ldCBTaGFuPyBUaGUgYW5zd2VyIGlzIGFic3VyZGx5IHNpbXBsZSEgL2RyaXZlL2ZvbGRlcnMgV2hlbiBoZSBhY2tub3dsZWRnZXMgdG8gaGltc2VsZiB0aGF0IGhpcyBwdW55IGJyYWluIGFuZCB1bnJ1bHkgaW1wdWxzZXMgY29uc3RpdHV0ZSBubyByZWxpYWJsZSBndWlkZSB0byB0aGUgYWNxdWlzaXRpb24gb2YgdGhvc2UgdGFuZ2libGUgYW5kIGludGFuZ2libGUgYXNzZXRzIHdpdGhvdXQgd2hpY2ggaGUgY2Fubm90IGhvcGUgdG8gZXNjYXBlIGEgbW9zdCB0ZXJyaWZ5aW5nIGZhdGUhIE1pZ2h0IHdlLCB3aG9tIHlvdSBoYXZlIG5hbWVkICJTcGFjZSBNZW4sIiBzaGFyZSB3aXRoIHlvdSB0aGUgYWN0dWFsLCBwcm92YWJsZSBmYWN0cyB3ZSBoYXZlIGJlZW4gYWJsZSB0byBkaXNjb3ZlciBieSBleHBlcmltZW50IGFuZCBleHBlcmllbmNlIGluIHRha2luZyBwcmVjaXNlbHkgdGhlIG9wcG9zaXRlIGNvdXJzZSBvZiBhY3Rpb24gdG8gdGhhdCBmb2xsb3dlZCBieSB0aGUgbWFqb3JpdHkgb2YgZWFydGggZHdlbGxlcnM/

IFRGOIDPNBTSA2TVNZTSAZ3VOJSXEIDVNZUXEIDPOJZGCIDBNB5HEZLCNBTCAZLOMZ2SA3THM5ZHUY3HMYQHU3TROIQG63BAOZQXA3TIM53GE2DGEBXXE6LWOJUXEZLGEB3GCICROZUXMYLSEBLGCZ3SPF4XM5DSMFYHELBAJJ3GM4LCPIQG4YLREBIGK4TOM53GS4RAKZQXI4TBNB3GO3BAM5RCA3TZOZ2GCIDHOVZHMZJAPF3GS4TGEBVHMZ3VEBTXK5TGEBTGQY3FOJ5HEIDHMV3GQ6TJOZSW4Z3SEBXWQZZAM5RCA2TVNZTSA3TJNZ3HSPZALJXGC6DWMFYSA5TBEB2HEYLSMVXHSIDKMJUHS4JAOVXGS4RAMFRGC4RAMJZSAZ3VOJ5CCICHOVZHMZJAONXGO4RAOZTCA3TZPEQGOYTCEBVHE6LZEB4GCYTKMEQGOYRANRRGQIJAIZ2W46LZEBVHEIDGOVXGK4RAM52W4ZZAONXGO4R7EBAUEIJAKZTSA5TGEBRGQZJANZUWE2TSOEQHMYLHOJQWO5TCMEQGOYRANZYGI2DOOZQWOIDMMJUCA2TWM52SAZ3VOIQGK4TGNB4WOZRAMJXWO3TWMFZHCIDHOVSWE2DUOUQGO5LSEBYGEYLGOZTGO4TBM4QG4YLREBRXEZLGOZTGO4TBM4QGQZTSEB3GCIDOEBYGEYLGM5SWQ4DHOZUXEIDKNZWCAYTTEBTXK4RANFZGK3BAONRGK4DSMYQGYYTIEB2W42LSEBUGM4TREBTWEIDROJTGOZLCNQQHE2LSMVWGO5LWMF2CA5DCMJYSA3TBOEQG64TONBTXM43IPEQG4YLREBQWE2RAOZQWM3TBOJ4WYIDDPFXGCIDHMIQHE6TDPFRGYIDHMIQHAYT2PJ3GOIDGNB3HA5TROIQGEYJANYQHI6LCN5XHSIDGOBXHS4RBEBBGQZJAOVRHU4TGEBXGK4RAN5UHM6LHEBTWEIDDMVRGS5TROIQHAYT2ONRGKZ3GEBSGQ5THOIQG64TMMJQXCIDMMJUGKIDRMVZG46TGEBRHGIDZNBVWQZLMEBUGC3THM5XHMYLON54XEIJAI52XE5TFEBYG4ZLSEB3GMIDOEBYXE6LWOR2WOLBAONRGKIDHOVZGK4RAOZTCAYLCEBYWK2DRORZGK3BBEBJGCZ3SMVTW45TBOZQXIIDUNBZGMZ3GEB3GMIDFMJXW64TREBRHGIDOPF4SA5THMYQGGZLCN54XE6TGEBTG42LSEBTXK4RAMN4XE3TGNBSXEIDCOMQHC4TJOZTHMYLUEBZWK4TGOUQGG6LOMFTCA43CMUQGO5LSOZSSA4TBO5RGY6TSMFTS4IBIKYQHU5TUOVTSA3TROEQGO5LSNQQHEYLHOJSSA5TBM5RCA3TZPEQGM2DQOUQGG6LOMFTCA2TWM52SA3LSMZTSCKJAF4YU4T3VKBGTCTTZIR4GUMRQGB4UQQ3VPFPVELLSNBEVKS3IKV2FESRAJZ4XSIDCNBSSA4TRNBYG4Z3WMJQW46JAONXHA5TZOZTXM4TGEBXGK4RAOJQWO5TFOJ4WYIDTMVZHELBANZQXCIDGMIQGS3TFOZZHCIDOMVZCAZ3VOIQG6ZLOMFYHK4TGEBRHGIDGM5UHC3BANZQXCIDDMVXHAZ3WOBXHSIDOMNRXS5TQNZTXMYTBEBTXK3THEBQWEIDGM5UHC4TBM4QHK3TGEBZGS4TFEBZW45TZOJYSAZ3CEBZXMYLREBRWK4TQOZTHE6LMEBTXK4RAM5WGG4RAMJZSA5TBMZTWK2DQM53GEYJAN5ZGMZZAMZUHMZ3SOEQGOYRAOV3GMIDDNZSWO5TQNB4W4ZJAN5ZGCZZANZQXCIDON53HS5THNQXCAQ3FOZTGEYLGFQQGK4TTMJSXUIDGOB2WEYTZMYWCA5TBMZTXMZ3IM5ZGMIDTMJSSAZ3VOIQHMYLGNZQXEIBINRZGMLBAOJUXEYJAOVRGMY3WM5XHSZRJEBXGK4RANBQXQYLCNJQS4ICHOVZGYIDKMJUHS4JAN5ZCA2DBMJYHA2DDOZZHCLRAKVXGS4RAM52XEZTSEBXGC4JAOZQWC2D2OJSW433ZOIQGEZ3VOJSSAITKMJQXC4TFMYRCA4DCPJZCA3TPMJUGOIDHOVSWE2DUOUQGMYT2OIQGMYTFM4QGE4ZAPJXHI5TQH4QE63BAMFRCA6TSNZQWMIJAJJZCA5LONFZCA2TCMV4HE4JAM52XE6RAMJUGOIJAJJ2XEZLSEBYXM4JANJZCA5DSM4QGE2DFEB3GCZTHMVUHAZ3WMJQWMPZAKNSWE6RAM52XEIDGOJ4XGZTOPJZCARTCNBSXA4RANJ2XM4DVEB3GMIDONFXHM6LON54XEIDHMIQGYYTIFYQFMIDKOZ4XSIDHOJ4XSIDMMJUCA6TCMVZCAZTVMJUHS4JANRRGQIDQNZSXEIDHMIQHQYLCNIXA====
```


By using CyberChef, we can decode the hashes given.

The first part: 

```
(9:=6 :? 2 D6?D6 6249 >@C?:?8 >2C<D E96 368:??:?8 @7 Q2 ?6H 52JQ J6E[ 2D E9:D =2DE J62C 92D D@F?565 E96 562E9 <?6== @7 2? 6C2 5:D2DEC@FD E@ E96 H6=72C6 2?5 92AA:?6DD @7 >2?<:?5 :? >2?J H2JD[ D@ E96 }6H *62C ;FDE 52H?:?8 AC@>:D6D 2? 6A@49 @7 F?A2C2==6=65 6?=:89E6?>6?E 2?5 @AA@CEF?:EJ 7@C >2?<:?5 E@ C64@FA 9:D =@DD6D DF776C65 E9C@F89 :8?@C2?46[ @C H:==7F= 2?5 56=:36C2E6 DF3DE:EFE:@? @7 >2?VD 32D6 56D:C6D 2?5 56DECF4E:G6 H:== 7@C E96 s:G:?6 (:== 2?5 !6C764E !=2? @7 v@5[ 9:D rC62E@CP (62C:=J 5C:G6]8@@8=6]4@> 92G6 E96 52JD 5C28865 3J[ H9:=6 A=@ED 2?5 4@F?E6C A=@ED 4@>A=:42E65 2?5 >F=E:A=:65 >2?VD F?D@=G23=6 AC@3=6>D] (6 92G6 H2E4965 H:E9 2 9@CC@C :>A@DD:3=6 E@ C6AC6DD[ >2?VD :?67764EF2= 2EE6>AED E@ 6IEC:42E6 9:>D6=7 7C@> E96 EC62496C@FD BF:4<D2?5D @7 5646AE:G6 Q28C66>6?EDQ 2446AE65 :? 2AA2C6?E 8@@5 72:E9[ @?=J E@ 36 CFE9=6DD=J EC2>A=65 F?56C 7@@E H96? E96:C 6G:= AFCA@D6 92D 366? 249:6G65]
```
Has been encoded in ROT47

The second part: 

```
V2h5IGRvIHdlIHNheSB0aGUgdGlkZSBoYXMgbm93IHR1cm5lZD8gQmVjYXVzZSBhbGwgbWFua2luZCBlbnNsYXZlZCBvciBzdGlsbCBjYXBhYmxlIG9mIHJlY292ZXJpbmcgdGhlaXIgbG9zdCBoZXJpdGFnZSBvZiBmcmVlZG9tIGJlZ2luIHRvIHNlZSBmb3IgdGhlbXNlbHZlcyB0aGUgZW5vcm1pdHkgb2YgdGhlaXIgZm9sbHkgaW4gdHJhbnNncmVzc2luZyBsYXdzIGFsbC1wb3dlcmZ1bCB0byBwcm9tb3RlIHRoZWlyIHBlcnNvbmFsIHByb2dyZXNzIGFuZCBjb25zZXF1ZW50IHBvc3Nlc3Npb24gb2YgYWxsIHRoZXkgbW9zdCBlYXJuZXN0bHkgbmVlZCBhbmQgZGVzaXJlISBXaGVuIHdpbGwgTWFuIGNlYXNlIGhpcyByaWRpY3Vsb3VzIGF0dGVtcHRzIHRvIG9ic3RydWN0IHRoZSBvcmRlcmx5IHByb2Nlc3NlcyBvZiBwcm9ncmVzc2l2ZSBkZXZlbG9wbWVudCBhcyBzZXQgaW4gbW90aW9uIGF0IHRoZSBjb21tZW5jZW1lbnQgb2YgaGlzIHNvam91cm4gb24gdGhlIHBsYW5ldCBTaGFuPyBUaGUgYW5zd2VyIGlzIGFic3VyZGx5IHNpbXBsZSEgL2RyaXZlL2ZvbGRlcnMgV2hlbiBoZSBhY2tub3dsZWRnZXMgdG8gaGltc2VsZiB0aGF0IGhpcyBwdW55IGJyYWluIGFuZCB1bnJ1bHkgaW1wdWxzZXMgY29uc3RpdHV0ZSBubyByZWxpYWJsZSBndWlkZSB0byB0aGUgYWNxdWlzaXRpb24gb2YgdGhvc2UgdGFuZ2libGUgYW5kIGludGFuZ2libGUgYXNzZXRzIHdpdGhvdXQgd2hpY2ggaGUgY2Fubm90IGhvcGUgdG8gZXNjYXBlIGEgbW9zdCB0ZXJyaWZ5aW5nIGZhdGUhIE1pZ2h0IHdlLCB3aG9tIHlvdSBoYXZlIG5hbWVkICJTcGFjZSBNZW4sIiBzaGFyZSB3aXRoIHlvdSB0aGUgYWN0dWFsLCBwcm92YWJsZSBmYWN0cyB3ZSBoYXZlIGJlZW4gYWJsZSB0byBkaXNjb3ZlciBieSBleHBlcmltZW50IGFuZCBleHBlcmllbmNlIGluIHRha2luZyBwcmVjaXNlbHkgdGhlIG9wcG9zaXRlIGNvdXJzZSBvZiBhY3Rpb24gdG8gdGhhdCBmb2xsb3dlZCBieSB0aGUgbWFqb3JpdHkgb2YgZWFydGggZHdlbGxlcnM/
```
Has been encoded in BASE64

The last part: 

```
IFRGOIDPNBTSA2TVNZTSAZ3VOJSXEIDVNZUXEIDPOJZGCIDBNB5HEZLCNBTCAZLOMZ2SA3THM5ZHUY3HMYQHU3TROIQG63BAOZQXA3TIM53GE2DGEBXXE6LWOJUXEZLGEB3GCICROZUXMYLSEBLGCZ3SPF4XM5DSMFYHELBAJJ3GM4LCPIQG4YLREBIGK4TOM53GS4RAKZQXI4TBNB3GO3BAM5RCA3TZOZ2GCIDHOVZHMZJAPF3GS4TGEBVHMZ3VEBTXK5TGEBTGQY3FOJ5HEIDHMV3GQ6TJOZSW4Z3SEBXWQZZAM5RCA2TVNZTSA3TJNZ3HSPZALJXGC6DWMFYSA5TBEB2HEYLSMVXHSIDKMJUHS4JAOVXGS4RAMFRGC4RAMJZSAZ3VOJ5CCICHOVZHMZJAONXGO4RAOZTCA3TZPEQGOYTCEBVHE6LZEB4GCYTKMEQGOYRANRRGQIJAIZ2W46LZEBVHEIDGOVXGK4RAM52W4ZZAONXGO4R7EBAUEIJAKZTSA5TGEBRGQZJANZUWE2TSOEQHMYLHOJQWO5TCMEQGOYRANZYGI2DOOZQWOIDMMJUCA2TWM52SAZ3VOIQGK4TGNB4WOZRAMJXWO3TWMFZHCIDHOVSWE2DUOUQGO5LSEBYGEYLGOZTGO4TBM4QG4YLREBRXEZLGOZTGO4TBM4QGQZTSEB3GCIDOEBYGEYLGM5SWQ4DHOZUXEIDKNZWCAYTTEBTXK4RANFZGK3BAONRGK4DSMYQGYYTIEB2W42LSEBUGM4TREBTWEIDROJTGOZLCNQQHE2LSMVWGO5LWMF2CA5DCMJYSA3TBOEQG64TONBTXM43IPEQG4YLREBQWE2RAOZQWM3TBOJ4WYIDDPFXGCIDHMIQHE6TDPFRGYIDHMIQHAYT2PJ3GOIDGNB3HA5TROIQGEYJANYQHI6LCN5XHSIDGOBXHS4RBEBBGQZJAOVRHU4TGEBXGK4RAN5UHM6LHEBTWEIDDMVRGS5TROIQHAYT2ONRGKZ3GEBSGQ5THOIQG64TMMJQXCIDMMJUGKIDRMVZG46TGEBRHGIDZNBVWQZLMEBUGC3THM5XHMYLON54XEIJAI52XE5TFEBYG4ZLSEB3GMIDOEBYXE6LWOR2WOLBAONRGKIDHOVZGK4RAOZTCAYLCEBYWK2DRORZGK3BBEBJGCZ3SMVTW45TBOZQXIIDUNBZGMZ3GEB3GMIDFMJXW64TREBRHGIDOPF4SA5THMYQGGZLCN54XE6TGEBTG42LSEBTXK4RAMN4XE3TGNBSXEIDCOMQHC4TJOZTHMYLUEBZWK4TGOUQGG6LOMFTCA43CMUQGO5LSOZSSA4TBO5RGY6TSMFTS4IBIKYQHU5TUOVTSA3TROEQGO5LSNQQHEYLHOJSSA5TBM5RCA3TZPEQGM2DQOUQGG6LOMFTCA2TWM52SA3LSMZTSCKJAF4YU4T3VKBGTCTTZIR4GUMRQGB4UQQ3VPFPVELLSNBEVKS3IKV2FESRAJZ4XSIDCNBSSA4TRNBYG4Z3WMJQW46JAONXHA5TZOZTXM4TGEBXGK4RAOJQWO5TFOJ4WYIDTMVZHELBANZQXCIDGMIQGS3TFOZZHCIDOMVZCAZ3VOIQG6ZLOMFYHK4TGEBRHGIDGM5UHC3BANZQXCIDDMVXHAZ3WOBXHSIDOMNRXS5TQNZTXMYTBEBTXK3THEBQWEIDGM5UHC4TBM4QHK3TGEBZGS4TFEBZW45TZOJYSAZ3CEBZXMYLREBRWK4TQOZTHE6LMEBTXK4RAM5WGG4RAMJZSA5TBMZTWK2DQM53GEYJAN5ZGMZZAMZUHMZ3SOEQGOYRAOV3GMIDDNZSWO5TQNB4W4ZJAN5ZGCZZANZQXCIDON53HS5THNQXCAQ3FOZTGEYLGFQQGK4TTMJSXUIDGOB2WEYTZMYWCA5TBMZTXMZ3IM5ZGMIDTMJSSAZ3VOIQHMYLGNZQXEIBINRZGMLBAOJUXEYJAOVRGMY3WM5XHSZRJEBXGK4RANBQXQYLCNJQS4ICHOVZGYIDKMJUHS4JAN5ZCA2DBMJYHA2DDOZZHCLRAKVXGS4RAM52XEZTSEBXGC4JAOZQWC2D2OJSW433ZOIQGEZ3VOJSSAITKMJQXC4TFMYRCA4DCPJZCA3TPMJUGOIDHOVSWE2DUOUQGMYT2OIQGMYTFM4QGE4ZAPJXHI5TQH4QE63BAMFRCA6TSNZQWMIJAJJZCA5LONFZCA2TCMV4HE4JAM52XE6RAMJUGOIJAJJ2XEZLSEBYXM4JANJZCA5DSM4QGE2DFEB3GCZTHMVUHAZ3WMJQWMPZAKNSWE6RAM52XEIDGOJ4XGZTOPJZCARTCNBSXA4RANJ2XM4DVEB3GMIDONFXHM6LON54XEIDHMIQGYYTIFYQFMIDKOZ4XSIDHOJ4XSIDMMJUCA6TCMVZCAZTVMJUHS4JANRRGQIDQNZSXEIDHMIQHQYLCNIXA====
```

Has been encoded in BASE32 and ROT13.

The output should result a readable text:

```
While in a sense each morning marks the beginning of "a new day" yet, as this last year has sounded the death knell of an era disastrous to the welfare and happiness of mankind in many ways, so the New Year just dawning promises an epoch of unparalleled enlightenment and opportunity for mankind to recoup his losses suffered through ignorance, or willful and deliberate substitution of man's base desires and destructive will for the Divine Will and Perfect Plan of God, his Creator! Wearily drive.google.com have the days dragged by, while plots and counter plots complicated and multiplied man's unsolvable problems. We have watched with a horror impossible to repress, man's ineffectual attempts to extricate himself from the treacherous quicksands of deceptive "agreements" accepted in apparent good faith, only to be ruthlessly trampled under foot when their evil purpose has been achieved.

Why do we say the tide has now turned? Because all mankind enslaved or still capable of recovering their lost heritage of freedom begin to see for themselves the enormity of their folly in transgressing laws all-powerful to promote their personal progress and consequent possession of all they most earnestly need and desire! When will Man cease his ridiculous attempts to obstruct the orderly processes of progressive development as set in motion at the commencement of his sojourn on the planet Shan? The answer is absurdly simple! /drive/folders When he acknowledges to himself that his puny brain and unruly impulses constitute no reliable guide to the acquisition of those tangible and intangible assets without which he cannot hope to escape a most terrifying fate! Might we, whom you have named "Space Men," share with you the actual, provable facts we have been able to discover by experiment and experience in taking precisely the opposite course of action to that followed by the majority of earth dwellers?

Not but what there have been numerous rash attempts made by incautious believers in Divine Intelligence, Wisdom and Creative Ingenuity to align their lives with this supreme triumvirate but to what avail? Mankind in general would have none of them! Their fate is all too well known to you! Shall we share that fate? NO! It is our avowed intention to acquaint you with the results obtained through the consistent and persistent use in a constructive way of the very forces you have used to destroy everything good and beautiful and now insanely plan to employ to commit suicide on a global scale! Our homes are built to provide comforts quite beyond your dreams of luxury unattainable! Their care is a delight, for there is no drudgery! Entertaining guests is robbed of all its problems save the pleasure of devising fresh plans for their enjoyment. (I might add they enter into all such plans with zest!) /1ABhCZ1AlQkw200lUPhl_E-euVHXuHgEW All our educational facilities are entirely free, and so varied are the branches of study and practical application that no student has ever failed to find precisely the type of instruction best suited to his particular bent and ability. Prisons, reform schools, institutes for the insane (yes, even hospitals) are unknown. They would be unoccupied. Have these and innumerable other "wonders" come about through some sort of magic? By no means! We have worked them out! Where did we get our instructions? From the selfsame Source which is available to you. I will tell you more should you care to know.

```

Analyzing the text, we can find some interesting strings, which pieces together into a google drive link:

```
drive.google.com
/drive/folders
/1ABhCZ1AlQkw200lUPhl_E-euVHXuHgEW

https://drive.google.com/drive/folders/1ABhCZ1AlQkw200lUPhl_E-euVHXuHgEW
```

Go to the URL and download the files for step 3 and 4


## 3. Step
We've got a image file after unzip the zip. In the password instruction, it tells us to find the species of this shark. 

By using some google lense, we can find this link: https://reefguide.org/pixhtml/reefshark24.html. On that website we see the name of this shark: "Caribbean Reef Shark" and its scientific name on the left top corner: "Carcharhinus Perezi"

>carcharhinus-perezi


## 4. Step
The zip file here requires a password, which is the result of step3: "carcharhinus-perezi". We should get an pcapng file after the unzipping.

For the analyze of this pcap file, I will use "Wireshark": 

```bash
wireshark ./step-04-pcap-fvcweium.pcapng
```

What we are trying to find, is some kind of zip file or either a google drive link, or a hacktoria link.

I will filter the request by ftp-data. This results me to find a zip file:

```
Frame 2692: 2950 bytes on wire (23600 bits), 2950 bytes captured (23600 bits) on interface enp0s3, id 0
Ethernet II, Src: RealtekU_12:35:02 (52:54:00:12:35:02), Dst: PcsCompu_e2:ce:7c (08:00:27:e2:ce:7c)
Internet Protocol Version 4, Src: 161.35.213.127, Dst: 10.0.2.15
Transmission Control Protocol, Src Port: 48798, Dst Port: 55084, Seq: 1, Ack: 1, Len: 2896
FTP Data (2896 bytes data)
[Setup frame: 2680]
[Setup method: PASV]
[Command: RETR /fkf434j3vgty4y64y4.zip]
Command frame: 2684
[Current working directory: ]
```



To export this we will start by right click on the first request, follow tcp-stream, show data as "raw" and export as "output-04-05.zip"

## 5. Step

The unzipped file is again a image file. This is the first rabbithole. We dont need to find the place on the image at all. The reason of that is, there is a hidden file hidden in this image. To check and crack the potential hidden files password, we can use "stegseek":

```
stegseek image-step-05-fkgvdgfdmw.jpg 
cat image-step-05-fkgvdgfdmw.jpg.out
```

The content of the output-file is the following: 

```
We hear the former head of Hackoria / Tiberian Order's HUMINT team likes to post on social media.
```


## 6. Step

Step5 reveals that a former head of hacktoria form the "Tiberian Order's HUMINT" team, really likes to tweet on social media. Since the "Tiberian Order's HUMINT" was in the past, ill use the "wayback machine" to search for a older version of hacktoria.

I found a snapshot on the 15th December 2011: https://web.archive.org/web/20220126051123/https://hacktoria.com/

Viewing their [the-team](https://web.archive.org/web/20220126051123/https://hacktoria.com/the-team/)page, at the bottom, we find a person named Julia Sharpe, with a description that matches our target:

```
Lead for the Tiberian Serpent FIELD HUMINT Team Operations.
```

Underneath that is a twitter link: https://web.archive.org/web/20220129074649/https://twitter.com/julesshapry confirming that this person has an twitter account. So searching for "Julia Sharpe" on twitter, we are able to find her current [account](https://twitter.com/julia_sharpe007), with a encoded BASE32 message: 
```
NB2HI4DTHIXS62DBMNVXI33SNFQS4Y3PNUXXO4BNMNXW45DFNZ2C6Y3PNZ2HEYLDORZS62LUMVWXGL3SMFRGE2LUNBXWYZJPNJTWI53WNVZWYZRPORXW63DTFVZXIZLQFUYDOLLGM5XGW43RNJVXCLT2NFYA
```

which decodes to: 
```
https://hacktoria.com/wp-content/contracts/items/rabbithole/jgdwvmslf/tools-step-07-fgnksqjkq.zip
```

We ofcourse note down the persons twitter username, for the card-file:
>julia_sharpe007

## 7. Step

Download and unzip the file, reveals ton of python scripts. Since we are searching for either zip, hacktoria, or google drive strings, ill use cat and grep to find it: 

```bash
cat *.py | grep google
```

indeed we found a google drive link:

```
https://drive.google.com/drive/folders/1NhNYUalh1knesoJyD4EV5ikfHscYIKkQ
```

## 8. Step

This step requires us to set up a vm. Ill just use "VirtualBox" for this. First import the ova file and just start the machine. Meanwhile we can take a look at the password-hint.txt that we are given besides the ova: 

```
The one I always use ending in 123 and starting with a capital P..
```

The password is obviously "Password123". When the machines has booted, we can see that its hostname is called "zayed-svr". Since we are missing the username, I wildly guess "zayed". Suprisingly it worked! 

The home directory didnt contain anything useful. By checking the users privilege: "sudo -l" we can see that this user has root privilege:

```bash
sudo su
cd /root
```

Further informations are located in the ".bash_history" file. 

The content says that the user created a file called .vboxm by using the vim text editor, in the /media folder. So lets go into the /media folder and check out the created file:

```bash
cd /media
cat /.vboxm
```

This file reveals a link:

```
https://hacktoria.com/wp-content/contracts/items/rabbithole/bfgiunfummjh/image-step-09-sdffwacff.zip
```

We also need to take note of the username for the card-file:
>zayed

## 9. Step

Download and extract the file reveals yet another image file. This image shows a stone-tablet with the language of Klumgongyn written on it. If you translated the language, you'll be falling into the second rabbithole. All you have to do is to "string" the file which reveals a BASE32 string:
```
NB2HI4DTHIXS62DBMNVXI33SNFQS4Y3PNUXXO4BNMNXW45DFNZ2C6Y3PNZ2HEYLDORZS62LUMVWXGL3SMFRGE2LUNBXWYZJPMRUGO3DXMVZG2L3HNIZDGNBYGUZWU43FMY2DGNJOPJUXA===
```

It decodes to an link:

```
https://hacktoria.com/wp-content/contracts/items/rabbithole/dhglwerm/gj234853jsef435.zip
```

Note tho that the extracted zip also revelas a file called name.txt containing the following:

```
HaakonVMagnusson
******V*********
```

## 10. Step

The downloaded zip do require a password, which is coincidentally the content of name.txt: "HaakonVMagnusson". A image file has been extracted.

I tried a lot of methods in the hope of finding the image but non worked. So I bought a intel from the hacktoria discord:

```
step 01 - it's in the little details 
step 02 - three different ciphers, section 3 is 2 ciphers 
step 03 - something about coral 
step 04 - files get transfered 
step 05 - mentioned on old versions of the website 
step 06 - internet archives, make sure you get the right version 
step 07 - comments matter 
step 08 - the username is in the machine name 
step 09 - norway... step 10 - aeropuerto internacional de zihuatanejo
```

"aeropuerto internacional de zihuatanejo" which translates to zihuatanejo international airport in spanish: https://www.google.com/maps/place/Aeropuerto+Internacional+de+Zihuatanejo/@17.6061676,-101.4658999,17z/data=!3m1!4b1!4m5!3m4!1s0x84347711101fd133:0x29ea518bde157f25!8m2!3d17.6061676!4d-101.4637112

This airport is located in mexico. I then searched the area and found the exact location of the image that has been taken: https://www.google.com/maps/@17.6403457,-101.5630311,3a,43.4y,109.89h,88.05t/data=!3m6!1e1!3m4!1s2C2zjkHFmqq3UnAszQyUpQ!2e0!7i16384!8i8192 

The street we are suppost to search is called: "Av Jose Maria Morelos Y Pavon"

## 11. Getting the card
Puzzeling step 3, step 06, step 08 and step 10 we get the following:

>carcharhinus-perezi-julia_sharpe007-zayed-mexico-av-jose-maria-morelos-y-pavon

Now unzip the file and get the card