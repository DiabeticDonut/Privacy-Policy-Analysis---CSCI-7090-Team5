# Privacy-Policy-Analysis---CSCI-7090-Team5

## Project Overview

The pipeline consists of the following steps:

1. **Transform Knowledge Graphs**  
   Parses `.yml` files representing app privacy graphs and converts them into structured tabular data.

2. **Exploratory Data Analysis (EDA)**  
   Visualizes patterns in purposes, relations, and data collection entities.

3. **Clustering**  
   Uses TF-IDF + metadata features and K-Means to identify clusters of data handling behaviors.

4. **Dimensionality Reduction & Visualization**  
   Applies SVD, t-SNE, and UMAP to visualize clusters in 2D space.

5. **Evaluation**  
   Calculates Silhouette and Trustworthiness scores to assess clustering quality and embedding fidelity.

---


##  How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/privacy-policy-clustering.git
cd privacy-policy-clustering
```

### 2. Install Dependencies

Make sure you have Python 3.7+ installed.

Install all required Python libraries using:

```bash
pip install -r requirements.txt
```
   
### 3. Prepare the Graph Files
Make sure all '.yml' knowledge graph files in a folder named:
'graphfiles/'

### 4. Launch the Notebook and Run all the cells

Open 'CSCI_7090_Team_5.ipynb' in Jupyter or Google Colab.


## Folder Structure

```bash
Privacy-Policy-Analysis---CSCI-7090-Team5/
├── graph files/                  # YAML knowledge graphs
├── data/                        # CSV output
│   └── privacy_policy_data.csv  # Will be generated after running transform_graphs()
├── CSCI_7090_Team_5.ipynb       # Main notebook
├── requirements.txt             # Python dependencies
└── README.md
```

## Key Functions
```bash
| Function               | Description                                     |
| ---------------------- | ----------------------------------------------- |
| `transform_graphs()`   | Converts YAML graphs to a CSV format            |
| `perform_eda()`        | Visualizes source, target, and purpose patterns |
| `perform_clustering()` | Applies clustering and dimensionality reduction |
| `eval()`               | Computes evaluation metrics for embeddings      |
```

