## Data Source: CORONAVIRUS (COVID-19) GEO-TAGGED TWEETS DATASET from IEEE Portal

#### ABSTRACT 
This dataset contains IDs and sentiment scores of geo-tagged tweets related to the COVID-19 pandemic. The real-time Twitter feed is monitored for coronavirus-related tweets using 90+ different keywords and hashtags that are commonly used while referencing the pandemic. Complying with Twitter's content redistribution policy, only the tweet IDs are shared. The tweet IDs in this dataset belong to the tweets created providing an exact location. You can re-construct the dataset by hydrating these IDs. For detailed instructions on the hydration of tweet IDs, please read this medium article.

#### Related publications:
Lamsal, R. (2021). Design and analysis of a large-scale COVID-19 tweets dataset. Applied Intelligence, 51(5), 2790-2804.
Lamsal, R., Harwood, A., & Read, M. R. (2022). Socially Enhanced Situation Awareness from Microblogs using Artificial Intelligence: A Survey. ACM Computing Surveys.

- Dataset name: GeoCOV19Tweets Dataset
- Number of tweets : 482,220 tweets
- Coverage : Global
- Language : English (EN)
- Our Selection: 2021_01 - 2022_05

#### Data Set Citation:
Lamsal, R. Design and analysis of a large-scale COVID-19 tweets dataset. Appl Intell 51, 2790–2804 (2021). https://doi.org/10.1007/s10489-020-02029-z

BibTeX:
```
@article{lamsal2021design,
title={Design and analysis of a large-scale COVID-19 tweets dataset},
author={Lamsal, Rabindra},
journal={Applied Intelligence},
volume={51},
number={5},
pages={2790--2804},
year={2021},
publisher={Springer}
}
```

#### Hydration
To hydrate the tweet IDs, we use Hydrator:

Getting the CSV files of this dataset ready for hydrating the tweet IDs: https://github.com/DocNow/hydrator
```
import pandas as pd
dataframe=pd.read_csv("april28_april29.csv", header=None)
dataframe=dataframe[0]
dataframe.to_csv("ready_april28_april29.csv", index=False, header=None)
```

