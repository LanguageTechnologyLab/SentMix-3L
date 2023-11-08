# SentMix-3L: A Bangla-English-Hindi Code-Mixed Dataset for Sentiment Analysis

**Publication**: *The First Workshop in South East Asian Language Processing Workshop under AACL-2023.*

**Read in [arXiv](https://arxiv.org/pdf/2310.18023.pdf)** 

---

## 📖 Introduction

Code-mixing is a well-studied linguistic phenomenon when two or more languages are mixed in text or speech. Several datasets have been built with the goal of training computational models for code-mixing. Although it is very common to observe code-mixing with multiple languages, most datasets available contain code-mixed between only two languages. In this paper, we introduce **SentMix-3L**, a novel dataset for sentiment analysis containing code-mixed data between three languages: Bangla, English, and Hindi. We show that zero-shot prompting with GPT-3.5 outperforms all transformer-based models on SentMix-3L.

---

## 📊 Dataset Details

We introduce **SentMix-3L**, a novel three-language code-mixed test dataset with gold standard labels in Bangla-Hindi-English for the task of Sentiment Analysis, containing 1,007 instances.

> We are presenting this dataset exclusively as a test set due to the unique and specialized nature of the task. Such data is very difficult to gather and requires significant expertise to access. The size of the dataset, while limiting for training purposes, offers a high-quality testing environment with gold-standard labels that can serve as a benchmark in this domain.

---

## 📈 Dataset Statistics

|                   | **All** | **Bangla** | **English** | **Hindi** | **Other** |
|-------------------|---------|------------|-------------|-----------|-----------|
| Tokens            | 89494   | 32133      | 5998        | 15131     | 36232     |
| Types             | 19686   | 8167       | 1073        | 1474      | 9092      |
| Max. in instance  | 173     | 62         | 20          | 47        | 93        |
| Min. in instance  | 41      | 4          | 3           | 2         | 8         |
| Avg               | 88.87   | 31.91      | 5.96        | 15.03     | 35.98     |
| Std Dev           | 19.19   | 8.39       | 2.94        | 5.81      | 9.70      |

*The row 'Avg' represents the average number of tokens with its standard deviation in row 'Std Dev'.*

---

## 📉 Results

| **Models**    | **Weighted F1 Score** |
|---------------|-----------------------|
| GPT 3.5 Turbo | **0.62**              |
| XLM-R         | 0.59                  |
| BanglishBERT  | 0.56                  |
| mBERT         | 0.56                  |
| BERT          | 0.55                  |
| roBERTa       | 0.54                  |
| MuRIL         | 0.54                  |
| IndicBERT     | 0.53                  |
| DistilBERT    | 0.53                  |
| HindiBERT     | 0.48                  |
| HingBERT      | 0.47                  |
| BanglaBERT    | 0.47                  |

*Weighted F-1 score for different models: training on synthetic, testing on natural data.*

---

## 📝 Citation

If you utilize this dataset, kindly cite our paper.

```bibtex
@article{raihan2023sentmix,
  title={SentMix-3L: A Bangla-English-Hindi Code-Mixed Dataset for Sentiment Analysis},
  author={Raihan, Md Nishat and Goswami, Dhiman and Mahmud, Antara and Anstasopoulos, Antonios and Zampieri, Marcos},
  journal={arXiv preprint arXiv:2310.18023},
  year={2023}
}

