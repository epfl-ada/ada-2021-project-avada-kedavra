# TITLE: A deep dive into the mediatic place of climate change

# Abstract 

Despite the scientifically esthablished climate emergency, there is still a lack of general action fighting against global warming, and a non-negligeable climatesceptical tendancy in the population. As a large part of the information the population receives is in the press, we would like to understand how is the environmental topic tackled in this media. The aim of the project is to provide deep insigth on who is talking about climate change, and how. Indeed, we would like to first understand what caracteristics make a person more inclined to talk about climate. Then, we would like to assess what proportion of the environmental mediac representation is actually taken by climat denial. This will enable us to have a global vizualisation of what kind of information is made available to the public media, and thus a better understanding of why so many people are not concerned about climate change.  


# Research Questions

 - [x] What is the current typical profile of a person talking about climate in the media ? Is it the same for other topic ? (Comparaison entre les caractéristiques de personnes les plus représentées dans le QuoteBank vs celles qui parlent du climat) (comparaison des nationalités avec une carte du monde) 
 
 - [x] Based on the evolution of the profile of a person talking about climate in the media, can we predict what characteristics will a climate-involved person have in the future ? 
 
 - [x] Is there any temporal evolution in the mediatic coverage of the climate crisis ? If so, does it correlate with specific events ? 
 
 - [x] Who are the top 10 people that talks the most about climate change over the year ? Does it show an evolution in the general opinions made publicly avaiblable by mainstream media ? 
 
 - [x] Are some communities excluded from the mediatic discussion surround climate change ? (Comparer la proportion de chacun des communautés dans QB en général avec la propotion des communautés dans les phrases qui parlent du climat)
 
 - [x] What is the most represented climate crisis-related topic along the years ? Does it show an evolution in the general opinions made publicly avaiblable by mainstream media ? (Trouver les mots reliés au climat les plus représentés dans les quotes chaque années)

 
# Dataset 

### Quotebank dataset 
It's a corpus of  quotations attributed to the speakers who uttered them, extracted from 162 million English news articles published between 2015 and 2020. Its

#### Clean and filtered Quotebank Climate-related dataset
This is a QuoteBank subdataset.
This dataset is a corpus of quotations that we identified as climate-change-related, extracted from the entire Quotebank dataset. It results from the cleaning and filtering of the Quotebank dataset. he filtering to obtain climate-related quotes was done using a list of keywords, that we esthablished using the two following articles: https://www.climaterealityproject.org/blog/key-terms-you-need-understand-climate-change and https://www.bbc.com/news/science-environment-11833685. This keyworld list is still very limited and biased at the moment, but we are considering options on how to expend it, and measure its bias. (See Methods)

#### Clean and filtered Quotebank Climate change skepticism-related dataset
Again, this is a QuoteBank subdataset. 
This dataset is very similar to the one previously described. In this case, we use another method to obtain the keywords, which is described in the joined NoteBook. As a base of our method we wused the folling article:  Once again, this method is very flawed, and will only be used for preliminary analysis. We will upgrade it in Milestone 3. (See Methods). 

### Speaker dataset
This dataset is the list of all the speakers that appear in the Quotebank dataset, along with the caracterists, such as nationality, gender, education, political party, date of birth, ethinc group and religion. We also enriched this data with two more columns, containing boolean values: whether this person talk about climate or not, and whether the quotes from this speaker appear as climate change skepticism. The first value is True if any quote from this speker is found in the Climate related Dataset.

### BERT training datasets
Thses two dataset will be use to train and test our BERTbase model. They were found on the article "ClimaText: A Dataset for Climate Change Topic Detection by Francesco S. Varini, Jordan Boyd-Graber, Massimiliano Ciaramita, Markus Leippold." We cleaned and modified them so that they will have an appropriate format for BERT training. 

Link to all our obtained data: https://drive.google.com/drive/folders/1kafZtuinbhqQUU2syhdQeBHnJ9_C5E6E?usp=sharing

# Methods

- BERT, to predict our categorical output [climate skeptic social] and [climate skeptic scientific] and detect climate-change topic in quotes
- Propensity score matching, in order to avoid unovserved correlations due to treatment prediction (and not effect of the treatment)

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


