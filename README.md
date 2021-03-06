# Updates

- We have prepared scripts for pre-training BERT on ABCI (12/10/2019).

# Scripts

## [Training BERT from scratch](https://github.com/aistairc/kirt_bert_on_abci)

We have prepared scripts for pre-training BERT on ABCI. The performance at the end tasks depends on the text collection for the pre-training. The scripts allow the training of BERT on ABCI on your large-scale domain text collection, which can be used to evaluate your domain-specific models. 

In our evaluation, it took 15 hours to train a BERT base model (about 1/3 of the computational cost in the BERT large model) on 83.5 GB texts ([2019 MEDLINE/PubMed baseline](https://www.nlm.nih.gov/databases/download/pubmed_medline.html)+[PMC Open Access Subset](https://www.ncbi.nlm.nih.gov/pmc/tools/openftlist/)) in an epoch using 16 GPUs. With the whole 4,356 GPUs in ABCI, the training time is estimated to be reduced to about 3.3 mins/epoch (~10 mins/epoch for a BERT large model). 

The performance is 83.50% in the nested named entity recognition on the BioNLP 2013 CG corpus. This performance is better than the original BERT (79.33%). This performance is also comparable to or slightly better than the scores by the BioBERT model (83.19%), which is fine-tuned from the original BERT, and the SciBERT model (82.60%), which is pre-trained on a smaller corpus.

## Fine-tuning BERT / evaluating BERT-based models (TBA)

# Models

## Biomedical BERT
- [base model (alpha)](https://data.airc.aist.go.jp/abci_bert/abci_bio_bert_base_alpha.zip)
- [base model (alpha, with sentence-based separator [SEP] token)](https://data.airc.aist.go.jp/abci_bert/abci_bio_bert_base_sep_alpha.zip)

# References

- Jacob Devlin, Ming-Wei Chang, Kenton Lee and Kristina Toutanova, "BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding." In Proceedings of the 2019 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long and Short Papers), pp. 4171-4186. 2019.

# Acknowledgement

The results are obtained from "Strategic Advancement of Multi-Purpose Ultra-Human Robot and Artificial Intelligence Technologies（SamuRAI） Project" and "Ultra High-Throughput Design and Prototyping Technology for Ultra Advanced Materials Development Project" commissioned by the New Energy and Industrial Technology Development Organization (NEDO) and a project commissioned by Public/Private R&D Investment Strategic Expansion PrograM (PRISM).
