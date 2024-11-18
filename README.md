# COVID-19 Research Articles Analysis

### Overrview

This project uses NLP (Natural Language Processing) techniques to analyze a dataset of research articles related to COVID-19. The dataset includes metadata and abstracts from 29,500 articles, facilitating insights into publication trends, topic modeling, and sentiment analysis. The goal is to identify key research topics, trends, and sentiment from the abstracts to assist researchers in navigating the extensive literature on COVID-19.

### Dataset 

- Source: A collection of COVID-19 research articles.
- Total Entries: 29,500
- Columns: 14, including metadata such as title, abstract, authors, and publish_time.

#### Key Columns

- title: The title of the research paper.
- abstract: Abstract of the research paper (textual data used for NLP tasks).
- publish_time: Date of publication.
- journal: Journal in which the article was published.
- authors: Authors of the paper.

#### Missing Values

Significant missing values exist in columns like publish_time, journal, and has_full_text. These were handled through imputation or exclusion, depending on the analysis.

### Project Workflow

1. Data Preprocessing
- Removed duplicates and handled missing values.
- Converted publish_time to datetime format.
- Preprocessed abstracts by: Tokenizing, Removing stopwords, Lowercasing and removing non-alphanumeric characters.

2. Exploratory Data Analysis (EDA)
- Abstract Length Distribution: Visualized the variability in abstract lengths.
- Source and Journal Analysis: Identified top sources and journals publishing COVID-19 research.

3. Topic Modeling

Using Latent Dirichlet Allocation (LDA), the following topics were identified:
- Topic 1: Public health and epidemic data.
- Topic 2: Clinical and respiratory infections.
- Topic 3: RNA synthesis and viral genome studies.
- Topic 4: Immune response and protein expression.
- Topic 5: Influenza strains and vaccine research.

4. Sentiment Analysis
- Performed sentiment analysis on abstracts using TextBlob.
- Visualized sentiment distribution to identify overall polarity trends in the research articles.

### Key Results

Most abstracts had neutral or positive sentiment, reflecting the research community's emphasis on constructive insights and findings.
- Topic 1: Focused on public health and epidemic data.
- Topic 2: Centered on clinical studies and respiratory infections.
- Topic 3: Explored RNA synthesis and genome research.
- Topic 4: Investigated immune responses and protein-level interactions.
- Topic 5: Discussed influenza strains, vaccine development, and species transmission.

### Visualizations

- Abstract Length Distribution: Histogram of word counts in abstracts.
- Top Sources and Journals: Bar plots of the most prolific contributors.
- Sentiment Analysis: Distribution of sentiment polarity across abstracts.
- Topic Visualization: Word clouds for each topic identified through LDA.

### Future Work

- Named Entity Recognition (NER): Extract key entities such as drug names, authors, or affiliations.
- Temporal Analysis: Analyze trends over time based on publish_time.
- Cluster Analysis: Group similar abstracts based on semantic similarity.

### Source

https://www.kaggle.com/datasets/anthonytherrien/covid-19-research-articles
