# FineTune_DistilRoBERTa

#### Fine tune [DistilRoBERTa base model](https://huggingface.co/distilroberta-base) for Objectivity analysis.


In depth:
- [news_source_objectivity](https://github.com/HzaRashid/news_source_objectivity) was my first [NLP](https://towardsdatascience.com/your-guide-to-natural-language-processing-nlp-48ea2511f6e1) project, where I used the NLTK, TextBlob, and Vader libraries to measure the objectivity of a news source's Tweets. 

- In this repository, I expand on objectivity analysis by fine tuning a pretrained [transformer model](https://towardsdatascience.com/illustrated-guide-to-transformers-step-by-step-explanation-f74876522bc0), DistilRoBERTa, to predict if a text with 240 characters is Objective or Subjective. 

- The Objective dataset is gathered from [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset?select=movies_metadata.csv), which, most importantly, contains plot descriptions on about 50000 films/tv-shows/documentaries.
-  The Subjective dataset is the popular [IMDB Dataset of 50k Movie Reviews](https://www.kaggle.com/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews).

- After getting the plot descriptions and reviews, I labeled them as either 'Objective' or 'Subjective', respectively. The final data frame that is split into train, validation, and test sets, consists of 10000 pieces of text, reduced to 240 characters (similar to Twitter), and is evenly divided between the two categories.
