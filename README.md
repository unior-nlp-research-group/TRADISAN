# TRADISAN
This repo contains the first version of **TRADISAN** ("conTRAstare la DIsinformazione in ambito SANitario tramite fake news detection sui social media"), **a dataset developed for the Italian language to assess health-related news reliability**. It is part of a research project which bears the same name, and is funded by Consortium GARR, the Italian National Research and Education Network.

The current dataset consists of **32,101 news**. We provide each headline with automatic annotations of **31 news reliability features, including stylometric, lexical and sentiment features**. Furthermore, each headline has **4 additional annotations**, i.e., **lemmas, POS, IOB and NER**. We release the dataset and headline features in tab-separated values (TSV) format (note: the dataset is compressed in a split zip file, i.e. zip and z01). Annotations for news body text are not yet available.

The 31 features are:
- **STYLOMETRIC**
  - **char_count** = number of characters
  - **uppercase_word_w** = number of words written in uppercase weighted for total number of words
  - **long_w_w** = number of words longer than six characters weighted for total number of words
  - **consecutive_question_count** = number of occurrences of consecutive question marks
  - **consecutive_excla_count** = number of occurrences of consecutive exclamation marks
  - **quotes_count** = number of quotes
  - **dou_quotes_count** = number of double quotes
  - **single_quote_count** = number of single quotes
  - **ellipses_count** = number of ellipses
  - **direct_discourse** = number of direct discourse (defined as a colon followed by double quotation marks)
  - **typo_count_w** = number of typos weighted for total number of words
- **LEXICAL**
  - **adverb_count_w** = number of adverbs weighted for total number of words
  - **comp_w** = number of comparatives weighted for total number of words
  - **superl_count_w** = number of superlatives weighted for total number of words
  - **currency_w** = number of currency-related words weighted for total number of words
  - **rev_hurtlex_count_w** = number of words present in the HurtLex lexicon weighted for total number of words
  - **hurtlex_score** = total HurtLex score computed
  - **neg_adverbs_count_w** = number of negative adverbs weighted for total number of words
  - **noun_count_w** = number of nouns weighted for total number of words
  - **prop_noun_count_w** = number of proper nouns weighted for total number of words
  - **adj_count_w** = number of adjectives weighted for total number of words
  - **adj_poss_others_w** = number of possessive adjectives other than 1st and 2nd person weighted for total number of words
  - **1st_pers_sing_w** = number of 1st personal singular pronouns weighted for total number of words
  - **2nd_pers_sing_w** = number of 2nd personal singular pronouns weighted for total number of words
  - **digits_w** = number of digits weighted for total number of words
  - **buzzwords_count_w** = number of buzzwords weighted for total number of words
- **SENTIMENT**
  - **nrc_anger_w** = number of anger-related words weighted for total number of words
  - **nrc_trust_w** = number of trust-related words weighted for total number of words
  - **nrc_joy_w** = number of joy-related words weighted for total number of words
  - **opos** = positive polarity value computed
  - **oneg** =  negative polarity value computed

 The 4 additional annotations are:
 - **lemmas** = a list of lemmatized tokens (without puntuation)
 - **pos** = Part-of-speech tagging 
 - **iob** = Inside-Outside-Beginning chunk-tagging
 - **ner** = Named Entity Recognition tagging

| id | source | date | url | headline | char_count | ... | oneg | lemmas | ... | ner |
| -- | ------ | ---- | --- | -------- | ---------- | --- | ---- | ------ | --- | --- |
| 3409 | la Repubblica | 2023-01-17 00:00:00 | ... | Così il digiuno modifica il cervello | 31 | ... | 0.6437915 | ['così', 'il', 'digiuno', 'modifica', 'il', 'cervello'] | ... | ['O', 'O', 'O', 'O', 'O', 'O'] |
| 15526 | ByoBlu | 2022-09-21 00:00:00 | ... | “BILL GATES HA GESTITO IL COVID PER ARRICCHIRSI”: ORA SE NE ACCORGE ANCHE IL MAINSTREAM | 73 | ... | 0.0032087807 | ['BILL', 'GATES', 'HA', 'GESTITO', 'IL', 'COVID', 'PER', 'ARRICCHIRSI', 'oRA', 'sE', 'NE', 'ACCORGE', 'ANCHE', 'IL', 'MAINSTREAM'] | ['O', 'MISC', 'MISC', 'O', 'MISC', 'O', 'ORG', 'O', 'ORG', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'MISC'] |

<p align="center">
Two examples from the dataset
</p>  

In the TSV file for the dataset (TRADISAN_dataset.tsv), each row corresponds to a news article. Each sample has, in this order, a unique id number, source, date of publication, headline, body of text, image links and url. The table has 7 columns in total.

In the TSV file for headline features, each row corresponds to a news headline (found in the 'headline' column). Each sample has, in this order, a unique id number, source, date of publication, url, headline, the 31 feature annotations and the additional annotations at the end, after the 31 features. The table has 40 columns in total.

The dataset is released under Creative Commons license CC BY-NC-SA.

To cite this work:

**Giordano, L. & di Buono, M.P. (2023). Assessing Italian News Reliability in the Health Domain through Text Analysis of Headlines. In Carvalho, S. et al. (eds.) (2023). Language, Data and Knowledge 2023 (LDK 2023): Proceedings of the 4th Conference on Language, Data and Knowledge. NOVA FCSH - CLUNL. https://doi.org/10.34619/srmk-injj**
