# TITLE: A deep dive into the mediatic place of climate change

# Abstract 

Despite the scientifically established climate emergency, there is still a lack of action against global warming. The aim of this project is to provide deep insight on the mediatic representation of climate-related issues. We would like to first investigate the temporal evolution of the climate change topic in the media, then understand the main characteristics of people mentioning it, and their opinions. Climate change is a very polarizing subject, so we would like to look into the general feeling toward this topic. We would also like to, if possible, predict which characteristics predispose the speaker to get involved in this debate based on the climate-involved people profil.

# Research Questions
 
- [x] Is there any temporal evolution in the mediatic coverage of the climate crisis ? 
 
- [x] What are the main typical profiles of people talking about climate in the media ? Who in the media represent the most this subject over time ?   

- [x] What is the main sentiment communicated in the media over time concerning the climate crisis ? 
 
- [x]  Based on the profile of person talking about climate in the media, can we predict what characteristics will a climate-involved person have in the future ?

# Dataset 

### Quotebank dataset 
It's a corpus of quotations attributed to the speakers who uttered them, extracted from 162 million English news articles published in English between 2015 and 2020. 

#### Clean and filtered Quotebank Climate-related dataset
This is a QuoteBank subdataset.
This dataset is a corpus of quotations that we identified as climate-change-related, extracted from the entire Quotebank dataset. It results from the cleaning and filtering of the Quotebank dataset. The filtering to obtain climate-related quotes was done using a list of keywords, that was exctracted using logistic regression and the two given test sets. 

### Speaker dataset
This dataset is the list of all the speakers that appear in the Quotebank dataset, along with the caracterists, such as nationality, gender, education, political party, date of birth, ethinc group and religion. We also enriched this data with one more column, containing boolean values describing whether this person talk about climate or not. The first value is True if any quote from this speaker is found in the Climate related Dataset. For futherer analysis, we kept the 20 most represented features for each column and turned them into one hot columns. This enable us to handle the categorical datas.

Link to all our obtained data: METTRE LE LIEN

# Methods

- In order to visualize the temporal evolution of the climate change topic, we plotted the distributon of quotes over months and years.

- To obtain the top 20 main features of each columns we exploded the values for each attribut and plot them in barplots.

- We used the vaderSentiment analysis in order to obtain the rates of positive and negative emotions in the quotes over time

- To perform classification, we .....



