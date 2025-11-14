# Antibiotic Resistance Visualisation

This project explores how clinical antibiotic resistance trends relate to environmental antibiotic contamination.

Using clinical MIC (Minimum Inhibitory Concentration) data for *Neisseria gonorrhoeae* (1979–2017) and pharmaceutical concentration measurements from the Thames River (2009–2011), the analysis:

- visualises resistance trends for key antibiotics such as Azithromycin and Ciprofloxacin,
- compares resistance patterns across regions (UK, USA, Canada, Denmark, Japan),
- and examines whether low-level antibiotic contamination in water systems may act as an environmental reservoir for resistance.

---

## Objectives & Research Questions

### **Objectives**
- Investigate trends in antibiotic resistance over time in different regions.
- Examine environmental reservoirs of resistance genes in water systems.
- Analyse how environmental contamination may contribute to clinical resistance patterns.

### **Research Questions**
1. How have resistance levels for key antibiotics (e.g. Azithromycin, Ciprofloxacin) changed over time across different countries or regions, and which regions show the most pronounced increases or stable trends?
2. What do measured antibiotic concentrations in the Thames River reveal about potential environmental reservoirs of resistance, particularly for widely used antibiotics like Azithromycin and Ciprofloxacin?
3. Which factors—such as antibiotic type, region, or water contamination levels—most strongly predict or correlate with rising clinical resistance trends?

---

## Datasets Used

### **1. Clinical Resistance Dataset (1979–2017)**
- Source: Kaggle — *Predicting Antibiotic Resistance in Gonorrhoea*
- Includes MIC values and binary resistance indicators for Azithromycin, Ciprofloxacin, Ceftriaxone, Cefixime, Tetracycline, and Penicillin.

### **2. Thames River Pharmaceutical Concentrations (2009–2011)**
- Source: EU Data Portal
- Contains measured concentrations (ng/L) of Azithromycin, Ciprofloxacin, and Doxycycline at 21 monitoring locations.

Together, these datasets allow an integrated exploration of clinical and environmental dimensions of antimicrobial resistance.

---

## Tech Stack

- Python  
- Jupyter Notebook  
- pandas  
- numpy  
- matplotlib  
- seaborn  

---

## Files in this Repository

- `Antibiotic_Resistance_Visualisation.ipynb` — main analysis notebook  
- `metadata.csv` — clinical antibiotic resistance dataset  
- `River_PharmaConcentrations.csv` — Thames River dataset  
- `requirements.txt` — Python dependencies  

---

## How to Run

You can run this notebook either locally on your machine or in any Jupyter-based environment (JupyterHub, JupyterLab, VS Code, Google Colab, etc.).

### **Option A — Running Locally**

1. (Optional) Create and activate a Python virtual environment.
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Launch Jupyter Notebook or JupyterLab:

   ```bash
   jupyter notebook
   ```
   or  
   ```bash
   jupyter lab
   ```

4. Open `Antibiotic_Resistance_Visualisation.ipynb` and run all cells.

---

### **Option B — Running on JupyterHub / JupyterLab**

1. Upload:
   - `Antibiotic_Resistance_Visualisation.ipynb`
   - `metadata.csv`
   - `River_PharmaConcentrations.csv`

2. Open the notebook directly in the interface.

3. Ensure the correct Python kernel is selected (with pandas, numpy, matplotlib, seaborn).

4. Run all cells from top to bottom — no installation needed if the environment already provides the required libraries.


---

## Key Insights

### **Clinical Resistance**
- #### **Rising resistance in key antibiotics**:
  **Ciprofloxacin** and **Azithromycin** show clear increases in MIC values over time in several regions (e.g. UK, USA, Canada, Japan). For many years, mean MICs exceed EUCAST resistance thresholds, confirming widespread resistance.
  **Azithromycin** resistance shows rising trends in the UK, USA, and Canada, with occasional extreme MIC outliers up to 512 mg/L.
- #### **Older antibiotics largely unusable**:
  **Penicillin** and **Tetracycline** exhibit high MIC values and widespread high resistance levels, consistent with their removal from front-line treatment.
- #### **Critical, but under pressure**:
  **Ceftriaxone** and **Cefixime** remain mostly effective, but creeping increases and occasional spikes highlight the importance of continued monitoring for these last-line treatments.


### **Environmental Contamination**
- #### **Environmental contamination is persistent and increasing**:
  Antibiotic concentrations in the Thames River **increased** between 2009 and 2010–2011 for Azithromycin, Ciprofloxacin and Doxycycline, with greater variability in the later period. Higher variability in the inter-pandemic period suggests changes in pharmaceutical usage or wastewater management.

- #### **Sub-inhibitory environmental levels still matter**:
  Although levels are far below (ng/L) clinical MICs, persistent exposure may act as a selective pressure and reservoir for resistance genes in environmental bacteria.

---

## Skills & Topics Demonstrated

- Data cleaning & preprocessing (handling special MIC values like `>`, `<`, `>=`)
- Exploratory Data Analysis (EDA)
- Visualisation techniques:
  - histograms  
  - pie charts  
  - scatter plots  
  - box plots  
  - grouped bar charts  
  - time-series trends by country  
- Outlier handling with IQR filtering
- Integration of clinical and environmental datasets
- Interpretation using EUCAST resistance breakpoints
- Scientific reasoning and narrative explanation

---

## Summary

This project demonstrates how data visualisation can illuminate the complex interplay between clinical antibiotic resistance and environmental contamination. By combining resistance surveillance with aquatic pharmaceutical data, it highlights the multi-layered nature of antimicrobial resistance and underlines the importance of both clinical stewardship and environmental management.

---
