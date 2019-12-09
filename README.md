# Overview

- We have prepared scripts of training/fine-tuning BERT on ABCI
- It took 3 days to train a BERT base model on 83.5 GB texts in an epoch using 16 GPUs. 
- The performance is 83.50% (compared to 82.60% with SciBERT) in the nested named entity recognition on the BioNLP 2013 CG corpus.

# Scripts

- [training BERT from scratch](https://github.com/aistairc/kirt_bert_on_abci)
- fine-tuning BERT / evaluating BERT-based models (TBA)

# Models

- [Biomedical BERT base model (alpha)](https://data.airc.aist.go.jp/abci_bert/abci_bio_bert_base_alpha.zip)
- [Biomedical BERT base model (alpha, with sentence-based separator [SEP] token)](https://data.airc.aist.go.jp/abci_bert/abci_bio_bert_base_sep_alpha.zip)

# Acknowledgement

The results are obtained from projects commissioned by NEDO (New Energy and Industrial Technology Development Organization) and PRISM (Public/Private R&D Investment Strategic Expansion PrograM).
