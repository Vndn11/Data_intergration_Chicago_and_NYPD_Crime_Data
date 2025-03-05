### **Crime Data Integration and Mapping: NYPD & Chicago Crime Datasets**

#### **📌 Project Overview**
This project focuses on **integrating, matching, and mapping crime datasets** from **New York Police Department (NYPD) and Chicago Police Department (CPD)**. The goal is to **align crime descriptions, arrest records, and criminal activities** between the two cities by using **machine learning techniques, specifically BERT embeddings and cosine similarity**, to match different crime categories.

---

### **📂 Datasets Used**
The project integrates multiple datasets from **Chicago** and **New York**, including:

1. **Chicago Crimes Dataset** – Records of crimes reported in Chicago.
2. **NYPD Arrests Dataset** – Details of arrests made in New York.
3. **NYPD Shooting Dataset** – Data related to shooting incidents in New York.
4. **NYPD Criminal Summons Dataset** – Records of issued criminal summons.
5. **Chicago IUCR Laws Dataset** – Legal classification of crimes in Chicago.

---

### **🔍 Data Preprocessing & Cleaning**
The datasets are preprocessed by:
✔ Filtering records after **2014** for consistency.  
✔ Converting **date formats** to standard datetime format.  
✔ Standardizing key fields like **FBI Codes** and **IUCR Codes**.  
✔ Cleaning and handling **missing values**.  
✔ Converting law descriptions into numerical representations for similarity calculations.  

---

### **🛠 Matching Crime Descriptions Across Cities Using BERT**
Since crime descriptions vary between the NYPD and CPD datasets, **BERT (Bidirectional Encoder Representations from Transformers)** is used to find **semantic similarities** between crime descriptions.

1. **Generating BERT Embeddings:**  
   - Tokenized **NYPD offense descriptions** and **Chicago IUCR crime descriptions**.  
   - Converted text into **BERT embeddings** (numerical vectors).  
   
2. **Computing Cosine Similarity:**  
   - Matched **NYPD offenses** to the closest **IUCR crime category** using cosine similarity.  
   - Identified **most similar laws** for mapping across the two datasets.  

---

### **🔗 Crime Data Integration & FBI Code Mapping**
✔ **Mapped NYPD crime descriptions to Chicago’s IUCR legal codes** using the similarity scores.  
✔ **Mapped IUCR codes to FBI crime classification codes** to standardize crime types.  
✔ Created a unified **"Master Arrest Dataset"** and **"Master Crime Dataset"** that integrates information from both cities.  

---

### **📊 Key Results**
📌 **Successfully mapped NYPD crimes to equivalent Chicago IUCR codes** using **BERT-based similarity matching**.  
📌 **Standardized crime reporting across the two cities**, enabling cross-city crime trend analysis.  
📌 Generated two comprehensive datasets:
   - **Master Arrest Dataset** (`Master_Arrest.csv`)
   - **Master Crime Dataset** (`Master_Crime.csv`)

---

### **🚀 Future Enhancements**
🔹 Implement **Deep Learning models (Transformers)** to improve law-matching accuracy.  
🔹 Expand integration with other **major US cities** for a national crime comparison model.  
🔹 Create **visual dashboards** to analyze and compare crime trends across cities.  

