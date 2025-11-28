# Amazon Prime Video Content Analysis

## Project Overview
Comprehensive Exploratory Data Analysis (EDA) and Machine Learning analysis on the Amazon Prime Video dataset. This project profiles titles (movies and TV shows), analyzes content distribution across genres, release years, and countries, and builds predictive models for content scoring.

## 📊 Project Structure

### Notebooks
- **`Amazon_Prime_Video_Content_...ipynb`** - Main EDA analysis covering:
  - Data loading and cleaning
  - Genre analysis and normalization
  - Release year trends
  - Content type distribution (Movies vs Shows)
  - Top actors and directors
  - Geographic content distribution
  - Visualizations and key insights

- **`Amazon_Prime_ML_Submission_...ipynb`** - Machine Learning model for content scoring:
  - Automated target variable selection
  - Feature engineering from titles and genres
  - Model training (Baseline, Linear Regression, Random Forest)
  - Performance evaluation and feature importance
  - Predictive insights

### Data Files
- **`titles.csv.zip`** - Main titles dataset (9,871 rows)
  - Fields: id, title, type, description, releaseYear, runtime, genres, imdbScore, tmdbScore, etc.
  - Includes metadata for movies and TV shows

- **`credits.csv.zip`** - Credits dataset (124,235 rows)
  - Fields: personId, id, name, character, role (ACTOR/DIRECTOR/WRITER)
  - Links cast and crew to titles

### Visualizations
- **`year_trend.png`** - Titles released per year (1912-2022)
- **`top_genres.png`** - Top 20 genres distribution
- **`content_type_counts.png`** - Movies vs Shows breakdown

## 🔍 Key Findings

### Dataset Insights
- **Total Titles**: 9,871 (spanning 110 years)
- **Content Mix**: Dominated by movies (~87%) with TV shows (~13%)
- **Top Genres**: Drama, Comedy, Thriller, Romance, Action
- **Release Pattern**: Sharp increase in content from 2015 onwards

### EDA Discoveries
- Drama is the most prevalent genre across all content
- Most titles released between 2020-2022
- Geographic diversity with strong US presence
- Genre combinations reveal common pairing patterns

### ML Model Performance
- **Target Variable**: Runtime (selected for availability and variance)
- **Best Model**: Random Forest
- **Key Features**: Type (Show/Movie), Release Year, TMDB Popularity, IMDb Score
- **Top Predictive Feature**: Content Type (35.8% importance)

## 🛠️ Technologies & Libraries
- **Python 3.8+**
- **Data Analysis**: Pandas, NumPy
- **Machine Learning**: Scikit-learn (Random Forest, Linear Regression)
- **Visualization**: Matplotlib, Seaborn
- **Development**: Jupyter Notebook

## 📈 Files Information

| File Name | Size | Purpose |
|-----------|------|----------|
| titles.csv.zip | ~100MB | Main dataset with all title information |
| credits.csv.zip | ~50MB | Actor, Director, Writer information |
| Notebooks (.ipynb) | Executed | Complete analysis with outputs and visualizations |
| PNG files | Plots | Key visualizations for presentations |

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas numpy scikit-learn matplotlib jupyter
```

### Usage
1. Extract CSV files: `unzip titles.csv.zip && unzip credits.csv.zip`
2. Open notebooks in Jupyter: `jupyter notebook`
3. Run cells sequentially to reproduce analysis
4. View generated visualizations and model outputs

## 📊 Analysis Workflow

1. **Data Loading** → Clean and validate datasets
2. **EDA Phase** → Explore patterns, distributions, and relationships
3. **Feature Engineering** → Create meaningful features from raw data
4. **Model Building** → Train and compare multiple algorithms
5. **Evaluation** → Assess model performance with key metrics
6. **Insights** → Extract actionable recommendations

## 💡 Key Insights for Stakeholders

- **Content Strategy**: Drama dominates but diversification possible
- **Release Timing**: Recent years show highest content volume
- **Recommendation**: Focus on genre combinations for better recommendations
- **Predictability**: Content type is strong predictor of runtime

## 📝 Data Processing Notes

- Genre strings manually cleaned (brackets, quotes removed)
- Dates parsed and converted to numeric types
- Missing values imputed using median for numerical features
- One-hot encoding applied for categorical variables

## 🎯 Future Enhancements

- [ ] Text analysis on descriptions using NLP
- [ ] Sentiment analysis of reviews
- [ ] Advanced feature engineering with actor/director networks
- [ ] Deep learning models for title prediction
- [ ] Interactive dashboard for content exploration
- [ ] Time-series forecasting for content trends

## 📚 References

- Dataset: Amazon Prime Video public dataset
- Analysis follows EDA and ML submission templates
- Models: Standard supervised learning algorithms

## ✨ Author
**Vishnu27122004** - Engineering Student | Data Analysis | ML Enthusiast

## 📞 Contact & Support
For questions or suggestions, please reach out via:
- GitHub: [@Vishnu27122004](https://github.com/Vishnu27122004)
- LinkedIn: [Profile](https://linkedin.com/in/vishnu27122004)

---

**Last Updated**: November 28, 2025
**Status**: Project Complete ✓
