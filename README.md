# FineTune_DistilRoBERTa

#### Fine tune [DistilRoBERTa base model](https://huggingface.co/distilroberta-base) for Objectivity analysis.


In depth:
- [news_source_objectivity](https://github.com/HzaRashid/news_source_objectivity) was my first [NLP](https://towardsdatascience.com/your-guide-to-natural-language-processing-nlp-48ea2511f6e1) project, where I used the nltk, textblob, and vader libraries to measure the objectivty of a news source's tweets. 

- In this repository, I expand on objectivity analysis by fine tuning a pretrained transformer model, DistilRoBERTa, to predict if a text with 240 characters is Objective or Subjective. 

- The Objective dataset is gathered from [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset?select=movies_metadata.csv), which, most importantly, contains plot descriptions on about 50000 films/tv-shows/documentaries, in the movies_metadata.csv file under the 'overview' column.
-  The Subjective dataset is the popular [IMDB Dataset of 50k Movie Reviews ](https://www.kaggle.com/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews).

- I gathered the synopses and reviews from the respective datasets, and labeled them to either 'Objective' or 'Subjective' in a final data frame consisting 10000 pieces of text, reduced to 240 characters (i.e., similar to Twitter), and evenly divided between the synopses (which are given the Objective label) and reviews (given the Subjective label).
