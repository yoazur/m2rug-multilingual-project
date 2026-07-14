# m2RUg Multilingual Project
This project aims to smoothly(ish) use different languages with m2RUg French voicebanks in OpenUtau using tools like dictionaries and additionnal reclists for necessary phonemes.
> [!NOTE]
> This repo is still being made and is not complete. Come back later to see when it's done.

# Table of contents
- [Making your m2RUg multilingual](https://github.com/yoazur/m2rug-multilingual-project/blob/main/README.md#making-your-m2RUg-multilingual)
  - [English](https://github.com/yoazur/m2rug-multilingual-project/blob/main/README.md#adding-english)
  - [Japanese](https://github.com/yoazur/m2rug-multilingual-project/blob/main/README.md#completing-japanese)
- [Using the different languages](https://github.com/yoazur/m2rug-multilingual-project/blob/main/README.md#using-the-different-languages)
  - [English](https://github.com/yoazur/m2rug-multilingual-project/blob/main/README.md#using-english)
  - [Japanese](https://github.com/yoazur/m2rug-multilingual-project/blob/main/README.md#using-japanese)
- [Credit](https://github.com/yoazur/m2rug-multilingual-project/blob/main/README.md#credit)
# Making your m2RUg multilingual
In this part we'll see how to add language compability to an m2RUg-based voicebank using dictionaries and additionnal phonemes.
## Adding English
### The dictionary
Most of the phonemes necessary to make english are already in complete m2RUg voicebanks. However, you can optionally add the W phoneme when recording your voicebank if you also plan on adding full japanese compatibility (we'll talk about that later). That said, to make english words convert to the right m2RUg-sampa phonemes, we'll mainly use a phoneme dictionary. To add it to the desired voicebank :
- Download the [en-xsampa.yaml](https://github.com/yoazur/m2rug-multilingual-project/blob/main/Dictionaries/en-xsampa.yaml) found in the Dictionaries folder.
![Download en-xsampa.yaml](https://github.com/yoazur/m2rug-multilingual-project/blob/main/tutorial-images/downloadendict.png)
- Place it at the root folder of the voicebank.
![Place the file in root directory of voicebank](https://github.com/yoazur/m2rug-multilingual-project/blob/main/tutorial-images/placeendict.png)
> [!IMPORTANT]
> This dictionary includes the mentioned before W phoneme that you'll see in a moment. If you do not wish to record the W-Addon reclist or you're adding onto a voicebank that is not yours, you may simply download [en-xsampa(no-W).yaml](https://github.com/yoazur/m2rug-multilingual-project/blob/main/Dictionaries/en-xsampa(no-W).yaml) instead and remove (no-W) from the name of the file.
### The W-Addon
The en-xsampa.yaml dictionary uses the W phoneme, an additional vowel used for english and japanese, equivalent to the "uh" phoneme in arpasing. To record and add the W phoneme to your own m2RUg voicebank:
- Download the [W-m2RUg-addon.txt](https://github.com/yoazur/m2rug-multilingual-project/blob/main/Additional-Phonemes/W-addon/W-m2RUg-addon.txt) reclist found in Additional-Phonemes/W-addon folder.
![Download W-m2RUg-addon.txt](https://github.com/yoazur/m2rug-multilingual-project/blob/main/tutorial-images/downloadwaddon.png)
- Record the reclist using your recording software of choice (OREMO or RecStar is recommended for reclist recording)
- Create a new folder in your voicebank for the addon (This makes organisation easier). In that folder, put all your recordings and the [oto.ini](https://github.com/yoazur/m2rug-multilingual-project/blob/main/Additional-Phonemes/W-addon/oto.ini) included in Additional-Phonemes/W-addon.  
![Make a folder for the W phoneme](https://github.com/yoazur/m2rug-multilingual-project/blob/main/tutorial-images/waddonfolder)
- Configure the oto.ini using your otoing method of choice (setparam, vLabeler, Laberu, Openutau, whatever is fine)

Your voicebank now has english ready to use ! Check out [how to use your new english compatibility](https://github.com/yoazur/m2rug-multilingual-project/blob/main/README.md#using-english).
## Completing Japanese
Almost all of the phonemes necessary to make japanese are already in complete m2RUg voicebanks and the french dictionary cmudict-fr.txt for OpenUtau already has japanese hiragana corresponding to the correct phonemes. However, there is a single phoneme not included in basic m2RUg : the japanese u. That's why this section is only useful if you want to record the W phoneme (which I talked about in the english section earlier) for your own voicebank for full japanese compatibility.

To add this phoneme and achieve full japanese compatibility with your m2RUg, simply follow the same [instructions as for adding english](https://github.com/yoazur/m2rug-multilingual-project/blob/main/README.md#adding-english) (both the dictionary and the W-Addon), since the en-xsampa.yaml dictionary also contains japanese hiragana. When that's done, check out [how to use your new japanese compatibility](https://github.com/yoazur/m2rug-multilingual-project/blob/main/README.md#using-japanese).

# Using the different languages
## Using English
To use the dictionary for english, we'll use the built-in english x-sampa phonemizer for OpenUtau. If the dictionary doesn't work at first and the phonemes are blank, try using the phonemizer with any voicebank without the dictionary to initialise the phonemizer and create the base dictionary in the Plugins folder first (i think idk really). This dictionary has been confirmed to work on the latest version of OpenUtau Lunai edition. (it probably works on other versions and i know it doesn't work at first but i can't figure out how i did make it work in the first place uuuurrghh)
## Using Japanese

# Credit
Thank you to [Utau French Ressources](https://utaufrance.com) for making the m2RUg reclist.

Thank you to [intunist](https://github.com/intunist/) for the [base dictionnary](https://github.com/intunist/diffsinger-english-support/blob/main/intunist-eng-word-dict.txt) used for english.
