# COVID-19 Research Articles Analysis

## Overview

The rapid growth of COVID-19 research has resulted in a vast collection of literature, making it challenging for researchers to keep up. This project applies Natural Language Processing (NLP) techniques to analyze over 29,500 research articles, extracting actionable insights on key research topics, trends, and sentiment. The analysis provides a comprehensive overview of the state of COVID-19 research, aiding researchers in navigating this extensive literature more effectively.

### Problem Statement

The overwhelming volume of COVID-19-related publications makes it difficult to identify key areas of focus, trends, and actionable insights. This project addresses this issue by using NLP techniques to analyze research articles, uncover prominent topics, and assess overall sentiment in the literature.

### Dataset

- Source: COVID-19 Research Articles Dataset.
- Size: 29,500 articles.
- Key Features:
    - Title: Research paper title.
    - Abstract: Summary of the research (used for NLP tasks).
    - Publish Time: Date of publication.
    - Journal: Journal where the article was published.
    - Authors: List of authors.

### Solution Approach:

1. Data Preprocessing
- Removed duplicates and handled missing values (e.g., imputed or excluded incomplete records).
- Converted publication dates into a datetime format for temporal analysis.
- Preprocessed abstracts through:
    - Tokenization.
    - Removal of stopwords.
    - Lowercasing and removal of non-alphanumeric characters.

2. Exploratory Data Analysis (EDA)
- Abstract Length Distribution: Analyzed and visualized variability in abstract lengths.
- Source and Journal Analysis: Identified the most prolific journals and sources contributing to COVID-19 research.

3. Topic Modeling
- Applied Latent Dirichlet Allocation (LDA) to identify five key topics:
    - Topic 1: Public health and epidemic data.
    - Topic 2: Clinical and respiratory infections.
    - Topic 3: RNA synthesis and viral genome studies.
    - Topic 4: Immune response and protein expression.
    - Topic 5: Influenza strains and vaccine research.

4. Sentiment Analysis
- Conducted sentiment analysis on abstracts using TextBlob.
- Visualized sentiment polarity (positive, neutral, negative) to assess trends in research focus and tone.

### Key Results

Topics Identified:
- Public Health: Studies on epidemic modeling and population-level health impacts.
- Clinical Focus: Research on respiratory infections and clinical management.
- Genomic Studies: Insights into RNA synthesis and viral genomes.
- Immunology: Investigations into immune responses and protein-level interactions.
- Vaccines: Studies on influenza strains, vaccine development, and species transmission.

Sentiment Analysis:
- Most abstracts exhibited neutral or positive sentiment, reflecting the research community's constructive focus on solutions and findings.

Visual Insights:
- Abstract Length Distribution: Highlighted variability, with most abstracts being concise but informative.
- Top Journals: Identified leading publishers contributing to COVID-19 research.
- Word Clouds: Created for each topic to emphasize key terms and themes.

### Challenges: 

- Unstructured Text: Required extensive preprocessing to handle variability in abstract quality and content.
- Class Imbalance in Sentiment: Addressed through normalization techniques to ensure robust analysis.

### Future Directions

1. Named Entity Recognition (NER): Extract specific entities like drug names, affiliations, or geographic regions.

2. Temporal Analysis: Study trends over time to track research focus shifts or emerging areas of interest.

3. Advanced Models: Leverage transformer-based models (e.g., BERT) for deeper insights and improved text understanding.

4. Semantic Clustering: Group abstracts by similarity to identify subfields within broader topics.

### Source

https://www.kaggle.com/datasets/anthonytherrien/covid-19-research-articles
