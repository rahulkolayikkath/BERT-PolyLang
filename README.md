# BERT-PolyLang
A BERT based chemical language model to learn polymer representations.
This repo serves as a code release to my master's project advised by Dr Tarak kumar Patra.
Affliations: Patra Research Group, IIT Madras

## Overview 
The workflow consist of training a tokenizer first and using the tokenizer for training the language model.

### Training of the tokenizer 
We explored two paths to train the tokeniser 
1) Implement BPE from Scratch adapting to Psmile strings
Tokeniser is trained using Byte Pair Encoding inspired from Andrej Karpathy's [minbpe](https://github.com/karpathy/minbpe)
2) Train tokeniser using Hugging Face [Tokenizer](https://pypi.org/project/tokenizers/)
We trained the HF Tokenizer model BPE with custom special tokens which include fucntional groups, elements and ions present in psmiles

### Testing the tokenizer
Use test_tokenizer.py script to test the tokeniser model



## Read More
1) [Language Moodelling for learning robust polymer representations](https://rahulkolayikkath.github.io/personal-website/CH19B022_Mtech_Thesis.pdf), Masters Thesis:Rahul Krishna K, IITM(2024)
2) [polyBERT: a chemical language model to enable fully machine-driven ultrafast polymer informatics](https://www.nature.com/articles/s41467-023-39868-6), Christopher Kuenneth and Rampi Ramprasad, Nature Communications, 14(1), July 2023