# The RumorStance Project

The data used in the paper "The presence of unexpected biases in online fact-checking" after being anonymized for the reproducibility of research outcomes.

The paper will be published in the Harvard Kennedy School Misinformation Review (https://misinforeview.hks.harvard.edu/) shortly.

##### Please cite as:
Park S, Park Y, Kang J, and Cha M <br>
The presence of unexpected biases in online fact-checking <br>
Harvard Kennedy School Misinformation Review, to be published in 2021. <br>

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

Please find the detailed codes for each feature:
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

poli: 
- the political orientation, the values are in (1, 2, 3, 4, 5)
- Each value corresponds to the following orientation: (Vert Liberal, Liberal, Middle-of-the-road, Conservative, Very conservative)

ethnicity: 
- The values are in (1, 2, 3, 4, 5): respondents can choose multiple answers
- Each value corresponds to the following ethnicity: (Asian/Pacific Islander, Black, White, Native American/Alaska Native, Exclusive/None of the Above)
```

Should you have any questions or comments, please contact us at the following email address: shaun01.park@gmail.com. <br> <br>

< end of document >
