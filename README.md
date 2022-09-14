# About PaperFellow

PaperFellow was built by four devoted participants of Le Wagon's Data Science Bootcamp as a final project within 10 days.

It aims to classify scientific papers based on content. For getting the data for supervised classification, we web scraped [ArXiv.org](arxiv.org) (an open-access archive for scholarly articles) and requested the [OpenAlex API](https://en.wikipedia.org/wiki/Our_Research#OpenAlex). The academic field delivered when obtaining the data in PDF format, served as a target.

In data preprocessing, using NLP techniques, we cut away any distracting characters, signs and words and reduced the remaining words to their inflected form. We used n-grams (grouping consecutive words together), to facilitate our models to distinguish academic fields more easily. Then we fed numeric representations of our text data into different models: a Support Vector Machine, a CNN-based neural network and two Recurrent Neurel Networks (one with an embedding layer, another with a pretrained Word2Vec embedding).

The Support Vector Machine resulted in the best performance of all those approaches we tried (91 percent accuracy, when four targets were given).

We also deployed our project on a Heroku page and built a workflow that would allow us to automate the model maintainance.
