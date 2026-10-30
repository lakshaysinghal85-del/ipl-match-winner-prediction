# 🏏 IPL Match Winner Prediction System

IPL Match Winner Prediction System is a machine learning-based web application developed to predict the possible winner of an Indian Premier League (IPL) cricket match. It combines a React.js frontend with a Python Flask backend to provide an interactive platform for entering match details and generating predictions using a trained machine learning model.

The application allows users to select participating teams, toss winner, toss decision, and other match-related details to predict the likely winning team. The trained machine learning model processes the selected inputs and generates a prediction through the backend API.

## 🎯 Objectives

- Develop a machine learning-based system for predicting IPL match outcomes.
- Analyze historical IPL match data to identify patterns and trends.
- Apply machine learning techniques to predict possible match winners.
- Provide an interactive web interface for entering match information.
- Integrate the React.js frontend with a Python Flask backend.
- Process match-related information using Pandas and NumPy.
- Display prediction results in a simple and understandable format.
- Demonstrate the practical application of machine learning in sports analytics.

## ✨ Features

- **Team Selection:** Select the participating IPL teams for a particular match.
- **Toss Winner Selection:** Choose the team that won the toss.
- **Toss Decision:** Select whether the toss winner decided to bat or field.
- **Match Information:** Enter relevant match details required by the prediction model.
- **Winner Prediction:** Predict the possible match winner using the trained machine learning model.
- **Machine Learning Integration:** Uses a pre-trained model stored in `iplwinner.pkl` to generate predictions.
- **Interactive Frontend:** Provides a React.js-based interface for entering match details and viewing results.
- **Flask REST API:** Handles prediction requests and communicates with the machine learning model.
- **Google Authentication:** Integrates Google OAuth for user authentication.
- **Team Mapping:** Uses predefined team codes to process team selections consistently.
- **Real-Time Prediction Response:** Sends user inputs to the backend and displays the generated prediction.

## 🛠️ Technologies Used

| Technology | Purpose |
| ---------- | ------- |
| Python | Backend programming and machine learning implementation |
| Flask | Building backend server and REST API endpoints |
| React.js | Developing the interactive frontend |
| JavaScript | Frontend application logic and API communication |
| Pandas | Data manipulation and preprocessing |
| NumPy | Numerical operations and data processing |
| Joblib | Loading the trained machine learning model |
| Scikit-learn | Machine learning model development and prediction (if used during training) |
| Google OAuth | User authentication |
| Flask-CORS | Enabling cross-origin communication |
| HTML5 | Web page structure |
| CSS3 | Frontend styling and layout |
| npm | Frontend package and dependency management |

## 🏗️ System Architecture

The application follows a client-server architecture with machine learning integration.

- **Frontend Layer:** Uses React.js to provide an interactive interface for selecting teams and entering match details.
- **Input Processing Layer:** Collects and organizes match information before sending it to the backend.
- **API Layer:** Uses Flask REST API endpoints to receive prediction requests from the frontend.
- **Data Processing Layer:** Uses Pandas and NumPy to process and prepare input data.
- **Machine Learning Layer:** Loads the trained model from `iplwinner.pkl` and generates match predictions.
- **Authentication Layer:** Integrates Google OAuth for user authentication.
- **Prediction Output Layer:** Sends the predicted winning team back to the React frontend for display.

## ⚙️ Core Operations

The system performs the following important operations:

### 1. Team Selection

- Select the first participating team.
- Select the opposing team.
- Map the selected teams to their corresponding predefined team codes.
- Validate the selected teams before prediction.

### 2. Toss Information

- Select the toss-winning team.
- Select the toss decision.
- Process the toss information as an input to the prediction model.

### 3. Match Data Processing

- Collect the selected match information.
- Convert categorical inputs into the required model format.
- Prepare the input data for machine learning prediction.
- Pass the processed data to the trained model.

### 4. Machine Learning Prediction

1. The user enters the match details through the React interface.
2. The frontend sends the information to the Flask backend.
3. The backend receives and validates the input data.
4. The trained model (`iplwinner.pkl`) is loaded using Joblib.
5. The model processes the input features.
6. The predicted winner is generated.
7. The prediction result is returned to the frontend.
8. The frontend displays the predicted winning team.

### 5. User Authentication

- Provide Google-based login functionality.
- Authenticate users through Google OAuth.
- Verify authentication information through the backend.

## 🔌 API Endpoints

The Flask backend provides API endpoints for handling prediction requests and authentication.

| Module | HTTP Method | Endpoint | Operation |
| ------ | ----------- | -------- | --------- |
| Prediction | POST | `/predict` | Generate IPL match winner prediction |
| Authentication | POST | Google OAuth verification endpoint | Verify Google authentication token |

*Note: Update the authentication endpoint according to the actual route implemented in your Flask backend.*

## 🤖 Machine Learning Model

The application uses a pre-trained machine learning model to predict IPL match outcomes.

- **Model File:** `iplwinner.pkl`
- **Model Loading:** Joblib
- **Input Features:** Participating teams, toss winner, toss decision, and other configured match features.
- **Prediction:** Generates the predicted winning team based on the input features.

The model is integrated with the Flask backend, allowing predictions to be generated through API requests from the React frontend.

## 🚀 Setup and Installation

### Prerequisites

- Python 3.11 or compatible version
- Node.js and npm
- Visual Studio Code
- Git
- Required Python packages
- Google OAuth credentials (if authentication is enabled)

### 1. Clone the Repository

```bash
git clone <your-github-repository-url>
```

### 2. Backend Setup

Navigate to the backend directory:

```bash
cd backend
```

Create and activate a virtual environment:

```bash
python -m venv venv
```

Windows:

```bash
venv\Scripts\activate
```

Install the required dependencies:

```bash
pip install flask flask-cors joblib numpy pandas
```

Start the Flask backend:

```bash
python app.py
```

The backend will run at:

`http://localhost:5000`

### 3. Frontend Setup

Open another terminal and navigate to the React application directory:

```bash
cd ipl-prediction-app
```

Install frontend dependencies:

```bash
npm install
```

Start the React development server:

```bash
npm start
```

*If your project uses Vite, use `npm run dev` instead.*

The frontend will run at the development URL displayed in your terminal.

## 📁 Project Structure

```text
IPL-Match-Winner-Prediction/
│
├── backend/
│   ├── app.py
│   ├── iplwinner.pkl
│   └── requirements.txt
│
├── ipl-prediction-app/
│   ├── public/
│   ├── src/
│   │   ├── App.js
│   │   ├── components/
│   │   └── ...
│   ├── package.json
│   └── package-lock.json
│
├── .gitignore
└── README.md
```

*The structure is illustrative. Update the filenames and folders according to your actual repository.*

## 🔮 Future Scope

- Improve prediction accuracy using additional historical IPL data.
- Experiment with different machine learning algorithms.
- Include venue-based match analysis.
- Add detailed team performance statistics.
- Display historical head-to-head records between teams.
- Introduce player performance analysis.
- Add graphical representation of prediction probabilities.
- Develop a match history section to store previous predictions.
- Integrate live IPL match information.
- Improve the user interface with additional analytics and visualizations.

## 🎓 Project Information

**Project Name:** IPL Match Winner Prediction System  
**Student:** Lakshay  
---

**IPL Match Winner Prediction System — Applying Machine Learning to Cricket Analytics and Predicting Match Outcomes.**