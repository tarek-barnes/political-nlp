Project Design -- 

You can see a high-level view of my initial plan in Checklist.ipynb. This was the starting point in my analysis. The purpose of this project was to look at raw text of political discourse to better understand differences stemming from ideologies. Or, in other words: can I find clear differences between liberal and conservative rhetoric? I added labels to publications as either left or right-leaning. I modeled for topics on each publication with a couple different options. My dataset seemed too big for LDA. I played around with adding stop words, modifying min/max_df parameters, and tweaking the number of topics, which helped a bit. I experimented with KMeans and TSNE to see if I could find underlying structure when looking at topics of single publications vs. multiple publications vs. corpus. I also looked at more surface-level things, like syntax, sentiment, and relative number of adjectives to see if I could flesh out tone of voice or strength of language. 


Other note --

I'd started with trying to generate 1-2 sentence summaries by using entire books & corresponding scraped summaries. However, this either seemed like it would be either too easy (calculating the most representative sentence) or too hard (two separate neural networks. I changed ideas so I'd have something more flexible to work with.


Tools --

Other than the standard ones, I used Tableau and spaCy (which I heard was more up-to-date than NLTK). I also experimented with an app called TAACO, which turned out not to be helpful for my application, but which automatically generates some interesting NLP results from raw input text.


Data --

News Aggregator Dataset and All the News dataset, both from Kaggle. See links below.
https://www.kaggle.com/uciml/news-aggregator-dataset
https://www.kaggle.com/snapcrack/all-the-news/home


Algorithms --

I did not use anything taught outside the scope of class. So, for topic modeling: LDA (didn't work - dataset too large), LSA, NMF (each with CountVec & TFIDF). For other NLP, worked with NLTK and spaCy. For modeling, clustering w/ KMeans and exploration with TSNE. 