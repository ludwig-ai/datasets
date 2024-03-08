# Motivation
Open Source Datasets to Use for Demonstrating Ludwig Capabilities

# Background

These datasets are obtained from public sources, such as Kaggle, HuggingFace, and individual GitHub repositories.  In certain situations, this repository contains conditioned (e.g., cleaned) versions of the corresponding original datasets.

# Usage Pattern

For example, the dataset can now be accessed as "https://raw.githubusercontent.com/ludwig-ai/datasets/main/TLDRNews/tldr_news_full.csv.gz" and loaded into a Pandas DataFrame using:
```
>>> import pandas as pd
>>> df_dataset: pd.DataFrame = pd.read_csv(filepath_or_buffer="https://raw.githubusercontent.com/ludwig-ai/datasets/main/TLDRNews/tldr_news_full.csv.gz", compression="gzip")
>>> df_dataset.shape
(7932, 4)
>>> df_dataset.head(n=5)
   split                                           headline                                            content  category
0      0  NASAâs Ingenuityâthe First Ever Off-World Heli...  NASA's Perseverance rover will be carrying a f...         2
1      0  Huge space hotel promises fake gravity and 'su...  Space hotels will soon become a reality, with ...         2
2      0                             Pomerium (GitHub Repo)  Pomerium is an identity-aware proxy that enabl...         3
3      0  Tech Lead Expectations for Engineering Project...  This document contains a guide on being an eng...         3
4      0  Who was Fahim Saleh, the tech CEO brutally dis...  Fahim Saleh was a tech entrepreneur who lived ...         4
>>> 
```

Hence, it will no longer be necessary to upload datasets into Google Drive and mount the drive in Colab notebooks.

# Acknowledgments / Credits / References
* TLDRNews - obtained from [https://huggingface.co/datasets/JulesBelveze/tldr_news](https://huggingface.co/datasets/JulesBelveze/tldr_news), thanks to a gracious permission by the author, [Jules Belveze](https://www.linkedin.com/in/jules-belveze/).
