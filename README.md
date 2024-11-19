# **Data-Driven Investigations into Author Productivity and Citation Patterns**  

## **Project Overview**  
This project explores author productivity and citation trends across academic disciplines, with a focus on computer science. Using the [OpenCitations Meta](https://opencitations.net/meta) dataset, this research uncovers key insights into how citations have evolved over two decades (2000–2020). The study addresses two core research questions:  

1. **What are the trends in the number of citations and authors over time?**  
2. **Are there significant differences in hyperprolific authorship between computer science and other fields?**  

By leveraging Python, Apache Spark, and Pandas, the project delivers a comprehensive analysis through advanced data cleaning, augmentation, and visualization techniques.  

---

## **Server Environment**  

The analysis and data processing were conducted on **JupyterLab** running on a Kubernetes-based server. The server environment provided:  

- **Jupyter/scipy-notebook: Python 3.9 + Spark Gateway**  
- **Reserved Resources**:  
  - 35 CPU Threads and 120 GB Memory  
  - Maximum Capacity: 60 CPU Threads and 260 GB Memory  

This setup ensured the scalability and performance needed to handle the large OpenCitations Meta dataset (50 GB). Python dependencies were managed using **mamba**, **conda**, or **pip** within the environment.  

---

## **Features**  

- **Data Cleaning and Preprocessing**:  
  - Removed duplicates, null values, and non-Latin characters.  
  - Filtered data by discipline using DBLP ISSN/ISBN values.  
  - Incremental saving strategy for robust data processing.  

- **Visualization and Analysis**:  
  - Temporal trends of citations using CDF and PMF.  
  - Researcher's Article Growth Speed (RAGS) to track changes in publication rates.  
  - Comparative analysis of citation patterns between computer science and the general dataset using CCDF.  

---

## **Data Source**  
This project utilizes the **OpenCitations Meta dataset (Version 7, released February 2024)**, a comprehensive open-source database of bibliographic metadata. The dataset was refined with additional data from **DBLP** for enhanced accuracy in computer science-specific analyses.  

---

## **Key Findings**  

1. **Temporal Citation Trends**  
   - From 2000 to 2020, total citations increased significantly.  
   - However, the growth rate (RAGS) has steadily declined, indicating a slowing pace of citation accumulation.  

2. **Comparative Analysis of Citation Patterns**  
   - Computer science exhibits a sharper concentration of citations among fewer authors compared to the general dataset.  
   - By 2020, citation distribution in computer science became slightly more balanced, though the "long tail" phenomenon remains prominent.  

---

## **Project Structure**  

```
📂 Project Root  
 ├── 📂 data_cleaning/         # Scripts for data preprocessing and augmentation  
 ├── 📂 analysis_visualization/ # Jupyter Notebooks for analysis and visualization  
 ├── README.md                 # Project documentation  
 ├── requirements.txt          # Python dependencies  
```

---

## **Technologies Used**  

- **Python**: Core programming language for data analysis.  
- **Apache Spark**: For scalable data cleaning and processing.  
- **Pandas**: For handling smaller, filtered datasets.  
- **Matplotlib/Seaborn**: For data visualization.  
- **Jupyter Notebook**: Interactive data analysis environment.  

---

## **How to Cite**  

If you use this project in your research, please cite:  
**Banaudi, A.** "Data-Driven Investigations into Author Productivity and Citation Patterns," Bachelor Thesis, University of Turin, 2024.  

---

## **Acknowledgments**  

This project was supervised by **Prof. Idilio Drago** at the **University of Turin** and made possible by the data provided by **OpenCitations Meta**.  

