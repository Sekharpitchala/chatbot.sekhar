# 🛍️  Price Negotiation chatbot with  text and voice on E-commerce web site.
 💬🛒 An AI-powered chatbot that lets uAn AI-powered chatbot that lets users negotiate product prices on an e-commerce site using text and voice commands. Built with Flask, machine learning models, and voice interaction features, it creates a more human-like shopping experience.This Flask-based web application allows users to browse products, negotiate prices with a chatbot (via text or voice), and complete purchases. It also provides user authentication, order management, and sentiment-based product review analysis.

## 🚀 Features

### 🔐 User Authentication
- Signup and login functionality for secure access.

### 🛒 Browse Products
- View the list of available e-commerce products.

### 💬 Price Negotiation
- Negotiate prices with an AI-powered chatbot:
  - **Text-based negotiation**
  - **Voice-based negotiation**

### 📦 Order Management
- Complete purchases and view past order history.

### ✍️ Review System
- Post reviews for purchased products.
- Sentiment analysis using **VADER** (Positive, Negative, Neutral).



## 🛠️ Technologies Used

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Python, Flask
- **Database**: MySQL (MariaDB)
- **ML Libraries**: Scikit-learn, TensorFlow, Pandas, NumPy
- **Voice & NLP**: SpeechRecognition, VADER Sentiment Analysis
- **Others**: Matplotlib, PyAudio


## 💻 Installation

### 1. Clone the Repository:

git clone https://github.com/your-username/ecommerce-negotiate.git
cd ecommerce-negotiate

## 2. Create a Virtual Environment:

python -m venv venv
source venv/bin/activate       # For Windows: venv\Scripts\activate

## 3. Install Required Packages:

pip install -r requirements.txt

## 4. Set Up the Database:
Open your MySQL terminal and run the following:

CREATE DATABASE negotiate;
USE negotiate;

-- Users table
CREATE TABLE users (
    username VARCHAR(50) PRIMARY KEY,
    password VARCHAR(50),
    contact_no VARCHAR(15),
    emailid VARCHAR(50),
    address VARCHAR(100),
    gender VARCHAR(10)
);

-- Purchase order table
CREATE TABLE purchaseorder (
    username VARCHAR(50),
    product_id VARCHAR(50),
    product_name VARCHAR(100),
    amount FLOAT,
    transaction_date DATETIME
);

-- Reviews table
CREATE TABLE reviews (
    username VARCHAR(50),
    review TEXT,
    sentiment VARCHAR(10)
);

## 5. Add Dataset Files:

Place the following files inside the Dataset/ directory:
ecommerce.csv
model.csv
Make sure they are formatted correctly for product and price data.

## 6. Run the Application:
python app.py
## The application will be available at :  http://127.0.0.1:5000/index

## 📋 Usage Instructions :

 1 Register/Login to access the application.
 2 Browse Products and view available items.
 3 Use Text or Voice Chatbot to negotiate prices.
     Use keywords like first price and final price during negotiation.
 4 Purchase products and view orders in View Orders section.
 5 Post Reviews and view their sentiment prediction.

## 👨‍💻 Contributing
Interested in contributing? Fork the repo and submit a pull request with:
    1 Clear commit messages
    2 Brief description of your changes

## 📜 License
This project is licensed under the BVCEC.EDU.IN License.

## 📬 Contact
Developer: Pitchala Sekhar
Email: sekharpitchala2003@gmail.com
