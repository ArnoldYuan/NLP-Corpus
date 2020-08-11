# Popular Datasets for BioNER

## 1. GENIA
### Introduction
GENIA involves 36 fine-grained entity categories among 2,000 PubMed headings and abstracts.
### Relating paper
Jin-Dong Kim, Tomoko Ohta, Yuka Tateisi, and Ju- nichi Tsujii. 2003. GENIA corpus—a semantically annotated corpus for bio-textmining. *Bioinformat- ics 19(suppl. 1):i180–i182.*
### Statistics
+ 36 fine-grained entity categories
+ 2,000 MEDLINE abstracts
+ 17% nested mentions

| Item | Train | Dev | Test |
| - | - | - | - |
| Documents | 1,599 | 189 | 212 |
| Sentences | 15,022 | 1,669 | 1,855 |
| Split percentage | 81% | 9% | 10% |
| Nested level | 4 | 3 | 3 |
| Entity avg. length | 2.87 | 3.13 | 2.93 |
| Overall entities | 46,853 | 4,442 | 5,575 |
(A Neural Layered Model for Nested Named Entity Recognition)
### Download link
http://www.geniaproject.org/genia-corpus/term-corpus
### Variations
+ Sentence segmentation  
+ Tokenization  
+ POS Tagging
+ Syntactic Tree annotation
+ Function Tags
+ Term annotation
+ Event annotation




## 2. ACE 2004/2005
### Introduction
ACE Multilingual Training Corpus contains the complete set of English, Arabic and Chinese training data for the Automatic Content Extraction (ACE) technology evaluation.
### Relating paper
Christopher Walker, Stephanie Strassel, Julie Medero, and Kazuaki Maeda. 2006. ACE 2005 multilingual training corpus. *Linguistic Data Consortium, Philadelphia 57.*
### Statistics
+ 3 languages (English, Arabic and Chinese)
+ 7 main entity types  
Person (PER), Organization (ORG), Geographical Entities (GPE), Location (LOC), Facility (FAC), Weapon (WEA) and Vehicle (VEH)
+ 24% (ACE 2004) and 22% (ACE 2005) nested mentions respectively

| Item | Train | Dev | Test |
| - | - | - | - |
| Documents | 370 | 43 | 51 |
| Sentences | 9849 | 1,221 | 1478 |
| Split percentage | 80% | 10% | 10% |
| Nested level | 6 | 4 | 5 |
| Entity avg. length | 2.28 | 2.33 | 2.28 |
| Overall entities | 24,440 | 2,972 | 3,554 |
(A Unified MRC Framework for Named Entity Recognition)
### Download link
https://www.ldc.upenn.edu/collaborations/past-projects/ace/annotation-tasks-and-specifications


## 3. KBP2017
### Introduction
The goal of TAC Knowledge Base Population (KBP) is to develop and evaluate technologies for populating knowledge bases (KBs) from unstructured text. KBP includes component tracks that develop specific components and capabilities for KBP, as well as an end-to-end KB construction task called "Cold Start", which builds a KB from scratch by integrating selected components as their technology matures.

### Statistics
+ 3 languages (English, Chinese and Spanish)
+ 19% nested mentions
+ 90,000 "common" documents
+ 500 "core" documents annotated with entities, relations, and events (ERE)
+ Split strategy: Hongyu Lin, Yaojie Lu, Xianpei Han, and Le Sun. 2019b. Sequence-to-nuggets: Nested entity men- tion detection via anchor-region networks. In *Proceedings of the 57th Conference of the Association for Computational Linguistics, ACL 2019, Florence, Italy, July 28- August 2, 2019, Volume 1: Long Papers*, pages 5182–5192.
### Download link
https://tac.nist.gov/2017/KBP/data.html

## 4. JNLPBA
### Introduction
JNLPBA defines both training and testing datasets. These two datasets are composed of 2,000 and 404 PubMed abstracts, respectively. JNLPBA is originally from the GENIA corpus. However, only flat and topmost entities in JNLPBA are kept while nested and discontinuous entities are removed.
### Relating paper
Jin-Dong Kim, Tomoko Ohta, Yoshimasa Tsuruoka, Yuka Tateisi, and Nigel Collier. (2004). Introduction to the Bio-Entity Recognition Task at JNLPBA. in the *Proceedings of the International Workshop on Natural Language Processing in Biomedicine and its Applications (JNLPBA-04). pp. 70--75.*
### Statistics
+ Training set: 2,000 PubMed abstracts
+ Testing set: 404 PubMed abstracts
+ no nested mentions
+ IOB2 format

