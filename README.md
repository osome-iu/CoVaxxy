# CoVaxxy: A collection of English-language Twitter posts about COVID-19 vaccines 

This project, conducted by Indiana University’s Observatory on Social Media (OSoMe) in collaboration with colleagues from Politecnico di Milano, aims to track and investigate how online information impacts COVID-19 vaccine uptake and health outcomes. We offer public access to a [large collection of vaccine-related tweets](https://doi.org/10.5281/zenodo.5277197) that are gathered in real-time and updated daily (see our [data collection paper](https://ojs.aaai.org/index.php/ICWSM/article/view/18122) for more details). We combine this with [vaccine uptake and survey data](#dashboard) to create the [CoVaxxy dashboard](http://osome.iu.edu/tools/covaxxy), a web-page that allows anyone to visualize descriptive statistics and preliminary results,

## Twitter Data

An on-going collection of English-language Twitter posts about COVID-19 vaccines is available [here](https://doi.org/10.5281/zenodo.4526494).

To create as complete a set of Twitter posts related to COVID-19 vaccines as possible, we carefully select a list of keywords through a snowball sampling technique. We start with the two most relevant keywords, i.e., `covid` and `vaccine`, as our initial seeds.
Next, we gather tweets utilizing the filtered stream endpoint of the Twitter API for three hours. From these gathered tweets, we then identify potential keywords that frequently co-occur with the seeds, adding them to our seed list only after manually ensuring they are closely related to our topic. This process was repeated six times between Dec. 15, 2020 and Jan. 2, 2021 with each iteration's data collection taking place at different times of the day to capture tweets from different geographic areas and demographics. The seed list serves as our initial keyword list.
We further refine the keyword list by manually combining certain keywords into composites (e.g.`covid19 pfizer`), as a way to ensure that the dataset is broad enough to include most relevant (English) conversations while excluding tweets that are not related to the vaccine discussion. 

Some notes on the query syntax of Twitter's filtered stream API: 
* Queries that include keywords also match hashtags, URLs, and substrings. For example, `covid` matches `cnn.com/covid` and `#covid19`.
* Using `covid19 pfizer` as a composite matching phrase will capture tweets that contain `covid19` *and* `pfizer`. On the other hand, including `covid19`, `pfizer` as separate keywords will capture tweets that contain `covid19` *or* `pfizer`.

#### Iffy+
To categorize tweets as low credibility, we utilize the [Iffy+ Misinfo/Disinfo list](https://iffy.news/iffy-plus/) created by [Iffy.news](https://iffy.news/). As stated on the Iffy+ page, "_Iffy+ merges lists of sites that regularly publish mis/disinformation, as identified by major fact-checking and journalism organizations, into a single dataset._" Please checkout [the description](https://iffy.news/iffy-plus/) of the list for more information.

## Paper
More details on the data collection can be found in our paper describing the collection of English-language Twitter posts about COVID-19 vaccines:

* [Matthew R. DeVerna](https://www.matthewdeverna.com/), [Francesco Pierri](https://frapierri.github.io), [Bao Truong](https://btrantruong.github.io/), [John Bollenbacher](https://jbollenbacher.github.io/), [David Axelrod](https://cns-nrt.indiana.edu/students/trainees/2019/David-Axelrod.html), Niklas Loynes, [Cristopher Torres-Lugo](http://christorreslugo.com/), [Kai-Cheng Yang](http://www.kaichengyang.me/), [Fil Menczer](https://cnets.indiana.edu/fil/), and [John Bryden](http://jbryden.co.uk/home/) (2021) **"CoVaxxy: A collection of English Twitter posts about COVID-19 vaccines."** in Proceedings of the 15th International Conference on Web and Social Media. ([link to paper](https://ojs.aaai.org/index.php/ICWSM/article/view/18122))

If you use this data, please cite this reference paper.

## Dashboard

We have developed a live dashboard to allow people to visualize descriptive statistics and preliminary results. It is available here: https://osome.iu.edu/tools/covaxxy

Complimentary data sources used by the CoVaxxy dashboard:

* Vaccination data from the Centers for Disease Control and Prevention data found [here](https://covid.cdc.gov/covid-data-tracker/#vaccinations), as compiled by Our World in Data [here](https://github.com/owid/covid-19-data/blob/master/public/data/vaccinations/us_state_vaccinations.csv).
* Vaccine acceptance and refusal data from Carnegie Mellon University's [Delphi Epidata API](https://cmu-delphi.github.io/delphi-epidata/api/covidcast-signals/fb-survey.html#vaccination-indicators) survey data, created by the [Delphi Research Group](https://delphi.cmu.edu/about/).

VaccinItaly:
 * A member of the CoVaxxy team, [Francesco Pierri](https://frapierri.github.io), has also developed the [VaccinItaly dashboard](http://genomic.elet.polimi.it/vaccinitaly/) which is similar to CoVaxxy. This dashboard, however, specifically monitors Italian conversations around vaccines on Facebook and Twitter.  

## Team

* [Matthew R. DeVerna](https://www.matthewdeverna.com/), [Bao Truong](https://btrantruong.github.io/), [John Bollenbacher](https://jbollenbacher.github.io/), [David Axelrod](https://cns-nrt.indiana.edu/students/trainees/2019/David-Axelrod.html), [Cristopher Torres-Lugo](http://christorreslugo.com/), [Kai-Cheng Yang](http://www.kaichengyang.me/), [Fil Menczer](https://cnets.indiana.edu/fil/), [John Bryden](http://jbryden.co.uk/home/) *([Observatory on Social Media](https://osome.iu.edu/), Indiana University)* 
* [Francesco Pierri](https://frapierri.github.io) *(Department of Electronics, Information and Bioengineering, Politecnico di Milano)* 
* Niklas Loynes *(School of Social Sciences, University of Manchester)*

## Acknowledgments

This project is supported in part by the Knight Foundation and Craig Newmark Philanthropies. We used the Extreme Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number ACI-1548562.
