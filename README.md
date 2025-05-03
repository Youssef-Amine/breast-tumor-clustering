This project analyses breast tumors cells to discover trends and connections between certain features and diagnoses through unsupervised method (Clustering). 
---

## Objectives

- Find the simple connections between features with an Exploratory Data analysis
- Reduce dimensionalty trough a principal component analysis (PCA)
- Cluster data regarding the principal features 
- Visualize clusters in function of target feature diagnosis to see which tumors are more likely to be a cancer

## Project Structure

```bash
breast-tumor-clustering/
|
├── README.md                  # Project description
├── requirements.txt           # Required Packages 
├── wcbd.csv                    # Data
├── BreastCellTumorClustering   # Working notebook
```


---

##  Technology used

- Python (pandas, numpy, matplotlib, seaborn)
- Feature_engine
- Sklearn (PCA, Kmeans)

---

##  Results
Clusters identified
Cluster 1: groups observations with low PC1 values and moderate PC2 values, i.e. smaller, more regular tumors.
Cluster 0 : high PC2 values and centered around an average PC1 values, normal size and irregular tumors.
Cluster 2: strongly to the right on PC1, therefore associated with larger, more regular tumors, according to the important PCA variables.

Conclusion:
Clustering into 3 groups seems relevant. Each cluster has potential biological significance in relation to tumor morphology and regularity.
These clusters can be crossed with the diagnosis features to explore which type of tumor is more likely to be a cancer.
Most tumors from Cluster 1 are Benign and most tumors from Cluster 2 tumors are Malignant. 
Smaller and regular tumors are benign and larger but regular tumor are more like to be a cancer. 
Size highly determines if a tumor is a cancer but the regularity no because Cluster 0 where tumors are the most irregular contains as many benign as malignant tumors. 


## 📚 References

- https://www.kaggle.com/datasets/mdimraniqbal/breastcancer

---

> Portfolio project developed in 2025 by Youssef SAWADOGO. If you have any questions, please contact me via wyoussef.sawadogo@gmail.com
