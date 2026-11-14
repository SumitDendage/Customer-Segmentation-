# Customer Segmentation with K-Means

Groups mall customers into segments by **annual income** and **spending score** using K-Means clustering, so marketing can target each group differently (for example high-income/low-spend customers versus young high spenders).

![Python](https://img.shields.io/badge/Python-3.9+-3776AB?logo=python&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-EDA-150458?logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-K--Means-F7931E?logo=scikitlearn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)

## Workflow

1. **Data overview** – 200 customers with `CustomerID`, `Gender`, `Age`, `Annual Income (k$)` and `Spending Score (1-100)`; shape, types, missing values and summary statistics.
2. **Feature selection** – income and spending score, the two dimensions that matter most for targeting.
3. **Choosing *k*** – the **elbow method**: within-cluster sum of squares (WCSS) for *k* = 1…10.
4. **Clustering** – K-Means (`k-means++` initialisation) with **5 clusters**.
5. **Visualisation** – customers coloured by segment, with cluster centroids.

## Segments to look for

With income on one axis and spending on the other, five clusters typically separate into: high income / high spend (priority customers), high income / low spend (untapped potential), low income / high spend, low income / low spend, and an average middle group.

## Run it

```bash
git clone https://github.com/SumitDendage/Customer-Segmentation-.git
cd Customer-Segmentation-
pip install pandas matplotlib seaborn scikit-learn jupyter
```

Download the **Mall Customer Segmentation Data** (`Mall_Customers.csv`) from Kaggle into the folder, then:

```bash
jupyter notebook customer.ipynb
```

## Author

**Sumit Dendage** · [GitHub](https://github.com/SumitDendage) · [LinkedIn](https://www.linkedin.com/in/sumit-dendage-636a50201) · [Medium](https://dendagesumitbalkrishna123.medium.com)