| Item | Train | Dev | Test |
| - | - | - | - |
| Sentences | 16,691 | 1,855 | 3,856 |
| Split percentage | 90% | 10 % | - |
| Entity avg. length | 2.28 | 2.33 | 2.28 |
| Overall entities | 24,440 | 2,972 | 3,554 |
(already splitted)
### Download link
http://www.geniaproject.org/shared-tasks/bionlp-jnlpba-shared-task-2004

## 5. CoNLL-2003
### Introduction
The CoNLL 2003 NER task consists of newswire text from the Reuters RCV1 corpus tagged with four different entity types (PER, LOC, ORG, MISC).
### Relating paper
Erik F. Tjong Kim Sang and Fien De Meulder. 2003. Introduction to the CoNLL-2003 shared task: Language-independent named entity recognition. In *Proceedings of CoNLL*, pages 142–147.
### Statistics
+ 2 languages (English and German)
+ no nested mentions
+ IOB format
+ Requires access to **Reuters Corpus** and **ECI Multilingual Text Corpus**
+ Already splitted into train/dev/test sets
### Download link
https://www.clips.uantwerpen.be/conll2003/ner/

## 6. OntoNotes 5.0
### Introduction
OntoNotes 5.0 is an English dataset and consists of text from a wide variety of sources. The dataset includes 18 types of named entity, consisting of 11 types (Person, Organization, etc) and 7 values (Date, Percent, etc).
### Relating paper
Sameer Pradhan, Alessandro Moschitti, Nianwen Xue, Hwee Tou Ng, Anders Bjo ̈rkelund, Olga Uryupina, Yuchen Zhang, and Zhi Zhong. 2013. Towards robust linguistic analysis using OntoNotes. In *Proceedings of the Seventeenth Conference on Computational Natural Language Learning*, pages 143–152, Sofia, Bulgaria. Association for Computational Linguistics.
### Statistics
+ 3 languages (English, Chinese, and Arabic) 
+ 18 types of named entity
+ 11 types (Person, Organization, etc) and 7 values (Date, Percent, etc)
+ Split strategy: In the referred relating paper

### Download link
https://catalog.ldc.upenn.edu/LDC2013T19

## Preprocessing
### GENIA Tagger
Download: http://www.geniaproject.org/genia-corpus/term-corpus
### NERsuite  
A Named Entity Recognition toolkit which includes tokenizer, POS-tagger, lemmatizer and chunker.  
Download: http://nersuite.nlplab.org/index.html
### CoreNLP  
The stanford corenlp natural lan- guage processing toolkit.  
Download: https://github.com/stanfordnlp/CoreNLP

## Preprocessed corpora in Biology
### Download link
https://github.com/cambridgeltl/MTL-Bioinformatics-2016
### Paper
A Neural Network Multi-Task Learning Approach to Biomedical Named Entity Recognition.
### Statistics
+ format: IOB and IOBES
+ 15 NER corpora
+ 1 POS corpus
+ The download link also includes instructions for splitting train/dev/test datasets and detailed information about each dataset
>number of entities in these datasets

|               | train | dev   | test  | total |
|---------------|-------|-------|-------|-------|
| BC4CHEMD      | 29478 | 29486 | 25346 | 84310 |
| JNLPBA        | 46750 | 4551  | 8662  | 59963 |
| CRAFT         | 29026 | 9727  | 18881 | 57634 |
| BC5CDR        | 9385  | 9593  | 9806  | 28784 |
| BC2GM         | 15191 | 3061  | 6325  | 24577 |
| BioNLP13CG    | 10826 | 3616  | 6881  | 21323 |
| BioNLP13PC    | 7853  | 2734  | 5306  | 15893 |
| BioNLP11EPI   | 7586  | 2495  | 5730  | 15811 |
| BioNLP09      | 9296  | 2078  | 3589  | 14963 |
| AnatEM        | 6946  | 2139  | 4616  | 13701 |
| BioNLP13GE    | 3566  | 4132  | 4359  | 12057 |
| BioNLP11ID    | 5674  | 1598  | 3810  | 11082 |
| NCBI\-disease | 5134  | 787   | 960   | 6881  |
| Ex\-PTM       | 1787  | 603   | 2308  | 4698  |
| LINNAEUS      | 2119  | 711   | 1433  | 4263  |
