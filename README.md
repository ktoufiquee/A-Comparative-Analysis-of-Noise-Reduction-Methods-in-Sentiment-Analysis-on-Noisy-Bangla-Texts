# A Comparative Analysis of Noise Reduction Methods in Sentiment Analysis on Noisy Bengali Texts

This repository contains the code and datasets used in the paper titled **"A Comparative Analysis of Noise Reduction Methods in Sentiment Analysis on Noisy Bengali Texts
"** accepted in *2024 The 9th Workshop on Noisy and User-generated Text (W-NUT) collocated with EACL 2024*.

## Table of Contents

  - [Models](#models)
  - [Datasets](#datasets)
  - [Training & Evaluation](#training--evaluation)
  - [Benchmarks](#benchmarks)
  - [License](#license)
  - [Citation](#citation)

## Models

The code used to train and test the models are available in this repository on the folder *NC-SentNoB Codes*.


## Datasets

The NC-SentNoB dataset is available at this repository on the folder *NC-SentNoB Dataset*.
SentNoB dataset with Back translation applied is also available on the folder *Back-Translated Data*.
The 1000 ground truths used to evaluate denoising methods are available on the file *1000 Ground Truth.xlsx*

The SentNoB dataset is available at this [link](https://github.com/KhondokerIslam/SentNoB).


## Training & Evaluation

We used pretrained transformer based models for Sentiment Classification and SVM, BiLSTM, BanglaBERT for Noise Identification.

## Results
 
* Noise Identification

| Model           |  Precision | Recall  | F1-Score  |
|-----------------|------------|---------|-----------|
|SVM (C)          |  0.76      | 0.45    | 0.57      |
|SVM (W)          |  0.64      | 0.38    | 0.48      |
|SVM (C+W)        |  0.75      | 0.45    | 0.56      |
|Bi-LSTM          |  0.36      | 0.18    | 0.24      |
|Bangla-BERT-base |  0.73      | 0.54    | 0.62      |

* Sentiment Analysis on Noisy Text

| Model | Precision | Recall  | F1-Score  |
|-------|-----------|---------|-----------|
|Bangla-BERT-Base     | 0.72  | 0.72  | 0.72  |
|BanglaBERT           | 0.75  | 0.75  | 0.75  |
|BanglaBERT Large     | 0.74  | 0.74  | 0.74  |
|BanglaBERT Generator | 0.72  | 0.72  | 0.72  |
|sahajBERT            | 0.72  | 0.72  | 0.72  |
|Bangla-Electra       | 0.68  | 0.68  | 0.68  |
|MuRIL                | 0.73  | 0.73  | 0.73  |

* Sentiment Analysis on Denoised Text (Using Google Translate)

| Model | Precision | Recall  | F1-Score  |
|-------|-----------|---------|-----------|
|Bangla-BERT-Base     | 0.69  | 0.69  | 0.69  |
|BanglaBERT           | 0.72  | 0.72  | 0.72  |
|BanglaBERT Large     | 0.73  | 0.73  | 0.73  |
|BanglaBERT Generator | 0.70  | 0.70  | 0.70  |
|sahajBERT            | 0.70  | 0.70  | 0.70  |
|Bangla-Electra       | 0.66  | 0.66  | 0.66  |
|MuRIL                | 0.71  | 0.71  | 0.71  |

## License
Contents of this repository are restricted to non-commercial research purposes only under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/). 

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>

## Citation
If you use any of the datasets, models or code modules, please cite the following paper:
```
Coming soon.
```
