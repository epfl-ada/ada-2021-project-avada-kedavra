# TITLE: A deep dive into the mediatic place of climate change

# Abstract 

Despite the scientifically established climate emergency, there is still a lack of action against global warming. As a large part of the information the population receives is in the press, we would like to understand how is the environmental topic tackled in this media. The aim of the project is to provide deep insight on the mediatic representation of climate-related issues. Indeed, we would like to first understand what characteristics make a person represented in the public climate debate, and if some communities are excluded from it. This will help us have some insight on the most climate-related mediated opinions in the press. As the climate crisis is a rapidly evolving topic, we would also like to investigate its evolution in the press. This will enable us to have a global visualization of the information made available to the public across time, and thus a better understanding of why so many people are not concerned about climate change.
 
# Research Questions
 
 - [x] Is there any temporal evolution in the mediatic coverage of the climate crisis ? If so, does it correlate with specific events ? 
 
 - [x] Is there an evolution in the general climate-related opinions made publicly avaiblable by mainstream media ? What is the current typical profile of a person talking about climate in the media ? Is it the same for other topic ? Are some communities excluded from the mediatic discussion surround climate change ?
 
 - [x]  Based on the evolution of the profile of a person talking about climate in the media, can we predict what characteristics will a climate-involved person have in the future ?

- [x] How do the education and occupation of people represented in the media impact their opinion on the climate crisis ? (Regarder les mots les plus représentés dans les quotes selon les études et le metier des personnes ? Scientifique vs politique vs activiste)
  
- [x] What is the main sentiment communicated in the media by different types of speakers concerning the climate crisis ? 

voilà on a revu les questions avec alicia pour être plus large
# Dataset 

### Quotebank dataset 
It's a corpus of quotations attributed to the speakers who uttered them, extracted from 162 million English news articles published between 2015 and 2020. 

#### Clean and filtered Quotebank Climate-related dataset
This is a QuoteBank subdataset.
This dataset is a corpus of quotations that we identified as climate-change-related, extracted from the entire Quotebank dataset. It results from the cleaning and filtering of the Quotebank dataset. The filtering to obtain climate-related quotes was done using a list of keywords, that was exctrated using logistic regression and the two given test sets. 

### Speaker dataset
This dataset is the list of all the speakers that appear in the Quotebank dataset, along with the caracterists, such as nationality, gender, education, political party, date of birth, ethinc group and religion. We also enriched this data with one more column, containing boolean values describing whether this person talk about climate or not. The first value is True if any quote from this speaker is found in the Climate related Dataset.

### Model training datasets
Thses two dataset will be use to train and test the logistic regression model used to classify our quotes as climate related or not. They were found on the article "ClimaText: A Dataset for Climate Change Topic Detection by Francesco S. Varini, Jordan Boyd-Graber, Massimiliano Ciaramita, Markus Leippold." These datasets are composed of sentences labeled as climate related or not. They were obtained using Active Learning on previously existing datasets. 

Link to all our obtained data: https://drive.google.com/drive/folders/1kafZtuinbhqQUU2syhdQeBHnJ9_C5E6E?usp=sharing

# Methods

We will choose between the following classifer methods to explore and answer our research questions

- Logistic regression
- Tree 
    - Random Forest 
    - Gradient Boosting

# Timeline for Milestone 3
26 nov -> 17 dec

- M2.1 Loading data and treatments wee1 (26nov -> 3dec)
Method I - BERT, Maria and Virginie 
Method II - Propensity score matching , Maria 

- M2.2 Project (4dec -> 12dec)
Method I - Logistic regression, Anissa 
Method II - Tree classifiers, Alicia 

- M3 Results Interpretation (12dec -> 17dec)
Final tests and corrections. Conclusions on our research questions, Everyone
Data Story, Everyone

# Questions
- [x] For now, we are focusing our analysis on speakers that have a unique possible QID. Indeed, some of the speakers in the QuoteBank dataset have namesakes. We did not manage to find the QID corresponding the to speakers between the QIDs of their namesakes. How could we do that ? 

- [x] Should we fit the BERT algorithm or using a pre-existing model is possible (we sent a request to obtain a code from an article) for climate-skepticism detection?

- [x] In this milestone, we tried to construct a dataframe containing all climate-related events from 2015 to 2020. We did not manage to find a feasible method to do that. How should we do it ? 


