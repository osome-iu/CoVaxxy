# CoVaxxy: A global collection of English Twitter posts about COVID-19 vaccines #

The goal of this project is to investigate the impact of online information on COVID-19 vaccine uptake and health outcomes. <br>
Reference paper(s): <br>
DeVerna, Matthew, Francesco Pierri, Bao Tran Truong, John Bollenbacher, David Axelrod, Niklas Loynes, Cristopher Torres-Lugo, Kai-Cheng Yang, Fil Menczer, and John Bryden. **"CoVaxxy: A global collection of English Twitter posts about COVID-19 vaccines."** arXiv preprint arXiv:2101.07694 (2021) https://arxiv.org/abs/2101.07694

# Data
To create as complete a set of Twitter posts related to COVID-19 vaccines as possible, we carefully select a list of keywords through a snowball sampling technique. We start with the two most relevant keywords, i.e., `covid` and `vaccine`, as our initial seeds.
Next, we gather tweets utilizing the filtered stream endpoint of the Twitter API for three hours. From these gathered tweets, we then identify potential keywords that frequently co-occur with the seeds, adding them to our seed list only after manually ensuring they are closely related to our topic. This process was repeated six times between Dec. 15, 2020 and Jan. 2, 2021 with each iteration's data collection taking place at different times of the day to capture tweets from different geographic areas and demographics. The seed list serves as our initial keyword list.

We further refine the keyword list by manually combining certain keywords into composites (e.g.`covid19 pfizer`), as a way to ensure that the dataset is broad enough to include most relevant (English) conversations while excluding tweets that are not related to the vaccine discussion. 

Some notes on the query syntax of Twitter's filtered stream API: 
- Queries that include keywords also match hashtags, URLs, and substrings. For example, `covid` matches `cnn.com/covid` and `#covid19`.
- Using `covid19 pfizer` as a composite matching phrase will capture tweets that contain `covid19` *and* `pfizer`. On the other hand, including `covid19`,`pfizer` as separate keywords will capture tweets that contain `covid19` *or* `pfizer`.

More details on the list of final (single or composite) keywords used to collect Twitter data can be found in our paper describing [the collection of English-language Twitter posts about COVID-19 vaccines](https://arxiv.org/abs/2101.07694). If you use this data please cite the reference paper(s) above.

# Dashboard
We have developed a live dashboard to allow people to visualize descriptive statistics and preliminary results. It is available here: https://osome.iu.edu/tools/covaxxy

# Team
Our team is affiliated with The Observatory on Social Media at Indiana University. In future work related to COVID-19 vaccines, we intend to explore the relationship be-tween online discussion of COVID-19 vaccines and publichealth outcomes, like COVID-19 mortality and vaccine up-take.  We  will  also  leverage  existing  social  media  analysistools to track emerging narratives and suspicious accounts,such as bots, coordinated campaigns, and troll farms.

Members: 
* Matthew Deverna, Bao Tran Truong, John Bollenbacher, David Axelrod, Cristopher Torres-Lugo, Kai-Cheng Yang, Fil Menczer, John Bryden *(Observatory on Social Media, Indiana University)* <br>
* Francesco Pierri *(Department of Electronics, Information and Bioengineering, Politecnico di Milano)* <br>
* Niklas Loynes *(School of Social Sciences, University of Manchester)*

About OSoMe: 
The Observatory on Social Media (OSoMe, pronounced awe•some) is a joint project of the Network Science Institute ([IUNI](https://iuni.iu.edu/)), the Center for Complex Networks and Systems Research ([CNetS](https://cnets.indiana.edu/)) at the School of Informatics, Computing, and Engineering ([SICE](https://luddy.indiana.edu/)), and the [Media School](https://mediaschool.indiana.edu/) at Indiana University. 
The OSoMe mission:

> Transform the study of coupled media and technology networks that drive the diffusion of information. Offer access to data and tools to investigate the diffusion of (mis)information, uncover the vulnerabilities of the media ecosystem, and develop methods for increasing the resilience of citizens and democratic systems to manipulation. Train a generation of media professionals, enabling them to employ computational skills for fulfilling the traditional watchdog function of journalism. Our ambition is to position future reporters to uncover newsworthy information that is otherwise invisible to public scrutiny and empower citizens to navigate their way to informed participatory behavior.
# Acknowledgments
