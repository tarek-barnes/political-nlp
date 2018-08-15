The purpose of this project is ideally to summarize a book in a sentence. This is meant to be an extension from identifying a sentence which best represents a book.

## Domain

The domain being worked in is classic literature, specifically fiction. I'm familiar with the domain in that some might call me literate, but am not particularly well read in terms of literature in general.


## Data

Project Gutenberg and a website like SparkNotes with summaries of the raw books I obtain from PG.


## Known Unknowns

I'd like to use a neural network for this project. I'm deciding between a CNN and RNN, although a concern I have is the volume of data I input into my model. I might heavily filter out words (stop words and more), but even that might not be feasible and so sampling the books might be my only other alternative.

So my plan now is to feed the raw book text into the model and use the corresponding summaries to train the model. I'd like to come up with a more simplified (and unique) plot summary, so this is an area with an unclear level of effort. I don't have a solid plan as to how I'll do this yet, but I'm thinking about keeping track of different types of speech (nouns, verbs, characters, etc.) and frequencies of topics to determine the relative importance of ideas within the novel. Then I could conglomerate topics with word embeddings.

I would also like to add some kind of flexibility to the summary generation, maybe a summary relevant to the protagonist or antagonist, maybe humorous or serious. I don't know if that will be possible. I suspect the summaries I generate won't be all that accurate in the first place, given the length of a sentence or two. Finally, I'd like to create a Flask app for this since I didn't do it for my last project.