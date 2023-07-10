# TRADISAN
This repo contains the first version of TRADISAN ("conTRAstare la DIsinformazione in ambito SANitario tramite fake news detection sui social media"), a dataset developed for the Italian language to assess health-related news reliability. It is part of a research project which bears the same name, and is funded by Consortium GARR, the Italian National Research and Education Network.

The current dataset consists in 32.100 headlines, each provided with automatic annotations of 31 news reliability features, including stylometric, lexical and sentiment features. Furthermore, each headline has additional annotations, i.e., lemmas, POS, IOB and NER. We release the dataset in tab-separated values (TSV) format. 

| id | source | date | url | headline | char_count | ... | ner |
| -- | ------ | ---- | --- | -------- | ---------- | --- | --- |
| 3409 | la Repubblica | 2023-01-17 00:00:00 | ... | Così il digiuno modifica il cervello | 31 | ... | ['O', 'O', 'O', 'O', 'O', 'O'] |
| 15526 | ByoBlu | 2022-09-21 00:00:00 | ... | “BILL GATES HA GESTITO IL COVID PER ARRICCHIRSI”: ORA SE NE ACCORGE ANCHE IL MAINSTREAM | 73 | ... | ['O', 'MISC', 'MISC', 'O', 'MISC', 'O', 'ORG', 'O', 'ORG', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'MISC'] |

The dataset is released under Creative Commons license CC BY-NC-SA.

To cite this work:

Giordano, Luca and di Buono, Maria Pia. 2023.  Assessing Italian News Reliability in the Health Domain through Text Analysis of Headlines. In Proceedings of the 1st International Workshop on Disinformation and Toxic Content Analysis (DiTox 2023) - Language Data and Knowledge 2023.
