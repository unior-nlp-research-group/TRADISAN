# TRADISAN
This repo contains the first version of TRADISAN ("conTRAstare la DIsinformazione in ambito SANitario tramite fake news detection sui social media"), a dataset developed for the Italian language to assess health-related news reliability. It is part of a research project which bears the same name, and is funded by Consortium GARR, the Italian National Research and Education Network.

The current dataset consists in 32.100 headlines, each provided with automatic annotations of 31 news reliability features, including stylometric, lexical and sentiment features. Furthermore, each headline has additional annotations, i.e., lemmas, POS, IOB and NER. We release the dataset in tab-separated values (TSV) format. 

| id | source | date | url | headline | char_count | ... | ner |
| -- | ------ | ---- | --- | -------- | ---------- | --- | --- |
| 20861 | VoxNews | 2020-03-18 00:00:00 | ... | Voi chiusi in casa: il governo scarcera 12mila criminali | 48 | ... | ['O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O] |


The dataset is released under Creative Commons license CC BY-NC-SA.

To cite this work:

Giordano, Luca and di Buono, Maria Pia. 2023.  Assessing Italian News Reliability in the Health Domain through Text Analysis of Headlines. In Proceedings of the 1st International Workshop on Disinformation and Toxic Content Analysis (DiTox 2023) - Language Data and Knowledge 2023.
