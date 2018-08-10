---
layout: default
---

# Language in Peace and Conflict Studies

## Preamble

![bibmetrics_year&search_05-17](outputs/bibmetrics_year&search_05-17.jpeg)

Are we moving into a new era of peace and conflict studies? A new era defined by peacebuilding and state-building, and less by building the nation and the community. Furthermore, could there be a significant split emerging in the peace and conflict academe between those who espouse institutional, state-centric approaches to peacebuilding and those who criticise it as "liberal peacebuilding". 

The figure above shows the popularity trends of publications in the area since 2005. This data is derived from harvesting thousands of publication records from the Taylor and Francis Online repository, broken up by eight search terms, which could be considered sub-branches of Peace and Conflict Studies. Each grid above indicates the publication results for each of the eight search terms. (More about the project [below](#about)).

The interesting insight this figure above suggests is the split in trends between some search terms. 2010-2012 garned much interest in the areas of conflict resolution, conflict transformation, nation-building and peace-making, which have been declining ever since, whilst peacebuilding, statebuilding-building and (the critique of) liberal peacebuilding are continuing to trend upwards. 

Keep in mind that this graph is based on the bibliometric data associated with each article, which is taken as a proxy for the article's general popularity. The data expressed above does not indicate publication trends. You'll see this [below](#initial-results). Suffice it to say that popularity and publication numbers seem to be somewhat in sync. As you'd expect, peaks in publications look like they are followed by peaks in popularity a year or so later.  

There's still so much to say about the data expressed above, like the correlative relationships between couples such as state-building and nation-building or peace-making and peace-building (one goes up, the other goes down), but I'll leave this for later.

## Contents

* [About the project](#about)
* [Initial results](#initial-results)
* [Where to](#where-to)


## About the project {#about}

This project is a meta-analysis of the peacebuilding literature since 2005. The project involved building a web-scraping tool in R, feeding results into a Postgres database, and perform some quantitative text analysis (also in R). 

I have used the [Taylor and Francis Online](https://www.tandfonline.com/) publication repository to obtain a significant sample of journal articles based on eight keyword searches. Here is a list of the searches performed:
* "peacebuilding"
* "peacemaking"
* "state-building"
* "nation-building"
* "conflict resolution"
* "conflict transformation"
* "liberal peacebuilding"
* "peace and conflict studies"

For each search I returned ~5000 articles, except liberal peacebuilding which returned 100% search coverage of 1,846 articles. The results contain each article's title, publication date, authors, abstract, the full journal text and bibliometrics published on the article's webpage such as citations and views. 

First, I will be using this data to look at article popularity, profile the top countries mentioned, compare trends between searches. 

Second, I will be performing text analysis on the language used in titles, abstracts and the full text to ascertain common themes. This will also be broken down by search term.

Finally, I won't to identify the level of prescriptiveness/teleology in the articles, by search term (see [Where to](#where-to)).

After some data processing, this project collected the following number of articles by search term:

### Coverage
<iframe width="600" height="371" seamless frameborder="0" scrolling="no" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRQIsodC2Z9_9FdKCspFuvlCee87lK4IB4MrjBSo-qVyzebVeNdc9QtWhaPm1pfOkWw6G69ZGLCzgix/pubchart?oid=1351741946&amp;format=interactive"></iframe>

### Metric data
<iframe width="600" height="371" seamless frameborder="0" scrolling="no" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRQIsodC2Z9_9FdKCspFuvlCee87lK4IB4MrjBSo-qVyzebVeNdc9QtWhaPm1pfOkWw6G69ZGLCzgix/pubchart?oid=952477040&amp;format=interactive"></iframe>

### Country mentions
<iframe width="600" height="371" seamless frameborder="0" scrolling="no" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRQIsodC2Z9_9FdKCspFuvlCee87lK4IB4MrjBSo-qVyzebVeNdc9QtWhaPm1pfOkWw6G69ZGLCzgix/pubchart?oid=1121924922&amp;format=interactive"></iframe>

## Initial results {#initial-results}

![pub_count_year&search_05-17](outputs/pub_count_year&search_05-17.jpeg)

![common_countries_titles_20](outputs/common_countries_titles_20.jpeg)

![common_country_title_years_10](outputs/common_country_title_years_10.jpeg)

![common_countries_abstract_20](outputs/common_countries_abstract_20.jpeg)

![common_country_abstracts_years_10](outputs/common_country_abstract_years_10.jpeg)

![common_countries_abstract_search_20](outputs/common_countries_abstract_search_20.jpeg)

![views_ratio](outputs/views_ratio.jpeg)

![cites_ratio](outputs/cites_ratio.jpeg)

![alts_ratio](outputs/alts_ratio.jpeg)


## Where to 
### The is-ought problem

*Liberal peacebuilding is teleological* (e.g., [Greener, 2013](https://www.tandfonline.com/doi/abs/10.1080/17502977.2012.733575?src=recsys&journalCode=risb20),[Richmond, 2006](https://www.tandfonline.com/doi/abs/10.1080/14678800600933480?src=recsys&journalCode=ccsd20), [Richmond & Franks, 2007](https://www.researchgate.net/publication/240701003_Liberal_Hubris_Virtual_Peace_in_Cambodia))

*Peacebuilding and statebuilding is social engineering* (e.g., [Richmond, 2013](https://www.tandfonline.com/doi/abs/10.1080/13698249.2010.484909?journalCode=fciv20), [Goodhand & Mark Sedra](https://books.google.com.au/books?id=M4D7CwAAQBAJ&pg=PA1&lpg=PA1&dq=Peacebuilding+and+statebuilding+is+social+engineering&source=bl&ots=iTkjj1Haa1&sig=jScITjMJKtogN5RDdwktSyIJX5w&hl=en&sa=X&ved=0ahUKEwimu9eRiN_bAhVCI5QKHTeWBrAQ6AEINjAD#v=onepage&q=Peacebuilding%20and%20statebuilding%20is%20social%20engineering&f=false))

“The apparent gap between "is" statements and "ought" statements, when combined with Hume's fork, renders "ought" statements of dubious validity. Hume's fork is the idea that all items of knowledge are either based on logic and definitions, or else on observation. If the is–ought problem holds, then "ought" statements do not seem to be known in either of these two ways, and it would seem that there can be no moral knowledge.”

This project intends to identify the linguistic and academic trends in peacebuilding literature. It is particularly concerned with what some have called the teleological or prescriptive nature of the literature in the area. It attempts to quantitatively locate trends in the language used and identify any "ought" statements: i.e., a statement of the form "In order for agent A to achieve goal B, A reasonably ought to do C" exhibits no category error and may be factually verified or refuted. "Oughts" exist, then, in light of the existence of goals.
> For instance, a pair of scissors that cannot easily cut through paper can legitimately be called bad since it cannot fulfill its purpose effectively. Likewise, if a person is understood as having a particular purpose, then behaviour can be evaluated as good or bad in reference to that purpose. In plainer words, a person is acting good when that person fulfills that person's purpose.
> Eg., “ought” statements (within one or two sentences) with state-affirming terms like peace, community or nation can be used prescriptively

## Research questions
* What linguistic and publishing trends have existed over the past 20 years and how do related publication areas compare?
* What proportion of articles contain prescriptive sentences (%)?
* Is there a significant difference between proportion of prescriptive sentences with state-affirming terms between sample from Development studies, Peace and Conflict studies, Peacebuilding and Political science literature?

