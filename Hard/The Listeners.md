# The Listeners (Hard)
> MrMidnight

-----------------------------------------

### Mission Briefing:

```
Good day Special Agent K, glad you could make it. One of our oldest clients, a wealthy French businessman, is requesting we find a location where a conversation between two of his rivals will take place. These two have been after our clients’ fortune for a long time, endlessly scheming to end his business endeavors. After their recent attempt to sink one of our clients’ boats off the coast of Spain, while his wife and daughter were on board, our client has had enough.

The plan is to uncover the location of their meeting and have one of our Field Agents plant a listening device. This will record the meeting and lead to the valuable information our client is looking for. Using this information our client plans to take down the businesses of both rivals.

After their businesses are destroyed, we will be called upon again to fully end their existence. Something that, given the high profile of these men, wil make Hacktoria a hefty amount of money. As well as some very good standing with the French elite.

There is a catch to this however. We don’t know where this meeting will take place. Our client was able to intercept an image of the meeting location, which will take place 3 days from now at noon. Besides this photo, we know these rivals share a common interest in luxurious lifestyles along the coastlines of Western and Southern Europe.

Using this information and the intercepted image below, it is your task to figure out exactly where this meeting will take place. Our Field Agent closest to this region will take over from there.

As always. Special Agent K, the contract is yours, if you choose to accept.
```

### Extras:
```
Use your findings to generate the password that will unlock the “flagfile”, which in turn leads to your Contract Card.

The pattern will be as follows (make sure to add a dash between every word).:

country-zipcode-fullstreet-name-number
```

## 1. Download assets

Download the Flagfile
Download the full size image

## 2. Collecting intel 

From the briefing text we can find that its a "luxurious lifestyle “along the coastlines of Western and Southern Europe". The place in europe that could fit the description is "France" especially "the French Riviera" since its famous for luxury property and lifestyle.

From the image itself we can collect the follwing informations:

- [TM-F _French Premium traffic mirror_](http://www.vsi.eu/en/traffic-mirrors)
- [Agapanthus praecox (blue lily, African lily)](https://en.wikipedia.org/wiki/Agapanthus_praecox)

I was able to identify those informations by using google lense.

We could also find more intel by the building that is present on the picture:


So I started to look at architectures and compare them with the image we are given.

- The buildings in "Cannes, France" has an "[nouveau](https://en.wikipedia.org/wiki/Art_Nouveau)" art style. 
- The buildings in "Saint Tropez, France" has an "Traditional Provençal" art style.
- The buildings in "Monaco" has an "[Art Deco](https://en.wikipedia.org/wiki/Art_Deco)" art style. / Which is the exact type of building we are searching for


## 3. Finding the position

I opened google earth and searched for "Monaco" and by using the art of building as an indication we can find the exact position? No we unfortunatly cant find the exact position since the google map is using Street View images from 2011. But we do find the "Traffic mirror" indicating that we are at the right place.

## 4. Getting the flag

Just read the street-name and everything else from google maps and construct the password:

>Monaco-98000-Boulevard-de-Belgique-32

Now unzip the file and get the card.