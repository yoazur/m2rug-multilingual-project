# m2RUg Multilingual Project
This project aims to smoothly use different languages with m2RUg French voicebanks in OpenUtau using tools like dictionaries and additionnal reclists for necessary phonemes.
> [!IMPORTANT]
> This repo is still being made and is not complete. Come back later to see when it's done.

# Table of contents
- [Making your m2RUg multilingual](https://github.com/yoazur/m2rug-multilingual-project/blob/main/README.md#making-your-m2RUg-multilingual)
  - [English](https://github.com/yoazur/m2rug-multilingual-project/blob/main/README.md#adding-english)
  - [Japanese](https://github.com/yoazur/m2rug-multilingual-project/blob/main/README.md#completing-japanese)
- [Using the different languages](https://github.com/yoazur/m2rug-multilingual-project/blob/main/README.md#using-the-different-languages)
  - [English](https://github.com/yoazur/m2rug-multilingual-project/blob/main/README.md#using-english)
  - [Japanese](https://github.com/yoazur/m2rug-multilingual-project/blob/main/README.md#using-japanese)
  
# Making your m2RUg multilingual
In this part we'll see how to add language compability to an m2RUg-based voicebank using dictionaries and additionnal phonemes.
## Adding English
### The dictionary
To make your m2RUg voicebank recognise english words, we'll mainly use a dictionary. To add it to the desired voicebank :
- Download the [en-xsampa.yaml](https://github.com/yoazur/m2rug-multilingual-project/blob/main/Dictionaries/en-xsampa.yaml) found in the Dictionaries folder.
![Download en-xsampa.yaml](https://github.com/yoazur/m2rug-multilingual-project/blob/main/tutorial-images/downloadendict.png)
- Place it at the root folder of the voicebank.
![Place the file in root directory of voicebank](https://github.com/yoazur/m2rug-multilingual-project/blob/main/tutorial-images/placeendict.png)
> [!IMPORTANT]
> This dictionary includes the new W phoneme that you'll see in a moment. If you do not wish to record the W-Addon reclist or you're adding onto a voicebank that is not yours, you may simply replace all occurences of "W" (quotes included) with "u" in en-xsampa.yaml using the Find and Replace feature in your text editor of choice.
### The W-Addon
The en-xsampa.yaml dictionary uses the W phoneme, an additional vowel used for english and japanese, equivalent to the "uh" phoneme in arpasing. To record and add the W phoneme to your own m2RUg voicebank:
- Download the [W-m2RUg-addon.txt](https://github.com/yoazur/m2rug-multilingual-project/blob/main/Additional-Phonemes/W-addon/W-m2RUg-addon.txt) reclist found in Additional-Phonemes/W-addon folder.
![Download W-m2RUg-addon.txt](https://github.com/yoazur/m2rug-multilingual-project/blob/main/tutorial-images/downloadwaddon.png)
- Record the reclist using your recording software of choice (OREMO or RecStar is recommended for reclist reecording)
- Create a new folder in your voicebank for the addon (This makes organisation easier). In that folder, put all your recordings and the [oto.ini](https://github.com/yoazur/m2rug-multilingual-project/blob/main/Additional-Phonemes/W-addon/oto.ini) included in Additional-Phonemes/W-addon
![Make a folder for the W phoneme](https://github.com/yoazur/m2rug-multilingual-project/blob/main/tutorial-images/waddonfolder)
- Configure the oto.ini using your otoing method of choice (setparam, vLabeler, Laberu, Openutau, whatever is fine)

Your voicebank now has the W phoneme ready to use !
## Completing Japanese

# Using the different languages
## Using English
## Using Japanese

# Credit
Thank you to [Utau French Ressources](https://utaufrance.com) for making the m2RUg reclist.

Thank you to [intunist](https://github.com/intunist/) for the [base dictionnary](https://github.com/intunist/diffsinger-english-support/blob/main/intunist-eng-word-dict.txt) used for english.
