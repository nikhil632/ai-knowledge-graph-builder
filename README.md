# ai-knowledge-graph-builder
AI-powered system for building dynamic enterprise knowledge graphs using RAG, embeddings, and semantic pipelines.

# 🧠 AI Knowledge Graph Builder – Milestone 1  
### Enterprise Data Cleaning, Transformation, Normalization & Enrichment

This repository contains the completed **Milestone-1** of the AI Knowledge Graph Builder internship project.  
The objective of this milestone is to prepare high-quality enterprise data that will be used to create a Knowledge Graph in the next milestone.

---

## 📌 Milestone-1 Tasks Completed

### ✔ **1. Data Ingestion**
Loaded the raw Fortune 1000 (2024) dataset using Pandas.

### ✔ **2. Data Understanding**
- Inspected dataset shape and columns  
- Identified categorical and numeric fields  
- Checked missing values  
- Detected data quality issues (mixed yes/no, numeric NaN, inconsistent text)

### ✔ **3. Data Cleaning**
- Removed duplicate company entries  
- Converted Yes/No fields to numerical (1/0)  
- Standardized text (Company, Sector, Industry, CEO)  
- Cleaned numeric columns  
- Handled missing values (market cap, profits, percent changes)

### ✔ **4. Data Transformation**
- Created `Rank_Score` (1000 = best rank)  
- Converted assets and market cap from millions to billions  
- Added derived financial metrics

### ✔ **5. Data Normalization**
Applied MinMaxScaler to:
- Assets  
- MarketCap  
- Rank  

This makes values suitable for ML, similarity calculation, and KG algorithms.

### ✔ **6. Data Enrichment**
Added enterprise knowledge fields:
- `Continent` (derived from Country)
- `Company_Size` (Mega / Large / Medium / Small based on Assets)


---

## 📊 Output
- Final cleaned & enriched dataset: **fortune1000_cleaned.csv**
- Jupyter notebook with detailed steps: **Milestone1_Data_Preprocessing.ipynb**

Both files are ready for use in Knowledge Graph creation (Milestone-2).

---

## 🚀 Next Steps (Milestone-2)
- Create Knowledge Graph Schema  
- Build nodes: Company, Sector, Industry, CEO, Country  
- Build edges and relationships  
- Visualize using NetworkX / Neo4j  

---

## 👤 Author
**Nikhil Ghule**  
Intern — AI Knowledge Graph Builder Project



