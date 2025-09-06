# IPL Win Predictor

A machine learning-powered web application to predict the win probability of teams in Indian Premier League (IPL) cricket matches. Built with Streamlit, this project leverages historical IPL data and advanced modeling to provide real-time match outcome probabilities.

## Features

- Predict win probabilities for IPL teams based on match context
- User-friendly web interface built with Streamlit
- Select teams, city, target, score, overs, and wickets
- Visual probability output for both batting and bowling teams
- Uses real IPL match data for training and predictions

## How It Works

1. **Input Match Details:** Select batting and bowling teams, host city, target score, current score, overs completed, and wickets fallen.
2. **Model Prediction:** The app calculates match context features and uses a trained machine learning model to predict win/loss probabilities.
3. **Result Display:** Probabilities for both teams are displayed in a clear, easy-to-understand format.

## Tech Stack

- **Frontend:** Streamlit
- **Backend:** Python, scikit-learn
- **Data:** IPL match and delivery datasets (`matches.csv`, `deliveries.csv`)
- **Deployment:** Heroku (Procfile and setup.sh included)

## Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/Ankit0102/Ipl-Win-Predictor.git
   cd Ipl-Win-Predictor
   ```

2. **Install dependencies:**
   ```sh
   pip install -r requirements.txt
   ```

3. **Run the app locally:**
   ```sh
   streamlit run app.py
   ```

## Usage

- Open the app in your browser.
- Select match parameters.
- Click "Predict Probability" to view win chances for both teams.

## Project Structure

```
├── app.py                # Streamlit app source code
├── matches.csv           # IPL match data
├── deliveries.csv        # IPL ball-by-ball data
├── requirements.txt      # Python dependencies
├── Procfile              # Heroku deployment file
├── setup.sh              # Heroku setup script
├── README.md             # Project documentation
```

## Model

- Trained using IPL historical data
- Features include team, city, runs left, balls left, wickets, current run rate, required run rate, etc.
- Model file (`pipe.pkl`) required for predictions (not included in repo for size/privacy)

## Deployment

To deploy on Heroku:
1. Ensure `Procfile` and `setup.sh` are present.
2. Push to Heroku Git remote.
3. App will be available at your Heroku URL.

## Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements.

## License

This project is licensed under the MIT License.

## Author

- [Ankit0102](https://github.com/Ankit0102)
