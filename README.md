# 🏎️ Formula 1 Race Prediction Project

A machine learning project that predicts Formula 1 race outcomes using historical race data, driver statistics, and track characteristics.

## 📋 Project Overview

This project leverages machine learning algorithms to predict Formula 1 race results including podium positions, fastest laps, and championship standings. By analyzing historical data from previous seasons, the model identifies patterns and makes predictions for upcoming races.

## ✨ Features

- **Race Winner Prediction**: Predict the winner of upcoming F1 races
- **Podium Position Forecasting**: Estimate top 3 finishing positions
- **Fastest Lap Prediction**: Identify likely fastest lap candidates
- **Championship Points Projection**: Forecast driver and constructor standings
- **Historical Data Analysis**: Visualize trends and statistics from past seasons
- **Track-Specific Insights**: Consider circuit characteristics in predictions

## 🛠️ Technology Stack

### Programming & Data Science
- **Python 3.8+**: Primary programming language
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations
- **scikit-learn**: Machine learning algorithms
- **TensorFlow/Keras**: Deep learning models (optional)

### Visualization
- **Matplotlib**: Static visualizations
- **Seaborn**: Statistical data visualization
- **Plotly**: Interactive charts and graphs

### Data Sources
- **Ergast API**: Historical F1 data
- **FastF1 API**: Telemetry and timing data
- **Official F1 API**: Live timing and race data

## 🚀 Getting Started

### Prerequisites

```bash
Python 3.8 or higher
pip package manager
```

### Installation

1. Clone the repository:
```bash
git clone https://github.com/anamika-sg52/anamika-sg52.git
cd anamika-sg52
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Set up data sources:
```bash
python setup_data.py
```

### Usage

#### Basic Prediction
```python
from f1_predictor import RacePredictor

# Initialize predictor
predictor = RacePredictor()

# Load historical data
predictor.load_data(seasons=['2020', '2021', '2022', '2023'])

# Train model
predictor.train()

# Make prediction for next race
prediction = predictor.predict_race(circuit='Monaco', year=2024)
print(prediction)
```

#### Visualize Historical Performance
```python
from f1_analytics import DriverAnalytics

analytics = DriverAnalytics()
analytics.plot_driver_performance('Max Verstappen', seasons=5)
analytics.plot_constructor_comparison(['Red Bull', 'Mercedes', 'Ferrari'])
```

## 📊 Model Architecture

### Features Used
- **Driver Features**: Historical performance, qualifying positions, DNF rate, points scored
- **Constructor Features**: Team performance, reliability metrics, development rate
- **Track Features**: Circuit type (street/permanent), lap length, number of corners, DRS zones
- **Weather Features**: Temperature, rainfall probability, wind speed
- **Strategic Features**: Tire compound selection, pit stop strategies

### Algorithms Implemented
1. **Random Forest Classifier**: For categorical predictions (winner, podium)
2. **Gradient Boosting Regressor**: For continuous predictions (lap times, points)
3. **Neural Networks**: For complex pattern recognition (optional)
4. **Ensemble Methods**: Combining multiple models for better accuracy

## 📈 Model Performance

- **Race Winner Accuracy**: ~65-70%
- **Podium Prediction Accuracy**: ~55-60%
- **Top 10 Prediction Accuracy**: ~75-80%
- **Fastest Lap Prediction**: ~50-55%

*Note: F1 races have inherent unpredictability due to crashes, mechanical failures, and weather changes.*

## 📁 Project Structure

```
f1-prediction/
├── data/
│   ├── raw/                    # Raw data from APIs
│   ├── processed/              # Cleaned and processed data
│   └── models/                 # Saved trained models
├── notebooks/
│   ├── exploratory_analysis.ipynb
│   ├── feature_engineering.ipynb
│   └── model_training.ipynb
├── src/
│   ├── data_collection.py      # API data fetching
│   ├── preprocessing.py        # Data cleaning
│   ├── features.py             # Feature engineering
│   ├── models.py               # ML models
│   └── prediction.py           # Prediction pipeline
├── tests/
│   └── test_models.py          # Unit tests
├── requirements.txt
└── README.md
```

## 🎯 Future Enhancements

- [ ] Real-time prediction during race weekends
- [ ] Integration with live timing data
- [ ] Weather impact analysis improvements
- [ ] Driver rivalry and team dynamics modeling
- [ ] Mobile app for predictions
- [ ] Betting odds comparison
- [ ] Social media sentiment analysis

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👏 Acknowledgments

- **Ergast API** for providing comprehensive F1 historical data
- **FastF1** library for telemetry data access
- F1 community for insights and feedback
- All contributors who have helped improve this project

## 📞 Contact

**Anamika** - [@anamika-sg52](https://github.com/anamika-sg52)

Project Link: [https://github.com/anamika-sg52/anamika-sg52](https://github.com/anamika-sg52/anamika-sg52)

---

⚡ Made with passion for Formula 1 and Data Science! 🏁
