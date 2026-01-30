# Data-Analytics-Project
Estimating &amp; Forecasting UK Manufacturing Emissions using ML &amp; Deep Learning

This project develops a predictive data science framework to quantify and forecast harmful pollutant emissions across all manufacturing sub-sectors in the United Kingdom. Utilizing the UK National Atmospheric Emissions Inventory (NAEI) dataset, the study applies various Machine Learning (ML), Artificial Neural Networks (ANN), and Deep Learning methodologies to support the UK's net-zero policy.

### 📋 Project Overview
#### Objective: 
Provide fact-based estimates and business insights for industrial decarbonization across the UK.

#### Dataset: 
UK NAEI Point Source Emissions (2020 cycle), containing 64,026 observations and 14 technical features.

#### Core Problem: 
Industrial clusters are major contributors to global warming; this project models these complex emission patterns to identify key drivers.

### 🛠️ Tech Stack
#### Language: 
Python Programming

#### Libraries:
1) Data Handling: Pandas, NumPy 
2) Visualization: Matplotlib, Seaborn 
3) Machine Learning: Scikit-Learn 
4) Deep Learning: TensorFlow, Keras 

### 🏗️ Methodology
The project follows a rigorous data science pipeline:
1) Data Acquisition: Collection of point source data including grid references (Easting/Northing) and pollutant IDs.
2) Data Cleaning: Removal of records with missing spatial data and handling of approximately 33 different pollutants.
3) Exploratory Data Analysis (EDA):
      a) Discovered that England accounts for the highest concentration of emissions (73.03% of total) due to industrial clusters.
      b) Analyzed emissions by sector, noting that "Major Power Producers" are significant contributors.
4) Pre-processing:
      a) Categorical Encoding: Used get_dummies for features like 'Region' and 'Datatype'.
      b) Feature Selection: Applied Pearson’s Correlation Coefficient to identify highly associated inputs.
      c) Scaling: Implemented StandardScaler to normalize data points for improved model convergence.
5) Model Building: Built a 80/20 train-test split to evaluate five different architectures.

### 🤖 Models Implemented
1) Decision Tree Regressor: Used for its simplicity and interpretability.
2) Random Forest Regressor: An ensemble method that reduced overfitting and provided the highest accuracy.
3) Gradient Boosting: Focused on boosting performance by integrating weak learners.
4) Multi-Layer Perceptron (MLP): A neural network architecture utilizing backpropagation.
5) Deep Learning (TensorFlow): Implemented deep neural networks with multiple hidden layers to capture non-linear relationships.

### 📈 Evaluation & Results
Models were evaluated based on Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and R² Score.
1) Top Performer: The Random Forest Regressor outperformed other models by effectively managing the complex, large-scale dataset.
2) Insights: The research successfully identified spatial pollutant distributions, supporting targeted decarbonization strategies for specific UK regions.
