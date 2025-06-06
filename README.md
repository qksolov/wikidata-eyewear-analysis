# Wikidata Eyewear Analysis

This repository contains an exploratory analysis of notable individuals from Wikidata, supplemented with an eyewear detection analysis using the [EyewearCounter](https://github.com/qksolov/eyewear-counter) model to study glasses-wearing patterns across various occupations.

## Dataset

The analysis is based on the **Notable People Dataset**, specifically compiled for this project.  
It contains 417K+ biographical records of people born in the 20th and 21st centuries, extracted from Wikidata via SPARQL queries.

The dataset and detailed description are available in:
- the `/data` directory
- [Kaggle Dataset](https://www.kaggle.com/datasets/qqsolov/notable-people-dataset-wikidata-based)

## Notebooks

- `notebooks/notable-people-wikidata-eda.ipynb`  
  General analysis of the dataset: gender distribution, birth/death years, geography, and occupation groups.

- `notebooks/eyewear-notable-people-wikidata-eda.ipynb`  
  Analysis of model predictions: eyewear types (glasses, sunglasses, none) in relation to gender, age, occupations, and countries.
