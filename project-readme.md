# Customer Segmentation Analysis Project

## Overview
This project implements customer segmentation analysis using machine learning techniques to help businesses better understand their customer base and optimize their marketing strategies. The analysis uses various customer attributes including demographics, purchasing behavior, and campaign responses to create meaningful customer segments.

## Dataset Description
The dataset (`marketing_campaign.csv`) contains customer information including:

- Demographics (Age, Education, Family Status)
- Purchase behavior (Spending on different product categories)
- Campaign responses
- Website activity
- Customer loyalty metrics

### Key Features
- Personal Information: Age, Education, Marital Status, Income
- Family Information: Number of Children, Household Size
- Purchase Behavior: Spending across different product categories
- Campaign Response: Success rate of previous marketing campaigns
- Customer Activity: Web visits, purchases, deals used

## Technical Implementation

### Dependencies
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- yellowbrick

### Data Processing Steps
1. Data Cleaning
   - Handling missing values
   - Removing outliers
   - Date formatting
   - Feature engineering

2. Feature Engineering
   - Age calculation
   - Total spending computation
   - Family size derivation
   - Living situation categorization
   - Education level grouping

3. Dimensionality Reduction
   - PCA (Principal Component Analysis) with 3 components

4. Clustering
   - K-means clustering with elbow method for optimal cluster selection
   - Agglomerative clustering implementation

## Analysis Results

### Customer Segments Identified
The analysis identified 4 distinct customer segments based on:
- Spending patterns
- Income levels
- Family composition
- Response to campaigns
- Purchase behavior

### Visualization
The project includes various visualizations:
- Distribution of clusters
- Income vs. Spending patterns
- Campaign acceptance rates
- Demographic profiles
- Purchase behavior analysis

## Usage

1. Data Preparation:
```python
# Load and preprocess data
data = pd.read_csv('marketing_campaign.csv')
data = preprocess_data(data)
```

2. Feature Engineering:
```python
# Create derived features
data = engineer_features(data)
```

3. Clustering:
```python
# Perform clustering
clusters = perform_clustering(data)
```

## Insights and Applications

The segmentation results can be used for:
- Targeted marketing campaigns
- Product recommendations
- Customer retention strategies
- Campaign optimization
- Resource allocation

## Future Improvements

Potential enhancements:
1. Real-time customer classification
2. Integration with CRM systems
3. Dynamic segment updates
4. Additional feature engineering
5. A/B testing framework for marketing campaigns

## Project Structure
```
├── data/
│   └── marketing_campaign.csv
├── notebooks/
│   └── customer_segmentation.ipynb
├── src/
│   ├── preprocessing.py
│   ├── feature_engineering.py
│   └── clustering.py
└── README.md
```

## Contributing
Feel free to fork this project and submit pull requests for any improvements. Please ensure to follow the existing coding style and add appropriate tests for new features.

## License
This project is licensed under the MIT License - see the LICENSE file for details.