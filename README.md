# CoVaxxy: A global collection of English Twitter posts about COVID-19 vaccines 

The goal of this project is to investigate the impact of online information on COVID-19 vaccine uptake and health outcomes. 

# Data

An on-going collection of English-language Twitter posts about COVID-19 vaccines is available [here](https://zenodo.org/record/4530212).

To create as complete a set of Twitter posts related to COVID-19 vaccines as possible, we carefully select a list of keywords through a snowball sampling technique. We start with the two most relevant keywords, i.e., `covid` and `vaccine`, as our initial seeds.
Next, we gather tweets utilizing the filtered stream endpoint of the Twitter API for three hours. From these gathered tweets, we then identify potential keywords that frequently co-occur with the seeds, adding them to our seed list only after manually ensuring they are closely related to our topic. This process was repeated six times between Dec. 15, 2020 and Jan. 2, 2021 with each iteration's data collection taking place at different times of the day to capture tweets from different geographic areas and demographics. The seed list serves as our initial keyword list.
We further refine the keyword list by manually combining certain keywords into composites (e.g.`covid19 pfizer`), as a way to ensure that the dataset is broad enough to include most relevant (English) conversations while excluding tweets that are not related to the vaccine discussion. 

Some notes on the query syntax of Twitter's filtered stream API: 
* Queries that include keywords also match hashtags, URLs, and substrings. For example, `covid` matches `cnn.com/covid` and `#covid19`.
* Using `covid19 pfizer` as a composite matching phrase will capture tweets that contain `covid19` *and* `pfizer`. On the other hand, including `covid19`, `pfizer` as separate keywords will capture tweets that contain `covid19` *or* `pfizer`.

More details on the data collection can be found in our paper describing the collection of English-language Twitter posts about COVID-19 vaccines:

Matthew DeVerna, Francesco Pierri, Bao Truong, John Bollenbacher, David Axelrod, Niklas Loynes, Cristopher Torres-Lugo, Kai-Cheng Yang, Filippo Menczer, and John Bryden (2021) **"CoVaxxy: A global collection of English Twitter posts about COVID-19 vaccines."** Preprint arXiv:2101.07694 https://arxiv.org/abs/2101.07694

If you use this data, please cite this reference paper.

# Dashboard

We have developed a live dashboard to allow people to visualize descriptive statistics and preliminary results. It is available here: https://osome.iu.edu/tools/covaxxy

# Team

* [Matthew R. DeVerna](https://www.matthewdeverna.com/), Bao Truong, John Bollenbacher, David Axelrod, Cristopher Torres-Lugo, Kai-Cheng Yang, [Fil Menczer](https://cnets.indiana.edu/fil/), John Bryden *([Observatory on Social Media](https://osome.iu.edu/), Indiana University)* 
* Francesco Pierri *(Department of Electronics, Information and Bioengineering, Politecnico di Milano)* 
* Niklas Loynes *(School of Social Sciences, University of Manchester)*

# Acknowledgments

This project is supported in part by the Knight Foundation and Craig Newmark Philanthropies.