# COVID Misinformation on Twitter

### Description
This project seeks to compare the types of misinformation around COVID-19 and coronavirus circulating on English-language and Arabic-language social media.  In order to support public health campaigns and healthy hygiene and self-care practices, it is first necessary to understand what types of misconceptions exist among the general population on social media.

### Data
The data for this project consists of two corpora, one of English language tweets and one of Arabic language tweets. Each corpus consisted of approximately 250,000 tweets collected between the dates of October 1, 2020 and December 31, 2020.  This unstructured text data was cleaned and preprocessed prior to topic modeling and the creation of customized Word2Vec word embeddings.

### Target
The objective was to identify topics and types of misinformation, and to compare and contrast any topic differences between languages.  Three topics of misinformation were common in both sets of tweets:

Misinformation About

1) government conspiracy behind the pandemic
2) pandemic as a cover for an electronic surveillance campaign
3) pandemic being a planned experiment and an attack by China

One further topic was salient in the Arabic tweet data:

4) home and herbal remedies to cure coronavirus

### Tools Used:

**Twint** - scraping Twitter data

**NLTK** - English language pre-processing: cleaning, tokenizing, stop word removal

**Farasa** - Arabic language pre-processing: cleaning, tokenizing, stop word removal

**Sci-Kit Learn**:

  - count vectorizer and TF-IDF to create document-term matrices
  - non-negative matrix factorization for preliminary topic modeling
  
*Word2Vec* - creation of custom embeddings from the two tweet corpora

*CorEx* - customized topic modeling using anchor words discovered through investigation with the embeddings.

## Possible Impacts

**Use Case**:  Identifying and countering public health misinformation requires identifying the type and extent of misunderstanding and confusion around COVID-19 and coronavirus.  Investigating social media data provides appropriate informational targets for a public health campaign.

**Methodological Utility**:  Traditional topic modeling methods like non-negative matrix factorization and latent semantic analysis yield information about the broad spectrum of topics present in a dataset.  However, they are imprecise, as the methods require a prior understanding of exactly how many topics to choose. When attempting to focus in on particular topics or a small handful of topics in a large social media dataset with a large variety of topics, creating customized Word2Vec word embeddings to select appropriate topic anchor words and then utilizing these in a CorEx topic model can yield more precise returns.    
