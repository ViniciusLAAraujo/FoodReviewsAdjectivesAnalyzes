# Analysis on Adjective Frequency in Fine Food Reviews


<p align="center">
  <img src="https://github.com/ViniciusLAAraujo/GrafosTP01/blob/main/AllReviews.png" alt="FineFoodsFull" width="450" height="450">
</p>



## Table of Contents

- [About](#about)
  - [Problem Statement](#problem-statement)
  - [Complex Networks](#complex-networks)
  - [Abstract](#abstract)
- [How to Run](#how-to-run)
  - [Quick Tutorial](#quick-tutorial)
  - [Libraries](#libraries)
- [Conclusions](#conclusions)

## About

### Problem Statement

The purpose of this project is to conduct an analysis of adjective frequency in fine food reviews. By analyzing a sample of food reviews, we aim to gain insights into the sentiments expressed by customers towards various food items. Specifically, we will focus on identifying the most commonly used adjectives and their associations with different food products. This analysis will help us understand how customers perceive the quality and taste of fine foods based on the words they use in their reviews.

### Complex Networks

Complex networks are abstract representations of components and their relationships, enabling the modeling of real-world situations. They comprise various nodes connected by edges, and analyzing these networks aids in predicting behavior and identifying patterns. However, not every graph is a complex network. To be considered a complex network, graphs must meet specific characteristics, including clustering coefficient, degree distribution, resilience, pattern mixing, and degree correlation.

The chosen dataset fulfills the criteria to be considered a complex network. Within this network, notable features include triangle relationships connecting adjectives to multiple review scores and pattern mixing, where edges can have positive or negative connotations based on the weights associated with low or high-score reviews, respectively. Moreover, the graph can be categorized as a scale-free network, indicating a heterogeneous distribution of degrees among nodes (ratings and adjectives).

### Abstract

This project contributed to the construction of an article aimed at analyzing the relationship between ratings and adjectives in Amazon fine food reviews using the concepts of graphs and complex networks. The majority of reviews received ratings of 1, 4, or 5 stars. A random sample from the database revealed a higher volume of reviews with a score of 5, which can be attributed to the nature of Fine foods, suggesting higher quality. Interestingly, the analysis of adjectives like "hot," "little," and "small" yielded unexpected results, as these words may not initially seem closely related to positive qualities.


The original database can be found at [this link](https://snap.stanford.edu/data/web-FineFoods.html) (finefoods.txt.gz), and it contains over 500 thousand reviews. For this analysis, 1,112 reviews were randomly extracted (10 thousand lines from the foods.valeutxt file) and placed into the reviews.txt file.

For the full article (PT-BR), you can [download it here](https://github.com/ViniciusLAAraujo/GrafosTP01/blob/main/Pesquisa_Científica_Grafos.pdf).

## How to Run

### Quick Tutorial

To run this analysis, follow these steps:

1. Install Python and Jupyter Notebook on your machine. If you don't have them installed, you can follow this [Jupyter Notebook installation tutorial](https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook) to set them up.
2. Install the required [libraries](#libraries)
3. Clone this repository to your local machine.
4. Open the Jupyter Notebook file (.ipynb) in Jupyter Notebook.
5. Run each cell in the notebook to execute the analysis.

<p align="center">
  <img src="https://github.com/ViniciusLAAraujo/GrafosTP01/blob/main/Star1.png" alt="Star1" width="200">
  <img src="https://github.com/ViniciusLAAraujo/GrafosTP01/blob/main/Star2.png" alt="Star2" width="200">
  <img src="https://github.com/ViniciusLAAraujo/GrafosTP01/blob/main/Star3.png" alt="Star3" width="200">
</p>
<p align="center">
  <img src="https://github.com/ViniciusLAAraujo/GrafosTP01/blob/main/Star4.png" alt="Star4" width="200">
  <img src="https://github.com/ViniciusLAAraujo/GrafosTP01/blob/main/Star5.png" alt="Star5" width="200">
</p>

### Libraries

The project utilized the following libraries:

- [regex](https://pypi.org/project/regex/): A regular expression library.

```bash
pip install regex
```

- [networkx](https://pypi.org/project/networkx/): A library for creating and analyzing networks.

```bash
pip install networkx
```

- [matplotlib](https://pypi.org/project/matplotlib/): A plotting library for Python.

```bash
pip install matplotlib
```

- [nltk](https://pypi.org/project/nltk/): Natural Language Toolkit for text processing. 

```bash
pip install nltk
```
**In the case of NLTK, it is also necessary to download the English model. For more details, visit [this link](https://www.nltk.org/install.html)**

## Conclusions

Based on the conducted experiment, it was possible to construct a web of relationships between various adjectives used in fine food reviews. The "nltk" and "networkx" libraries played a crucial role in analyzing and organizing the data in an accessible manner. However, the attempt to trace the influence of adjectives on high ratings yielded unexpected results in some cases, indicating a need for linguistic considerations about the process of composing sentences in different idioms.

Upon analyzing the results, a majority of reviews received the highest rating (5 stars), nearly twice as many as all other ratings combined. This observation suggests that the higher number of top-rated reviews can be attributed to the superior quality of the dishes, given their classification as high-class items. Notably, adjectives like "great," "best," "favorite," and "delicious" had significantly high frequencies in these reviews, serving as strong indicators of positive ratings. Nonetheless, certain adjectives, such as 'good,' exhibited high overall frequency but proved to be less reliable indicators, given their use in both positive and negative reviews. This observation can be attributed to the versatility of the English language, where 'good' can be employed to form negative expressions like 'not good' or 'this wasn't good,' and even sarcastically, such as 'good food for a dog.

Ultimately, the analysis generated insightful conclusions and guidelines for different types of reviews. Particularly, the noteworthy presence of "hot," "little," and "small" adjectives in 4 and 5-star reviews stands out. While the frequent use of "hot" may be related to spicy and flavorful dishes, further investigation is required for the other two adjectives. The experiment's analysis provided valuable data that can enhance real-world scenarios, particularly in maximizing positive reviews. With more careful data structuring and elimination of outliers, such as linguistic composition symbols, even more precise and surprising results could be achieved.

<p align="center">
  <img src="https://github.com/ViniciusLAAraujo/GrafosTP01/blob/main/BipartieFull.png" alt="BipartieFull" width="450" height="450">
</p>