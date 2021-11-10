# TITLE: 

# Abstract 

Despite the scientifically esthablished climate emergency, there is still a lack of general action fighting against global warming, and a non-negligeable climatesceptic tendancy in the population. As a large part of the information the population receives is in the press, we would like to understand how is the environmental topic tackled in this media. The aim of the project is to provide deep insigth on who is talking about climate change, and how. Indeed, we would like to first understand what caracteristics make a person more inclined to talkabout climate. Then, we would like to assess what proportion of the environmental mediac representation is actually taken by climat denial. This will enable us to have a global vizualisation of what kind of information is made available to the public media, and thus a better understanding of why so many people are not concerned about climate change.  


# Research Questions

 - [x] What caracteristics of a person make them more inclined to talk about climate change ? to be climate sceptic ? 
 
 - [x] Who talks the most about climat change ?
 
 - [x] Does the concern about climate change differ according to the nationality, profession, education, political party, age or gender of the speakers ?  
 
 - [x] What is the proportion of climat-sceptic representation is the media ? 
 
 - [x] How climate representation does change according to natural catastroph ? 
 

 
# Dataset 

### Quotebank dataset 
It's a corpus of  quotations attributed to the speakers who uttered them, extracted from 162 million English news articles published between 2015 and 2020. 

### Clean and filtered Quotebank Climate-related dataset
This dataset is a corpus of quotations that we identified as climate-change-related, extracted from the entire Quotebank dataset. It results from the cleaning and filtering of the Quotebank dataset. he filtering to obtain climate-related quotes was done using a list of keywords, that we esthablished using the two following articles: https://www.climaterealityproject.org/blog/key-terms-you-need-understand-climate-change and https://www.bbc.com/news/science-environment-11833685. This keyworld list is still very limited and biased at the moment, but we are considering options on how to expend it, and measure its bias. (See Methods)

### Clean and filtered Quotebank Climate change skepticism-related dataset
This dataset is very similar to the one previously described. In this case, we use another method to obtain the keywords, which is described in the joined NoteBook. Once again, this method is very flawed, and will only be used for preliminary analysis. We will upgrade it in Milestone 3. (See Methods). Also, we only used the 2020 Quotebank dataset, as a test to see if this anaysis would be feasible.

### Speaker dataset
This dataset is the list of all the speakers that appear in the Quotebank dataset, along with the caracterists, such as nationality, gender, education, political party, date of birth, ethinc group and religion. We also enriched this data with two more columns, containing boolean values: whether this person talk about climate or not, and whether the quotes from this speaker appear as climate change skepticism. The first value is True if any quote from this speker is found in the Climate related Dataset.

# Methods
- Linear regression
- Tree
- BERT
- Hypothesis testing 

# Timeline for Milestone 3

# Questions

- [x] How could we deal with the fact that speakers are matched by name and not QID in the Quotebank and Quptebank-derived dataset ? 

- [x] BERT ? 