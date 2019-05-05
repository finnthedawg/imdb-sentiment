😂😁😐 Sentiment analysis of IMDB movie reviews 😞😠😤
---

This project conducts sentiment analysis on the `Large Movie Review Dataset v1.0` (Mass et al., 2011) which contains 100,000 reviews extracted from the IMDB movie review website. The dataset can be downloaded from the Stanford website. http://ai.stanford.edu/~amaas/data/sentiment/

### The dataset:

The core dataset contains 50,000 reviews split evenly into 25k train
and 25k test sets. The overall distribution of labels is balanced (25k
pos and 25k neg). There is an additional 50,000 unlabeled
documents for unsupervised learning.

In the entire collection, no more than 30 reviews are allowed for any
given movie because reviews for the same movie tend to have correlated
ratings. Further, the train and test sets contain a disjoint set of
movies, so no significant performance is obtained by memorizing
movie-unique terms and their associated with observed labels.  In the
labeled train/test sets, a negative review has a score <= 4 out of 10,
and a positive review has a score >= 7 out of 10. Thus reviews with
more neutral ratings are not included in the train/test sets. In the
unsupervised set, reviews of any rating are included and there are an
even number of reviews > 5 and <= 5.

## Run instructions
Install the required packages
```
pip install -U scikit-learn
```
Run the notebook and execute the cells in question
```
jupyter notebook analysis.ipynb
```

## Analysis performed:

#### Vectorization of words and learning classification using regression models

#### Building a Word2Vec model for sentiment analysis

#### Building a Doc2Vec model

## References

---
1. [IMDB] A.L.Maas,  R.E.Daly,  P.T.Pham,  D.Huang, A.Y.Ng,  and C.Potts,  “Learning word  vectors  for  sentiment  analysis,”  in Proceedings of the 49th Annual Meeting of the Association for Computational Linguistics: Human Language Technologies. Portland, Oregon,
2. [Word2Vec] Mikolov, T., Chen, K., Corrado, G.S., & Dean, J. (2013). Efficient Estimation of Word Representations in Vector Space. CoRR, abs/1301.3781.
