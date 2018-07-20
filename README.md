# Language in Peacebuilding

* “Liberal peacebuilding is teleological”
* “Peacebuilding and statebuilding is social engineering”


## The is-ought problem
“The apparent gap between "is" statements and "ought" statements, when combined with Hume's fork, renders "ought" statements of dubious validity. Hume's fork is the idea that all items of knowledge are either based on logic and definitions, or else on observation. If the is–ought problem holds, then "ought" statements do not seem to be known in either of these two ways, and it would seem that there can be no moral knowledge.”

This project intends to identify the linguistic and academic trends in peacebuilding literature. It is particularly concerned with what some have called the teleological or prescriptive nature of the literature in the area. It attempts to quantitatively locate trends in the language used and identify any "ought" statements: i.e., a statement of the form "In order for agent A to achieve goal B, A reasonably ought to do C" exhibits no category error and may be factually verified or refuted. "Oughts" exist, then, in light of the existence of goals.
> For instance, a pair of scissors that cannot easily cut through paper can legitimately be called bad since it cannot fulfill its purpose effectively. Likewise, if a person is understood as having a particular purpose, then behaviour can be evaluated as good or bad in reference to that purpose. In plainer words, a person is acting good when that person fulfills that person's purpose.
> Eg., “ought” statements (within one or two sentences) with state-affirming terms like peace, community or nation can be used prescriptively

## Research questions
What linguistic and publishing trends have existed over the past 20 years and how do related publication areas compare?
What proportion of articles contain prescriptive sentences (%)?
Is there a significant difference between proportion of prescriptive sentences with state-affirming terms between sample from Development studies, Peace and Conflict studies, Peacebuilding and Political science literature?

## About the project

This project is an opportunity to build a web-scraping tool in R, build a Postgres database, and perform some quantitative text analysis (also in R). I have used the [Taylor and Francis Online](https://www.tandfonline.com/) publication repository to obtain a quantitatively significant sample of journal articles based on eight keyword searches. Here is a list of the searches performed:
* "peacebuilding"
* "peacemaking"
* "state-building"
* "nation-building"
* "conflict resolution"
* "conflict transformation"
* "liberal peacebuilding"
* "peace and conflict studies"

For each search I returned ~5000 articles, except liberal peacebuilding which returned 100% search coverage of 1,846 articles. The results contained the article's title, publication date, authors, abstract, the full journal text and bibliometrics published on the article's webpage such as citations and views. 
After some data processing, this project collected the following number of articles by search term:


| search terms| no. retrieved | % of total | 
|-------------|---------------|-------------|
|peacebuilding |    |     |
|peacemaking |    |     |
|state-building |    |     |
|nation-building |    |     |
|conflict resolution |    |     |
|conflict transformation |    |     |
|liberal peacebuilding |    |     |
|peace and conflict studies |    |     |


## Workflow
A comparative analyse of language used in peace and conflict studies domains

* Digitise journal articles and categorise according to search queries
* Webscraping Taylor and Francis Online

Build flexible database, process data and transfer
* clean up data
* transform data into tables, including doing post-processing aggregates
* create DB schema
* load tables

Process text
* Tokenise
* Lemmanise
* Remove stop words and other redundant words

Text analysis
* Frequency counts
* Unigrams
* Bigrams
* Trigrams
* Sentiment analysis: what is the comparative sentiment expressed? Does this suggest teleology?
* Topic modeling: what are the general topics discussed by each set?
* Network analysis: what are the word clusters and how do they differ by set?

