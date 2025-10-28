# 🧠 **Social Graphs and Interactions — Royal Family Network Analysis**

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![NetworkX](https://img.shields.io/badge/Library-NetworkX-green.svg)](https://networkx.org/)
[![NLTK](https://img.shields.io/badge/NLP-NLTK-orange.svg)](https://www.nltk.org/)
[![Plotly](https://img.shields.io/badge/Visualization-Plotly-ff69b4.svg)](https://plotly.com/)
[![License](https://img.shields.io/badge/License-MIT-lightgrey.svg)](LICENSE)

---

## **Overview**
This project investigates **European royal family networks** through **graph analytics**, **Wikipedia API data extraction**, and **Natural Language Processing (NLP)**.  
It models monarchic relationships as a **knowledge graph** to study correlations between **inbreeding coefficients**, **social connectivity**, and **biographical sentiment analysis** derived from publicly available historical data.  

The analysis combines **network science**, **computational genealogy**, and **text mining** to uncover patterns in dynastic interrelations and hereditary impact over time.

---

## 🚀 **Key Features & Contributions**

### 🧩 **1. Automated Data Extraction**
- Implemented **web scraping** using the **Wikipedia RESTful API** to extract structured data from monarch biography infoboxes.  
- Parsed relationship attributes (e.g., `parents`, `spouses`, `predecessors`, `successors`) using **JSON query pipelines**.  
- Applied **data validation**, **entity resolution**, and **error handling** to ensure robust data ingestion.

> **Keywords:** Wikipedia API, JSON parsing, RESTful endpoints, data pipeline automation, entity disambiguation.

---

### 🌐 **2. Graph Construction & Analysis**
- Built a **multi-relational social graph** with **NetworkX**, modeling **royal individuals as nodes** and **family or political connections as edges**.  
- Edge attributes encoded **relationship types**: `blood`, `marriage`, and `succession`.  
- Node attributes included temporal metadata (`birth/death`, `reign start/end`) and computed genetic coefficients.  
- Computed **structural graph metrics**:
  - *Degree centrality*  
  - *Betweenness centrality*  
  - *Graph connectivity* and *component analysis*  
  - *Community modularity*  

> **Keywords:** graph analytics, knowledge graph, NetworkX, adjacency matrix, social network analysis (SNA), community detection, degree distribution, connected components.

---

### 🧬 **3. Inbreeding Coefficient Computation**
- Implemented a recursive computation of the **inbreeding coefficient** for each individual node:
f(X) = Σ [ 0.5^(n - 1) * (1 + f(A)) ]

where:
- `n` → number of individuals in the ancestral loop between the parents and common ancestor  
- `f(A)` → inbreeding coefficient of the common ancestor  

- Mapped **coefficient distributions** across dynasties and time periods to identify **genealogical bottlenecks**.  
- Compared inbreeding scores across centuries (1450–1700 vs. 1920+) to study **temporal trends in hereditary practices**.

> **Keywords:** graph-based inheritance modeling, genealogical inference, recursive algorithms, computational biology, historical data analytics.

---

### 🧠 **4. Natural Language Processing & Sentiment Analysis**
- Extracted biographical text from Wikipedia pages using **NLP preprocessing** techniques (tokenization, stopword removal, lemmatization).  
- Performed **sentiment analysis** with the **NLTK SentimentIntensityAnalyzer** to evaluate emotional tone and correlate it with health or leadership attributes in monarch biographies.  
- Identified **statistical shifts** in sentiment distributions between high- and low-inbreeding groups.

> **Keywords:** sentiment analysis, text mining, NLTK, feature extraction, computational linguistics, historical text analytics, data-driven storytelling.

---

### 📊 **5. Visualization & Reporting**
- Created **interactive visualizations** using **Plotly** and **Matplotlib** for:
- Graph connectivity patterns  
- Inbreeding distribution histograms  
- Temporal evolution of coefficients  
- Sentiment polarity comparisons  
- Generated **data-driven insights** supported by **reproducible Jupyter notebooks**.

> **Keywords:** data visualization, exploratory data analysis (EDA), Plotly, Matplotlib, network diagrams, Jupyter reproducibility.

---

## 🧰 **Tech Stack**

| **Category** | **Tools & Libraries** |
|---------------|----------------------|
| **Data Extraction** | Wikipedia API, Requests, JSON |
| **Graph Analysis** | NetworkX, Pandas, NumPy |
| **NLP** | NLTK, Regular Expressions |
| **Visualization** | Matplotlib, Plotly |
| **Development** | Python 3.10+, Google Colab, Jupyter Notebook |
| **Version Control** | Git, GitHub |

---

## 📈 **Key Insights**
- Constructed a **royal family knowledge graph** with **7,365 nodes** and **13,259 edges**.  
- Identified **Habsburg** and **Bourbon** dynasties as exhibiting the **highest inbreeding coefficients**.  
- Discovered that **modern royal lineages (post-1920)** retain genetic correlation patterns despite sociocultural shifts.  
- Observed **sentiment polarity variations** correlated with high genetic similarity scores, offering preliminary evidence of potential cognitive or reputational bias.

---

## 🧩 **Research & Industry Relevance**
This project bridges **computational social science**, **historical data mining**, and **applied graph learning**, demonstrating skills highly relevant to roles in:
- **AI-driven Knowledge Graphs**  
- **Social Network Analysis**  
- **Data Mining and API Engineering**  
- **NLP and Text Analytics**  
- **Data Science for Research and Policy Analytics**

---

## ⚙️ **How to Run**

Clone the repository and open the notebook in **Google Colab** or **Jupyter**.

```bash
# Clone the repo
git clone https://github.com/yourusername/social-graphs-royal-analysis.git
cd social-graphs-royal-analysis

# Install dependencies
pip install -r requirements.txt

# Open notebook
jupyter notebook COLAB_FINAL_PROJECT.ipynb


