# Overview

- We have prepared scripts for pre-training BERT on ABCI
  - The performance of BERT on the end tasks depends on the text collection for the pre-training. 
  - This script allows the training of BERT on ABCI on your large-scale domain text collection, which can be used to evaluate your domain-specific models. 
- In our evaluation, it took 15 hours to train a BERT base model (about 1/3 of the computational cost in the BERT large model) on 83.5 GB texts in an epoch using 16 GPUs.
  - With the whole 4,356 GPUs in ABCI, the training time can be reduced to about 3.3 mins (~10 mins for a BERT large model). 
- The performance is 83.50% in the nested named entity recognition on the BioNLP 2013 CG corpus.
  - The performance is comparable to or slightly better than the scores by the BioBERT model (83.19%), which is fine-tuned from the original BERT, and the SciBERT model (82.60%), which is pre-trained on a smaller corpus.


# Scripts

- [training BERT from scratch](https://github.com/aistairc/kirt_bert_on_abci)
- fine-tuning BERT / evaluating BERT-based models (TBA)

# Models

- [Biomedical BERT base model (alpha)](https://data.airc.aist.go.jp/abci_bert/abci_bio_bert_base_alpha.zip)
- [Biomedical BERT base model (alpha, with sentence-based separator [SEP] token)](https://data.airc.aist.go.jp/abci_bert/abci_bio_bert_base_sep_alpha.zip)

# Acknowledgement

The results are obtained from projects commissioned by NEDO (New Energy and Industrial Technology Development Organization) and PRISM (Public/Private R&D Investment Strategic Expansion PrograM).
