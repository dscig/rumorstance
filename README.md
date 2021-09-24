# The RumorStance Project

The data used in two papers "The presence of unexpected biases in online fact-checking" and "An Experimental Study to Understand User Experience and Perception Bias Occurred by Fact-checking Messages" after being anonymized for the reproducibility of research outcomes.

The first paper has been published in the Harvard Kennedy School Misinformation Review (https://doi.org/10.37016/mr-2020-53); the extended second one was presented at the Web Conference in April 2021 (https://doi.org/10.1145/3442381.3450121).

##### Please cite as:
Park S, Park Y, Kang J, and Cha M <br>
The presence of unexpected biases in online fact-checking <br>
Harvard Kennedy School Misinformation Review, doi.org/10.37016/mr-2020-53. 2021. <br>

or

##### Please cite as:
Park S, Park JY, Chin H, Kang JH, and Cha M <br>
An Experimental Study to Understand User Experience and Perception Bias Occurred by Fact-checking Messages <br>
In Proceedings of the Web Conference 2021 (pp.2769-2780), doi.org/10.1145/3442381.3450121. April, 2021. <br>


### Data Description

#### 1. Overview
```
- System used to conduct experiments simulating online news consumption environments: Amazon Mechanical Turk (https://www.mturk.com/)
- Dataset pre-processed and refined: download rumorstance_response_clean.csv
- Total number of respondents (# of rows in the dataset): 11,145
```

#### 2. Feature codes
The below table is the tested rumors drawn from the unconfirmed list of claims on Snopes.com.

<img src="./source/table_tested_rumors.png">

Please find the detailed explanation of the codes below for each feature.
```
claim:
- The tested rumors drawn from the unconfirmed list of claims on Snopes.com, the values are in (1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
- Each value corresponds to the codes in the table above

prestance: 
- The degree of the initial view towards a given unproven claim, the values are in (-2, -1, 0, 1, 2), which is a 5-point Likert scale
- Each value corresponds to the following view: (Definitely False, Somewhat False, Middle-of-the-road, Somewhat True, Definitely True) 

condition: 
- The hypothetical fact-checking conditions (i.e., messages/tags) provided to respodents towards a given claim, the values are in (1, 2, 3, 4, 5, 6)
- Each value corresponds to the following condition: (None, Mostly True, Mostly False, Mixed Evidence, Divided Evidence, Lack of Evidence)

see_t: 
- The degree to be OK with seeing a given claim on Twitter-like social media timeline, the values are in (-2, -1, 1, 2)
- Each value corresponds to the following degree: (Definitely Not OK, OK, Definitely OK)

see_f: 
- The degree to be OK with seeing a given claim on Facebook-like social media newsfeed, the values are in (-2, -1, 1, 2)
- Each value corresponds to the following degree: (Definitely Not OK, OK, Definitely OK)

see_m: 
- The degree to be OK with seeing a given claim on instant messangers like WhatsApp, the values are in (-2, -1, 1, 2)
- Each value corresponds to the following degree: (Definitely Not OK, OK, Definitely OK)

see_e: 
- The degree to be OK with seeing a given claim on emails, the values are in (-2, -1, 1, 2)
- Each value corresponds to the following degree: (Definitely Not OK, OK, Definitely OK)

share_t: 
- The degree of willingness to share a given claim through Twitter-like social media timeline, the values are in (-2, -1, 1, 2)
- Each value corresponds to the following degree: (Definitely No, No, Yes, Definitely Yes)

share_f: 
- The degree of willingness to share a given claim through Facebook-like social media newsfeed, the values are in (-2, -1, 1, 2)
- Each value corresponds to the following degree: (Definitely No, No, Yes, Definitely Yes)

share_m: 
- The degree of willingness to share a given claim through instant messangers like WhatsApp, the values are in (-2, -1, 1, 2)
- Each value corresponds to the following degree: (Definitely No, No, Yes, Definitely Yes)

share_e: 
- The degree of willingness to share a given claim through emails, the values are in (-2, -1, 1, 2)
- Each value corresponds to the following degree: (Definitely No, No, Yes, Definitely Yes)

poststance: 
- The degree of the subsequent view towards a given unproven claim after checking the fact-checking message, the values are in (-2, -1, 0, 1, 2), which is a 5-point Likert scale
- Each value corresponds to the following view: (Definitely False, Somewhat False, Middle-of-the-road, Somewhat True, Definitely True)

yearborn: 
- The year when each respondent was born, the values are in (1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20)
- Each value corresponds to the following year: (1981 or earlier, 1982, 1983, 1984, 1985, 1986, 1987, 1988, 1989, 1990, 1991, 1992, 1993, 1994, 1995, 1996, 1997, 1998, 1999, 2000 or later)

gender: 
- male: 1; female: 2
```

#### 3. Validity of the Data
In many cases, survey results are bound to multiple errors, and therefore we report some of the verification processes we took to ensure the validity of results. The Chi-squared test of independence identified that fact-checking conditions were randomly distributed across the ten rumor claims. No significant interaction was
observed between the assigned conditions and claims (𝜒2=44.21, df=45, p=0.51), and one-way ANOVA for pre-stance did not find any significant difference across the six states (F=0.77, p=0.57). We also checked what fraction of the respondents always picked the first (or the left-most) choices throughout the survey. This resulted in 0.35% (39/11,145) of all subjects, which is a negligible proportion. When choosing the ten claims, we tried to find topics of general interest. However, some topics may be more intuitive to understand than others, causing external validity problems. The users’ total response time was observed to identify any bias in perception difficulty across the claims and to check whether users took a reasonable amount of time on the survey. The total distribution of time spent on the survey is skewed. Most turkers completed their tasks within 10 minutes (98.80%) and the median time taken was 96 seconds, but a small fraction took a disproportionately large amount of time (e.g., several hours). Nonetheless, 99 percent completed the task within 12.2 minutes. Examining those users who took significantly long sessions, we find no correlation between the time spent and claims (𝜒2=8.08, df=9, p=0.53). <br>

Should you have any questions or comments, please contact us at the following email address: shaun01.park@gmail.com.

<end of document>
