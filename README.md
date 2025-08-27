# Dataset for MIEM-CA

## Overview

This dataset is the enhanced version of the standard ER_Magellan benchmarks used in the DeepMatcher paper ([original datasets](https://github.com/anhaidgroup/deepmatcher/blob/master/Datasets.md)). The enhanced version is performed using our multi-agent information enhancement module with three different large language models: [DeepSeek](https://github.com/deepseek-ai/DeepSeek-V2), [Llama3](https://github.com/meta-llama/llama3), and [Mistral](https://github.com/mistralai/mistral-inference).

## Dataset Structure
```bash
Data/
├── Dirty/                          
│   ├── DBLP-ACM/                   
│   ├── DBLP-GoogleScholar/         
│   ├── iTunes-Amazon/              
│   └── Walmart-Amazon/             
├── Structured/                     
│   ├── Amazon-Google/              
│   ├── DBLP-ACM/                   
│   ├── DBLP-GoogleScholar/        
│   ├── iTunes-Amazon/              
│   └── Walmart-Amazon/             
└── Textual/                      
    └── Abt-Buy/                    

Each dataset directory contains the following files:

Original Data:
- train.txt, valid.txt, test.txt

Enhanced Data:
- train_with_features_deepseek.txt
- train_with_features_llama3.txt  
- train_with_features_mistral.txt
- valid_with_features_deepseek.txt
- valid_with_features_llama3.txt
- valid_with_features_mistral.txt
- test_with_features_deepseek.txt
- test_with_features_llama3.txt
- test_with_features_mistral.txt
```

---
*This enhanced dataset is built upon the ER_Magellan benchmarks from [the DeepMatcher paper](https://pages.cs.wisc.edu/~anhai/papers1/deepmatcher-sigmod18.pdf).*
