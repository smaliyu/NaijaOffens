# NaijaHate: Offensive Language and Hate Speech Detection in Nigerian Languages

## Introduction
NaijaHate is a pioneering project aimed at addressing the growing problem of online offensive and hate speech in Nigeria. This project introduces the first labeled dataset for offensive and hate speech detection in three major Nigerian languages. Our goal is to aid in content moderation, social media monitoring, and threat evaluation through machine learning tools.

## Table of Contents
- [Project Description](#project-description)
- [Dataset](#dataset)
- [Lexicon](#lexicon)
- [Model Training](#model-training)
- [Research Paper](#research-paper)
- [Project Sponsors](#project-sponsors)
- [License](#license)
- [Contact](#contact)

## Project Description
The Offensive and Hate Speech Detection Project aims to tackle the pervasive issue of offensive and hateful content circulating in Nigeria's digital spaces. Leveraging state-of-the-art Natural Language Processing (NLP) techniques, the project seeks to develop robust algorithms and tools capable of automatically identifying and mitigating instances of hate speech across the three major languages spoken in Nigeria.

### Challenges Faced in Nigeria and the Role of Hate Speech Detection Projects

1. **Cultural Diversity**: Nigeria boasts over 250 ethnic groups, each with distinct languages and customs. This diversity can sometimes lead to tensions exacerbated by offensive or hateful speech. Offensive and Hate speech detection projects can help identify and mitigate such instances, fostering understanding among Nigeria's diverse population.

2. **Linguistic Variation**: With over 500 languages spoken, linguistic diversity poses a challenge for automated text analysis. Hate speech detection models must accurately identify offensive language across multiple languages and dialects, necessitating development in various Nigerian languages.

3. **Legal and Regulatory Framework**: Nigeria has laws against hate speech, but enforcement can be difficult, especially online. Hate speech detection projects can complement legal frameworks by aiding in the identification and reporting of hate speech instances, supporting law enforcement efforts.

4. **Ethical Considerations**: Hate speech detection projects must navigate ethical issues including privacy, censorship, and bias. Algorithms must be fair, transparent, and culturally sensitive, ensuring that legitimate expression is not suppressed.

## Dataset

The NaijaHate dataset is a dedicated effort to curate a comprehensive dataset for hate speech detection across three major Nigerian languages: Hausa, Yoruba, and Igbo. The datasets wer made up of tweets sollceted from Twitter now X, using the Twitter Academic API. We collected and annotated potentially harmful tweets in the Nigerian social media space. The statistics of annotated tweets per language is shown in the table below:

| Language | No. of tweets |
| --------- | ------------- |
| Hausa    | 6697 |
| Igbo      | 5452 |
| Yoruba    | 5001 |
        



 By providing this dataset, we aim to facilitate research and development in the field of natural language processing, specifically in the context of hate speech detection in African languages.

The dataset is freely available for researchers and can be accessed for academic and research purposes. This project aims to promote a safer online environment.


Link to dataset: [Dataset](https://github.com/smaliyu/NaijaHate/tree/main/Datasets)


## Lexicon
At the outset of the NaijaHate project, we curated hate speech lexicons for each of the major Nigerian languages. These lexicons played a crucial role in our data collection process, particularly in the collection of tweets in all the languages. The lexicons are comprehensive and tailored to the linguistic nuances of each language, ensuring effective identification of offensive and hate speech.

You can access the lexicons for all the languages in the [Lexicons folder](https://github.com/smaliyu/NaijaHate/blob/main/Data%20Sampling%20strategy_.pdf).

## Model Training
We focused on training four distinct models to analyze tweet datasets in three major Nigerian languages: Hausa, Igbo, and Yoruba. This endeavor involved a standardized PyTorch workflow, complemented by the extensive model repository available on Huggingface. The choice of Huggingface facilitated the use of advanced NLP models, each with its unique architecture but primarily encoder-based, similar to BERT.

To manage our language-specific datasets effectively, we developed a custom dataset class. This class was tailored to the unique characteristics of the Hausa, Igbo, and Yoruba languages, addressing specific text preprocessing and encoding needs. The use of PyTorch’s DataLoader was instrumental in handling the data efficiently in batches, optimizing computational resources.

A critical component of our methodology was leveraging AutoModel and AutoTokenizer classes from Huggingface. These tools enabled us to accommodate various model architectures seamlessly. AutoModel adapted dynamically to each model’s architecture, while AutoTokenizer ensured consistent and appropriate tokenization and encoding of our multilingual text data. This approach was particularly beneficial given the linguistic nuances of Hausa, Igbo, and Yoruba tweets.

The overarching aim of training these models was to distinguish and learn the class-specific features inherent in the tweet datasets of these three languages. By utilizing pretrained models and fine-tuning them on our datasets, we were able to harness pre-existing knowledge and adapt it to the context of Nigerian languages.

Finally, we evaluated the performance of each model on separate test sets for Hausa, Igbo, and Yoruba tweets. This evaluation primarily measured the models' accuracy, offering vital insights into their effectiveness in classifying tweets accurately across these languages.
  
## Research Paper

We have successfully published a paper titled "" that details the methodologies, findings, and implications of our project. This paper serves as a cornerstone in our efforts to understand and combat online hate speech in Nigerian languages. Link to the published paper: [Published Paper](<link-to-published-paper>)


We are also excited to announce that have submitted a paper titled "BEYOND ENGLISH: OFFENSIVE LANGUAGE DETECTION IN LOW-RESOURCE AFRICAN LANGUAGES", which aims to build upon our initial findings and explore new dimensions of hate speech detection. Here is the 


## Project Sponsors 
![DSA logo](DSA_logo.jpg)

We express our profound gratitude to Data Science Africa for their generous support in funding this project. Their commitment to advancing data science and machine learning across Africa has been instrumental in making NaijaHate a reality. This grant has enabled us to tackle the critical issue of hate speech in Nigerian languages, fostering a safer online environment.


## Contact 

For additional information, inquiries, or collaboration opportunities related to the NaijaHate project, please feel free to reach out to our Project Lead, Saminu Mohammad Aliyu. He can be contacted via email at [saminualiyu@gmail.com](mailto:saminualiyu@gmail.com). Your interest and support for our initiative are greatly appreciated, and we look forward to engaging with the community.
