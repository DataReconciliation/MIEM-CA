# Dataset for MIEM-CA

## Overview

This dataset is the enhanced version of the standard ER_Magellan benchmarks ([original datasets](https://github.com/anhaidgroup/deepmatcher/blob/master/Datasets.md)) used in the DeepMatcher paper. The enhanced version is performed using our multi-agent information enhancement module with three different large language models: [DeepSeek-V2](https://github.com/deepseek-ai/DeepSeek-V2), [Llama3](https://github.com/meta-llama/llama3), and [Mistral](https://github.com/mistralai/mistral-inference).

## Dataset Structure
```bash
Dataset/
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
```

### Data Organization
Original_Data/:
- `train.txt`
- `valid.txt` 
- `test.txt`

Enhanced_Data/:
- `train_with_features_deepseek.txt`
- `train_with_features_llama3.txt`
- `train_with_features_mistral.txt`
- `valid_with_features_deepseek.txt`
- `valid_with_features_llama3.txt`
- `valid_with_features_mistral.txt`
- `test_with_features_deepseek.txt`
- `test_with_features_llama3.txt`
- `test_with_features_mistral.txt`

### Dataset Categories

- Dirty Contains dirty datasets (4 datasets)
- Structured Contains structured datasets (5 datasets)  
- Textual Contains textual datasets (1 dataset)

### Example: Structured/Amazon-Google

```
Structured/Amazon-Google/
├── Enhanced_Data/
│   ├── train_with_features_deepseek.txt
│   ├── train_with_features_llama3.txt
│   ├── train_with_features_mistral.txt
│   ├── valid_with_features_deepseek.txt
│   ├── valid_with_features_llama3.txt
│   ├── valid_with_features_mistral.txt
│   ├── test_with_features_deepseek.txt
│   ├── test_with_features_llama3.txt
│   └── test_with_features_mistral.txt
└── Original_Data/
    ├── train.txt
    ├── valid.txt
    └── test.txt
```

---
*This enhanced dataset is built upon the ER_Magellan benchmarks from [the DeepMatcher paper](https://pages.cs.wisc.edu/~anhai/papers1/deepmatcher-sigmod18.pdf).*
