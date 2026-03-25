# CrossFit Games 2019 Power BI Project

## Description

![CrossFit Games 2019](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e6/2019_CrossFit_Games_Logo.svg/1280px-2019_CrossFit_Games_Logo.svg.png)

This project is a comprehensive Power BI analysis and prediction dashboard for the CrossFit Games 2019. It combines interactive data visualizations in Power BI with a machine learning model for athlete performance prediction, delivered through a Flask web application. The project includes dashboards for coaches and organizers, along with Jupyter notebooks for model training and Power BI project development.

## Features

- **Power BI Dashboards**: Interactive visualizations and reports for CrossFit Games data analysis.
- **Machine Learning Prediction**: Predicts athlete success based on age, weight, height, gender, division, and average points.
- **User Dashboards**: Separate web dashboards for coaches and organizers with tailored interfaces.
- **Data Analysis**: Jupyter notebooks for model training and Power BI project development.
- **REST API**: Endpoints for health checks and predictions.

## Installation

1. Clone the repository:
   ```
   git clone <https://github.com/NOT4TODAY1/CrossFit-Games-2019->
   cd CrossFit-Games-2019--main
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Ensure the trained model file `athlete_model.pkl` is present in the root directory (generated from `model.ipynb`).

## Usage

1. Run the Flask application:
   ```
   python app.py
   ```

2. Open your web browser and navigate to `http://localhost:5000` to access the main dashboard.

3. Use the prediction API by sending POST requests to `/predict` with athlete data in JSON format.

## Demo Credentials

To explore the interface and test the different user roles (Coach and Organizer), demo credentials are available upon request. Please contact the project maintainer via email at **MohamedAziz.TLILI@esprit.tn** with the subject line "CrossFit Games Demo Access" to receive the login details.

## API Endpoints

- `GET /`: Serves the main dashboard HTML page.
- `GET /health`: Health check endpoint to verify API and model status.
- `POST /predict`: Predicts top 10 finishes for an athlete. Requires JSON payload with athlete attributes.

## Technologies Used

- **Data Visualization**: Power BI
- **Backend**: Python, Flask, Flask-CORS
- **Machine Learning**: Scikit-learn, Joblib, Pandas
- **Frontend**: HTML, CSS
- **Data Analysis**: Jupyter Notebooks
- **Data**: Excel files with cleaned athlete and score data

## Project Structure

- `app.py`: Main Flask application
- `index.html`: Main login/dashboard page
- `coach-dashboard.html`: Coach-specific dashboard
- `organisateur-dashboard.html`: Organizer dashboard
- `model.ipynb`: Notebook for training the ML model
- `projet_power_bi.ipynb`: Power BI analysis notebook
- Data files: Excel spreadsheets with athlete data

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License.