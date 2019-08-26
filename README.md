# viNLaP: Visualizing polarized data sources

This project was conceived due to the need of visualize polarized data easily and effectively. The first version of vinLAp aims to show an overview of the MAGA corpus, crawled in GSoC 2018 by Maja Goudoz- For doing so, it focuses on three aspects. These aspects are: variability of the vocabulary by each side using Scattertexts, speech production by geographic regions using GeoSpeech and, speech generation analysis from a specific word using Speech Igniters.

## Getting Started

Clone this repository to your local machine.

### Prerequisites

This project runs with Python 3.7. We use Jupyter notebooks for the development of each aspect, to create everything dynamically. 

Install the following dependencies:

```
pip install pandas 
pip install seaborn 
pip install unicodedata
pip install nltk
pip install numpy
pip install networkx
pip install matplotlib
pip install scattertext
pip install tweepy
pip install datetime
pip install quantiphy
```

## Structure of the repo

In [data](/data), you will find:

### [tweets_maga](/data/tweets_maga.json) 

This dataset is a extension of the previous colleted MAGA corpus. It has the complete json object of each tweet. We hope this data will help other research in the future.

In [notebooks](/notebooks), you will find 4 jupyter notebooks:

### [GeoSpeech](/notebooks/GeoSpeech.ipynb) 

GeoSpeech contains two scripts. The first one will help you to crawl the complete json of a set of tweets' ids. This was used to get  [tweets_maga](/data/tweets_maga.json) . The second one will get the locations of the tweets even though they are not geolocated.

### [Exploratory Data Analysis](/notebooks/MAGA Corpus - Exploratory Data Analysis.ipynb) 

This notebook will give you an overview of the data we are working with. We consider useful for any tabular dataset you have. You will fins data distributions, unique themes, frequencies, etc.

### [ScattertextGenerator](/notebooks/Scattertext Generator.ipynb) 

ScattertextGenerator contains the main script of the project. It has a plug-n-play function to generate scattertexts as the ones in [results](/results) . 

### [SpeechIgniters](/notebooks/SpeechIgniters.ipynb) 

GeoSpeech contains two scripts. The first one will preprocess the text of each tweet in order to get the tokens for the word chains. The seconf script will use network graphs theory to create a function to obtain all the words related to a specific word of the dataset.

In [results](/results), you will find:

The scattertexts from our case of study's dataset.


## Authors

* **Fabricio Layedra** - *GSoC 2019 Student with CLiPS* - [PurpleBooth](https://github.com/FabricioLayedra)

## Acknowledgments

* **CLiPS** - *Supervision* - [PurpleBooth](https://www.uantwerpen.be/en/research-groups/clips/research/publications/)
* **ESPOL University Big Data Research Club** - *Supervision* - [PurpleBooth](http://www.espol.edu.ec/es/ingestigacion/grupos-de-investigacion/big-data)


