# 🎰 Lotto Max Number Predictor

A comprehensive data analysis and machine learning project that analyzes historical Lotto Max lottery data to generate number predictions using multiple statistical and AI approaches.

> **⚠️ Disclaimer:** This project is for **educational and entertainment purposes only**. Lottery draws are truly random events, and past results do not predict future outcomes. These predictions have no real predictive power. Please play responsibly.

## 📊 Project Overview

This Jupyter notebook analyzes over **1,205 historical Lotto Max draws** spanning from September 2009 to January 2026, applying seven different prediction methodologies and combining them through an ensemble voting system to generate final number recommendations.

## 🎯 Features

### Data Analysis
- **Historical data processing** of 1,205+ lottery draws
- **Frequency analysis** of all numbers (1-50)
- **Temporal trend analysis** (hot and cold numbers)
- **Statistical visualizations** including heatmaps, distribution charts, and trend graphs
- **Comprehensive data quality checks**

### Seven Prediction Methods

1. **Frequency-Based Analysis**
   - Identifies the most frequently drawn numbers across all historical draws
   - Based on long-term statistical patterns

2. **Hot Numbers Strategy**
   - Analyzes the last 50 draws to identify trending numbers
   - Focuses on recently popular numbers

3. **Cold Numbers Strategy**
   - Identifies "overdue" numbers that haven't appeared recently
   - Based on the theory of statistical regression to the mean

4. **Balanced Approach**
   - Combines hot and cold numbers strategically
   - Creates a mix of trending and overdue numbers

5. **Pattern-Based Analysis**
   - Examines historical patterns in number selection
   - Looks for correlations between number appearances

6. **Random Forest Machine Learning**
   - Uses scikit-learn's Random Forest Classifier
   - Trains on historical data to learn drawing patterns
   - Feature engineering based on number frequencies and temporal data

7. **XGBoost Algorithm**
   - Advanced gradient boosting machine learning model
   - Optimized for pattern recognition in lottery data
   - Provides probability-based predictions

### Ensemble Voting System

The project's crown jewel is the **ensemble prediction system** that:
- Collects predictions from all seven methods
- Uses a democratic voting mechanism
- Weights predictions based on method confidence
- Generates a final set of 7 main numbers and bonus number
- Provides alternative bonus numbers ranked by votes

## 📦 Dependencies

```python
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
```

## 🚀 How to Use

1. **Clone the repository**
   ```bash
   git clone https://github.com/Ray-Aldred/lotto-fun/edit/main/lotto-max-predictor.git
   cd lotto-max-predictor
   ```

2. **Install required packages**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost
   ```

3. **Open the Jupyter notebook**
   ```bash
   jupyter notebook Lotto_Max_Predictor.ipynb
   ```

4. **Run all cells** to generate predictions

5. **View outputs**
   - Visualization charts (saved as PNG files)
   - `prediction_summary.txt` with detailed results
   - Console output with all predictions

## 📈 Output Structure

### Main Prediction Output
- **7 Main Numbers**: Selected through ensemble voting
- **Primary Bonus Number**: Most voted bonus number
- **Alternative Bonus Numbers**: Top 5 backup bonus numbers

### Individual Method Predictions
Each of the seven methods generates its own set of 7 numbers, allowing you to:
- Compare different approaches
- Understand the reasoning behind each method
- Choose your preferred strategy

### Statistical Reports
- Most frequent numbers (all-time)
- Hot numbers (last 50 draws)
- Cold numbers (overdue)
- Voting distribution charts
- Frequency comparison visualizations

## 🔍 What I Implemented

### 1. Data Loading and Preprocessing
- Imported historical Lotto Max data with 1,205 draws
- Converted date formats for temporal analysis
- Validated data integrity and handled missing values
- Created separate arrays for main numbers and bonus numbers

### 2. Exploratory Data Analysis (EDA)
- **Frequency Distribution**: Calculated how often each number (1-50) appears
- **Temporal Analysis**: Tracked number trends over time
- **Statistical Summaries**: Mean, median, and range calculations
- **Correlation Analysis**: Examined relationships between numbers

### 3. Visualization Suite
Created multiple visualization types:
- **Bar charts** for number frequency distribution
- **Heatmaps** for number co-occurrence patterns
- **Line graphs** for temporal trends
- **Comparison charts** for method predictions
- **Voting distribution charts** for ensemble results

### 4. Prediction Algorithms

#### Statistical Methods
- Implemented frequency counting with pandas Counter
- Created rolling window analysis for hot/cold numbers
- Developed weighted selection algorithms

#### Machine Learning Models
- **Random Forest Classifier**
  - Feature engineering (frequency, recency, position)
  - Hyperparameter tuning
  - Probability-based selection
  
- **XGBoost Model**
  - Advanced gradient boosting implementation
  - Cross-validation for model validation
  - Feature importance analysis

### 5. Ensemble System
- Collected all predictions in a unified voting pool
- Implemented ranked voting mechanism
- Applied tie-breaking rules
- Generated confidence scores for each number

### 6. Reporting System
- Automated summary generation
- Timestamp and metadata inclusion
- Formatted text output with clear sections
- File export functionality

## 📊 Sample Output

```
======================================================================
🎯 FINAL ENSEMBLE PREDICTION
======================================================================
Main Numbers: [7, 9, 19, 23, 28, 30, 39]
Bonus Number: 18

Alternative Bonus: [38, 46, 27, 1, 10]
======================================================================
```

## 🛠️ Technical Implementation Details

### Data Structure
- **Input**: CSV/DataFrame with columns: Date, Number1-7, Bonus
- **Processing**: Flattened arrays for frequency analysis
- **Feature Engineering**: Temporal features, frequency encoding, position encoding

### Algorithm Performance
- Random Forest: Trained on 1,000+ samples
- XGBoost: Optimized with early stopping
- Ensemble: Combines 7 independent predictions

### Validation Approach
While true validation is impossible (lottery is random), the project includes:
- Historical backtesting framework
- Cross-validation for ML models
- Comparison of predicted vs. actual distributions

## 📚 Learning Outcomes

This project demonstrates:
- **Data wrangling** with pandas
- **Statistical analysis** and probability theory
- **Machine learning** classification techniques
- **Ensemble methods** and voting systems
- **Data visualization** best practices
- **Scientific computing** with NumPy
- **Project documentation** and reproducibility

## 🎓 Educational Value

Perfect for learning:
- How to approach a data science problem from scratch
- Combining multiple analytical approaches
- Implementing machine learning for pattern recognition
- Creating ensemble prediction systems
- Data visualization and reporting
- Working with time-series and categorical data

## 🤝 Contributing

Feel free to fork this project and experiment with:
- Additional prediction algorithms
- Different ensemble voting mechanisms
- Enhanced visualization techniques
- Alternative data sources
- Comparative analysis of different lotteries

## 📝 License

This project is open source and available for educational purposes.

## ⚖️ Responsible Gaming

Remember:
- Lottery games should be played for entertainment only
- Never spend more than you can afford to lose
- These predictions are statistically no better than random selection
- The house always has the edge in lottery games
- Seek help if gambling becomes a problem

## 🔗 Resources

- [Lotto Max Official Website]([https://www.olg.ca/en/lottery/play-lotto-max.html](https://lottomax.ca/))
- [Understanding Lottery Odds](https://en.wikipedia.org/wiki/Lottery_mathematics)

---

**Made with** 🧠 **for learning and** 🎲 **for fun**

*Remember: The only guaranteed way to win the lottery is not to play! This project is purely educational.*
