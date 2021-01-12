# The RumorStance Project

The data used in the paper "The presence of unexpected biases in online fact-checking" after being anonymized for the reproducibility of research outcomes.

The paper will be published in the Harvard Kennedy School Misinformation Review (https://misinforeview.hks.harvard.edu/) shortly.

##### Please cite as:
Park S, Park Y, Kang J, and Cha M <br>
The presence of unexpected biases in online fact-checking <br>
Harvard Kennedy School Misinformation Review, to be published in 2021. <br>

### Data Description
```
- Total number of respondents (# of rows) : 11,145


[South Korea]
- corona: 코로나
- wuhan pneumonia: 우한 폐렴

[Iran]
- corona: #کرونا
- coronavirus: #کروناویروس
- wuhan: #ووهان
- pneumonia: #سینه‌پهلو

[Vietnam]
- corona
- n-cov
- covid
- acute pneumonia: viêm phổi cấp

[India]
- corona: कोरोना
- wuhan pneumonia: वूहान निमोनिया
```

Also, Below are the column names (features) and the corresponding descriptions of the dataset:

```
- id (type == int64): The integer representation of the unique identifier for this Tweet
- conversation_id (int64): The Tweet ID of the conversation tree’s root
- created_at (datetime64): UTC time when this Tweet was created
- date (datetime64): UTC time formatted YYYY-MM-DD
- time (object): UTC time formatted h:m:s
- timezone (object): Timezone
- user_id (int64): The integer representation of the unique identifier for this User
- username (object): The screen name, handle, or alias that this user identifies themselves with
- name (object): The name of the user, as they’ve defined it
- place (object): Nullable When present, indicates that the tweet is associated (but not necessarily originating from) a Place
- tweet (object): The actual UTF-8 text of the status update
- mentions (object): Represents other Twitter users mentioned in the text of the Tweet
- urls (object): Represents URLs included in the text of a Tweet
- photos (object): Represents photo elements uploaded with the Tweet
- replies_count (int64): Number of times this Tweet has been replied to
- retweets_count (int64): Number of times this Tweet has been retweeted
- likes_count (int64): Nullable. Indicates approximately how many times this Tweet has been liked by Twitter users
- hashtags (object): Represents hashtags which have been parsed out of the Tweet text
- video (int64): The number of video elements uploaded with the Tweet
- geo (object): Nullable. Represents the geographic location of this Tweet as reported by the user or client application
- source (object): Utility used to post the Tweet, as an HTML-formatted string
- reply_to (object): Reply infos containing user_id and username
```

Deprecated Attributes:

```
- cashtags (object)
- quote_url (object)
- near (object)
- retweet (bool)
- user_rt_id (object) 
- user_rt (object)
- retweet_id (object) 
- retweet_date (object) 
- translate (object) 
- trans_src (object)
- trans_dest (object)
```


### Pipeline
Please refer to the manuscript to find the detailed explanations for the below four modules.

![](./image/pipeline_topic_model.png)

```
[Required Basic Packages]
The code has been tested running under Python 3.6.6. with the following packages installed (along with their dependencies):
- numpy == 1.16.0
- pandas == 0.23.4
```

#### 1. Pre-processing Data
For the detailed tweet pre-processing and tokenizing process, please refer to the below file including code snippet and corresponding explanation:
- "./code/code_text_preprocessing_tokenization.pdf"

```
[South Korea]
We have used the below Korean-specific stopwords and tokenizers.
- pre-processing
  - text cleaning: removed special characters and URLs  
  - stopwords: find "./code/korean_stopwords.txt"
- tokenizing: utilized the MeCab-Ko tokenizer (http://eunjeon.blogspot.com/)
- Please refer to the following code snippet file to find an example usage case: "./code/code_Korean_tokenize_sentences.pdf"

[Iran]
We have used the below Farsi-specific stopwords and tokenizers.
- pre-processing
  - text cleaning: removed special characters and URLs
  - stopwords: find "./code/farsi_stopwords.txt"
- tokenizing: utilized the Parsivar tokenizer (https://github.com/ICTRC/Parsivar)
- Please refer to the following code snippet file to find an example usage case: "./code/code_Persian_tokenize_sentences.py"

[Vietnam]
We have used the below Vietnamese-specific stopwords and tokenizers.
- pre-processing
  - text cleaning: removed special characters and URLs  
  - stopwords: find "./code/vietnamese_stopwords.txt"
- tokenizing: utilized the Pyvi tokenizer (https://github.com/trungtv/pyvi)
- Please refer to the following code snippet file to find an example usage case: "./code/code_Vietnamese_tokenize_sentences.pdf"

[India]
We have used the below Hindi-specific stopwords and tokenizers.
- pre-processing
  - text cleaning: removed special characters, non-Hindi characters/words, and URLs
  - stopwords: find "./code/hindi_stopwords.txt"
- tokenizing: utilized word-level morphemes as tokens
```

Should you have any questions or comments, please contact us at the following email address: shaun01.park@gmail.com. <br> <br>

< end of document >
