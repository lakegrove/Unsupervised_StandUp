At the end of preliminary tokenization and cleaning I took a look at men (blue) vs female (red) comics and the word differences between the two.

One thing off the bat is it's clear I will need to strip out kevin, dave, ellen, amy and some of the comics self referential names.  I also need to look at taking out more parts of speech I missed in my initial cleaning including words like "um" and "oh" 

In terms of diffences between the two we can see that women tend to talk more about pregnancy, therapy, body issues (weight, period, body) and husbands.  Men seem to have more words around police, jail, drugs, smoking, Michael Jackson and R Kelly. 

![Screen Shot 2021-05-25 at 2 13 26 PM](https://user-images.githubusercontent.com/19785958/119555444-7c509580-bd63-11eb-8e84-e1e768885ed1.png)


As for topic's I am currently in my first pass of topic modeling and have the below topics using NMF. I am continuing to refine my stop words and beginning to explore max_df/min_df handles to get a clearer picture of topics.  In my first topic I can see ideas around relationships and love. In the second topic ideas around communciation and being understoof with words like know, want, tell, look and need.  The next two topics are a bit confusing and probably have some prime candiates for stop words.

Topic 4 also stands out as it has white, black and asian and seems to indicate ideas around race.

![Screen Shot 2021-05-25 at 3 12 39 PM](https://user-images.githubusercontent.com/19785958/119562222-b6259a00-bd6b-11eb-9e50-e6db7b59b5b7.png)

My next steps are to to take this and run the NMF through TFIDF and look at topics alongside text to see if there is better luck there as my initial look here looks blah so far.  I am hoping to look at LSA at bit more and most likely eventually Corex.  For corex I am thinking about anchors around love, religion, drugs, sex, wife/hanband, kids and body.

Additional analysis if there is time is to compare the highest rated comedian (Dave Chapelle) vs the lowest rated (Amy Schumer).  I'd also like to look deeper at Chapelle (considered one of if not the greatest living comedian) and how his material has changed through time. 
