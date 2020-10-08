# Party manifestos

## Requirements

An account on the Google Cloud platform (GCP) and following the setup process described in: https://cloud.google.com/translate/docs/setup

Files in the current working directory:
* manifestos_parlgov_linktable.csv
* JSON file containing the GCP service account key 

Language/modules:
* Python 3
* nltk
* textblob
* wordcloud
* statsmodels
* google-cloud-translate
* numpy
* pandas
* matplotlib
* seaborn
* os
* requests
* json
* sqlite3
* re
* math
* collections

## Aim of the project

The aim of this project is to analyze how the strength of populist radical right parties affect the attitude of parties in government towards international cooperation. In particular, it analyzes party manifestos with respect to their sentiment towards international cooperation and the frequencies of words related to international cooperation.<br>
The core data and the texts of the party manifestos are retreived from the Manifesto Project API (https://manifesto-project.wzb.eu/information/documents/api). Data on the strength of populist radical right parties in the respective countries (vote share, seats share) come from the ParlGov database (http://www.parlgov.org/) and parties are defined as right-wing populist according to the PopuList classifcation (https://popu-list.org).<br>
The single steps are described in the notebook party_manifestos.ipynb.

### Table of contents
1. Importing the modules required
1. Collecting the data from the ParlGov database and the Manifesto Project API (core dataset)
2. Merging and processing the data
3. Visualization: diagrams on trends and populist radical right vs. other/government parties
4. Estimation of the effect of the strength of populist radical right parties on the attitude of government parties towards international cooperation
5. Fetching the party manifestos and text translation (Manifesto Project and Google Translate API)
6. Creating word clouds for word frequencies in party manifestos
