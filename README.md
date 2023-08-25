Flash cards are cards with question on one side and answers on opposite. Exist several computer apps that automate [spaced repetition]( www.gwern.net/Spaced-repetition) for memorization and have recorded alot of data. Humans really need more cognitive tests for their own health. I expected electronic flashcard data to be useful as a cognitive test so I started a project to analyze that data. Turns out the project teaches users about learning and allows them to experiment with and optimize their own learning process. In addition, the project encourages learning by illustrating success in detail, similar to gamification. 

A more indepth discussion of goals and why Anki works as a test of cognitive health is on [Open Humans wiki](wiki.openhumans.org/wiki/Flash_Cards_as_Cognitive_Test.)
 

## How to use these notebooks 
Green Code button ->  download Zip then open the html files in any browser.

IMPORTANTHERE \<- Search for this tag to skip lots of data munging,
debugging and minutia.

CHANGEME \<- If you run this notebook on your own data search for this
tag to find things you may need to change.

All the code was written for one specific database with its own idiosyncrasies. Please help me fix this by submitting errors on github along with your data as in step 2. Because project infers lots from data with little outside information, some sections require lots of data, like 50k reviews and 5k cards, and this may be unavoidable.   

1. Running these notebooks at home on your own data. 

On windows,install R and RStudio. Find collection.anki2 file (in my case "Anki\AnkiAppData\User 1"). Make a copy and put it into project folder or change COLLECTION_PATH to file's file path.

WARNING some of these notebooks take a LONG time to run. 

2. Uploading anki database to Jupyter or Open Humans

DATA LIKE THE CONTENTS OF NOTES AND CARDS WILL BECOME AVAILABLE TO AND IN THIS NOTEBOOK. If you do not have anything private in your collection just upload a copy of the database. If you do not want anyone to see some notes follow the following instructions. Make backups of all important directories which in my case is all under Anki. Disconnect from internet so Anki does not sync. Open anki. Delete Private decks and ones that may cause errors. Quit Anki. Send new collection.anki2 file to Open Humans. Replace new folders on you computer with backup to get deleted decks back.

## Other analyses of flashcard data 

Piotr Wozniaks work on Spacing and Repetion supermemo.guru/wiki/SuperMemo_Guru

Gwern tries something similar in gwern.net/treadmill#treadmill-effect-on-spaced-repetition-performance-randomized-experiment but without as much feature engineering. 

Learned how to get Anki's db and some ideas on what to do with the data from Ojisan Seiuchi
www.ojisanseiuchi.com/2017/12/17/Peering-into-Anki-using-R/

ChrisK91 chrisk91.me/2018/02/03/Accessing-the-Anki-database-via-R.html

Gene Dan genedan.com/no-126-four-years-of-spaced-repetition/

SigmaX www.reddit.com/r/Anki/comments/piqe81/all_my_anki_decks_as_a_sunburst_plot_after_5/

Anki has a stats window as well as several addons that try to improve
it. At what time does user perform best and chooses to do most cards for example.

ankiweb.net/shared/info/993120073 Adds correct answers by type
of card state

ankiweb.net/shared/info/266436365 Shows cumulative on reviews
per day histogram and minor improvements form many graphs. Breaks
occasionaly.

Also Anki Simulator and True Retention addons which I should review.

Mnemosny, an app similar to anki, has a database of user's reviews
which used to be available for the public but mnemosnye itself is not very popular.
