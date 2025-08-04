# Customer Segmentation Using K-Means Clustering

This project uses **unsupervised machine learning**—specifically, the **K-Means clustering algorithm**—to segment customers based on their behavior. The goal is to group similar customers together, which can help businesses tailor marketing strategies, improve customer experience, and enhance decision-making.

## 📌 Project Overview

* **Problem Statement:**
  Businesses often have large customer bases with varied behavior. Understanding customer segments helps in targeted marketing and improving services. This project clusters customers using features like Age, Income, and Spending Score.

* **Approach:**
  We use the **K-Means algorithm**, a popular clustering technique, to group customers into distinct segments based on numerical features.

## 🔧 Technologies Used

* **Python**
* **Jupyter Notebook**
* **Pandas** – Data manipulation
* **Matplotlib** & **Seaborn** – Data visualization
* **Scikit-learn** – Machine learning (KMeans)

## 📊 Dataset

The dataset used includes the following columns:

* `CustomerID`
* `Gender`
* `Age`
* `Annual Income (k$)`
* `Spending Score (1-100)`

> 📁 The dataset is loaded from a `.csv` file (you may need to ensure the dataset is available in your working directory).

## 📈 Steps Performed

1. **Data Loading and Exploration**

   * Loaded dataset using Pandas.
   * Explored the data using `head()`, `info()`, and visualizations.

2. **Data Visualization**

   * Used histograms, pairplots, and count plots to understand distributions.
   * Visualized relationships between variables like income vs. spending score.

3. **Preprocessing**

   * Cleaned the data (e.g., removed unnecessary columns).
   * Focused on numerical columns for clustering.

4. **Choosing Optimal Clusters**

   * Used the **Elbow Method** to determine the best number of clusters.

5. **Applying K-Means Clustering**

   * Fit the model on selected features.
   * Plotted the clusters with different colors to interpret the segments.

6. **Cluster Analysis**

   * Analyzed each cluster's behavior to understand key traits (e.g., high-income low-spending, etc.).

## 📷 Visual Outputs

The notebook includes several helpful plots:

* Elbow plot for optimal `k`
* Scatter plots of clusters
* Heatmaps and distribution plots for feature understanding

## 🧠 Key Learnings

* K-Means is effective for identifying patterns in unlabelled data.
* Visualizations are key to interpreting unsupervised results.
* The Elbow method is crucial in selecting the right number of clusters.

## 🚀 How to Run

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Launch the notebook:

   ```bash
   jupyter notebook Customer_Segmentation_Using_K_Means_Clustering_Machine_Learning_Project.ipynb
   ```

> ✅ Make sure to place the dataset CSV in the same directory, or update the path in the notebook.

OR

4. If you are using google colab, directly create kaggle token in profile settings,this will download kaggle.json file,upload it in google colab and then copy code and run all cells.
   ! pip install kaggle  # first step
   Api command to download dataset through kaggle:
   #!/bin/bash
!kaggle datasets download vjchoudhary7/customer-segmentation-tutorial-in-python  # api command to download dataset


## 📄 Requirements

pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
kaggle
```

## 🏁 Conclusion

This project demonstrates how businesses can use clustering techniques like K-Means to better understand their customers. With simple yet powerful visualizations and machine learning, customer behavior insights become more actionable.

## 📬 Contact

For questions or collaboration:

* Email: 411963ar@gmail.com

Insights:
1.People with small or less annual income ususally have high spending score or they spent more in mall compare to those with high annual income.

2.People with high annual income mostly have low spending score or they spend less in mall as compare to those with low annual income

3.People with low annual income and high spending scores can be offered with gift cards,loyality cards etc

4.Group of people with low annual income and low spending score can be offered with discounts,packages,offers to attract them and generate more sales.

Elbow method for choosing suitable number of clusters:
Using wcss- meaning: - with in clusters sum of squares - is basically a performance metrics to find the suitable number of clusters.It measure distance of each data point with its respective centroid, then square it to avoid negatives and then take sum all scores,this will give wcss value,we get different wcss values for different number of clusters, and use elbow method that shows a sudden slow down which indicates best number of suitable clusters.
