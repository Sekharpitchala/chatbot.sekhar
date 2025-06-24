# 🛍️ E-commerce Negotiation text and voice commands
 💬🛒 An AI-powered chatbot that lets users negotiate product prices on an e-commerce site using text and voice commands. Built with Flask, Machine Learning models, and voice interaction features for a more human-like shopping experience. An AI-powered chatbot that lets users negotiate product prices on an e-commerce site using text and voice commands. Built with Flask, Machine Learning models, and voice interaction features for a more human-like shopping experience.
💬🛒 An AI-powered chatbot that lets users negotiate product prices on an e-commerce site using text and voice commands. Built with Flask, Machine Learning models, and voice interaction features for a more human-like shopping experience. This is a Flask-based web application that allows users to **browse products**, **negotiate prices** using a chatbot (via **text or voice**), and complete their purchases. It also includes features for **user authentication**, **order management**, and **sentiment-based product review analysis**.

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
```bash
git clone https://github.com/your-username/ecommerce-negotiate.git
cd ecommerce-negotiate
2. Create a Virtual Environment:
bash
Copy
Edit
python -m venv venv
source venv/bin/activate       # For Windows: venv\Scripts\activate
3. Install Required Packages:
bash
Copy
Edit
pip install -r requirements.txt
4. Set Up the Database:
Open your MySQL terminal and run the following:

sql
Copy
Edit
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
5. Add Dataset Files:
Place the following files inside the Dataset/ directory:

ecommerce.csv

model.csv

Make sure they are formatted correctly for product and price data.

6. Run the Application:
bash
Copy
Edit
python app.py
Visit: http://127.0.0.1:5000

📋 Usage Instructions
Register/Login to access the application.

Browse Products and view available items.

Use Text or Voice Chatbot to negotiate prices.

Use keywords like first price and final price during negotiation.

Purchase products and view orders in View Orders section.

Post Reviews and view their sentiment prediction.

👨‍💻 Contributing
Interested in contributing? Fork the repo and submit a pull request with:

Clear commit messages

Brief description of your changes
##📜 License
This project is licensed under the BVCEC.EDU.IN License.

##📬 Contact
Developer:Pitchala Sekhar
Email: sekharpitchala2003@gmail.com
