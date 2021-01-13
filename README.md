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
- Dataset pre-processed and refined: rumorstance_response_clean.csv
- Total number of respondents (# of rows in the dataset): 11,145
```

#### 2. Feature codes
The below table is the tested rumors drawn from the unconfirmed list of claims on Snopes.com.

<img src="./source/table_tested_rumors.png">

Please find the detailed codes for each feature:
```
claim:
- The tested rumors drawn from the unconfirmed list of claims on Snopes.com.
- The values are from 1 to 10. The corresponding codes can be found in the table above.

prestance: 
- The initial view towards a given unproven claim by respondent.
- The values are in (-2, -1, 0, 1, 2), which is a 5-point Likert scale.

condition: 
- 


see_t: 
- 


see_f: 
- 


see_m: 
- 


see_e: 
- 


share_t: 
- 


share_f: 
- 


share_m: 
- 


share_e: 
- 


poststance: 
- 
- The values are in (-2, -1, 0, 1, 2), which is a 5-point Likert scale.

yearborn: 
- 


gender: 
- 


poli: 
- 


ethnicity: 
- 

```

Should you have any questions or comments, please contact us at the following email address: shaun01.park@gmail.com. <br> <br>

<end of document>
