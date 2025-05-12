# 🏠 Bengaluru House Price Prediction

A machine learning web application that predicts house prices in Bengaluru based on user input such as location, square footage, number of bedrooms, and bathrooms. This project uses a regression model built with Python and is deployed with a web interface using HTML, CSS, and JavaScript.

---

## 📁 Project Structure

```
.
├── Model
│   └── bengaluru_house_price_prediction.ipynb   # Jupyter notebook for model training
│
├── Server
│   ├── server.py                                # Flask server to handle API requests
│   ├── util.py                                  # Utility functions to load model and handle predictions
│   ├── columns.json                             # Contains the list of input features
│   └── house_price_model.pkl                    # Trained ML model serialized with pickle
│
├── Client
│   ├── app.html                                 # Frontend HTML page
│   ├── app.css                                  # Styling for the frontend
│   └── app.js                                   # JavaScript to interact with backend API
```

---

## ⚙️ How to Run the Project Locally

### 1. Clone the repository

```bash
git clone https://github.com/your-username/bengaluru-house-price-prediction.git
cd bengaluru-house-price-prediction
```

### 2. Set up a virtual environment (optional but recommended)

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install dependencies

Navigate to the Server folder and install the necessary packages:

```bash
cd Server
pip install -r requirements.txt
```

If `requirements.txt` is not present, install manually:

```bash
pip install flask pandas scikit-learn numpy
```

### 4. Run the Flask server

```bash
python server.py
```

The server will start at: [http://127.0.0.1:5000/](http://127.0.0.1:5000/)

### 5. Open the client interface

Open the `app.html` file from the `Client` folder in your browser. It will communicate with the server API to provide predictions.

---

## 📊 Model Details

- **Type**: Regression Model  
- **Algorithm**: Linear Regression (or whichever you used)  
- **Input Features**: Location, Total Square Feet, Number of Bedrooms (BHK), Number of Bathrooms  
- **Output**: Predicted house price (in Lakhs)

---

## 🚀 Future Improvements

- Deploy the app using Heroku / Render / AWS  
- Add more model options (Random Forest, XGBoost, etc.)  
- Improve UI/UX  
- Add error handling and input validation  

---

## 📌 Acknowledgements

- Dataset from [Kaggle](https://www.kaggle.com/)  
- Inspired by tutorials from [Codebasics](https://www.youtube.com/c/codebasics)

---

## 📬 Contact

For questions or suggestions, reach out via [your-email@example.com] or open an issue.