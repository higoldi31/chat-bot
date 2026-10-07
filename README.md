# 🤖 Machine Learning Chatbot

A simple **Machine Learning-based chatbot** built with Python, NLP, Scikit-learn, and Streamlit. The chatbot understands user queries by classifying them into predefined intents and returns an appropriate response.

The project demonstrates a complete beginner-friendly NLP workflow — from text preprocessing and feature extraction to model training and deployment through a Streamlit web interface.

## 🚀 Live Demo

👉 **[Try the Chatbot Live](https://chatbot-goldi-kumari.streamlit.app/)**

> Replace `YOUR_LIVE_LINK_HERE` with your deployed Streamlit application URL.

## 📌 Features

* 💬 Interactive chatbot interface
* 🧠 Machine Learning-based intent classification
* 🔤 NLP text preprocessing
* 📊 TF-IDF text vectorization
* 🤖 Logistic Regression classification
* 🎯 Confidence-based response handling
* 💾 Pre-trained model and vectorizer stored using Pickle
* 🗨️ Chat history maintained using Streamlit session state
* 🧹 Clear chat functionality
* 📚 Dataset containing predefined questions, intents, and responses
* 🌐 Streamlit web interface

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **NLTK**
* **Scikit-learn**
* **Streamlit**
* **Pickle**
* **TF-IDF**
* **Logistic Regression**

## 🧠 How It Works

The chatbot follows a simple NLP and Machine Learning pipeline:

```text
User Input
    ↓
Text Cleaning
    ↓
Tokenization
    ↓
Stopword Removal
    ↓
Stemming
    ↓
TF-IDF Vectorization
    ↓
Logistic Regression Model
    ↓
Intent Prediction
    ↓
Response Selection
    ↓
Chatbot Response
```

### 1. Text Preprocessing

The user's input is processed using NLTK:

* Converts text to lowercase
* Removes punctuation
* Tokenizes the sentence
* Removes English stopwords
* Applies Porter Stemming

### 2. TF-IDF Vectorization

The cleaned text is converted into numerical features using **TF-IDF (Term Frequency–Inverse Document Frequency)**.

### 3. Intent Classification

A **Logistic Regression** model is trained to classify user queries into predefined intents.

The dataset contains **63 examples** across multiple intents, including:

* Greeting
* Goodbye
* Python
* Machine Learning
* Artificial Intelligence
* Thanks

### 4. Response Generation

After predicting the intent, the application retrieves the corresponding response from the dataset.

A confidence threshold is also used. If the model is less than **40% confident**, the chatbot provides a fallback response instead of returning an uncertain answer.

## 📊 Model Performance

The Logistic Regression model achieved:

**Accuracy: 92.31%**

The model was trained using an **80/20 train-test split**.

```text
Training Data → 80%
Testing Data  → 20%

Accuracy → 92.31%
```

## 📂 Project Structure

```text
chat-bot/
│
├── app.py                  # Streamlit chatbot application
├── chatbot.ipynb           # Model development and training notebook
├── chatbot.csv             # Dataset containing questions, intents and responses
├── chatbot_model.pkl       # Trained Logistic Regression model
├── vectorizer.pkl          # Trained TF-IDF vectorizer
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
```

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/higoldi31/chat-bot.git
```

### 2. Navigate to the Project Directory

```bash
cd chat-bot
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

Activate the environment:

**Windows:**

```bash
venv\Scripts\activate
```

**macOS/Linux:**

```bash
source venv/bin/activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Run the Application

```bash
streamlit run app.py
```

The application will open in your browser.

## 💬 Example Conversations

### Example 1

```text
You: Hello

Bot: Hello! How can I help you?
```

### Example 2

```text
You: How can I learn ML?

Bot: Machine Learning allows computers to learn patterns from data.
```

### Example 3

```text
You: Bye

Bot: Goodbye!
```

## 📓 Model Training

The complete model development process is available in:

**`chatbot.ipynb`**

The notebook covers:

1. Dataset loading
2. Data exploration
3. Data validation
4. Text preprocessing
5. TF-IDF feature extraction
6. Train-test split
7. Logistic Regression training
8. Model evaluation
9. Model serialization
10. Testing the chatbot

## 📦 Dataset

The chatbot uses `chatbot.csv`, which contains three main columns:

| Column     | Description                      |
| ---------- | -------------------------------- |
| `text`     | User's input/question            |
| `intent`   | Intent associated with the input |
| `response` | Response returned by the chatbot |

## 🌐 Deployment

The application can be deployed using **Streamlit Community Cloud**.

Required deployment configuration:

```text
Main file: app.py
```

Make sure the following files are included in the repository:

```text
app.py
chatbot.csv
chatbot_model.pkl
vectorizer.pkl
requirements.txt
```

## 🔮 Future Improvements

Some possible improvements for this project:

* Add more training data and intents
* Improve model accuracy with a larger dataset
* Add more advanced NLP techniques
* Experiment with other classification algorithms
* Add conversation context and memory
* Integrate a generative AI model
* Add voice input and text-to-speech
* Improve the UI/UX
* Add authentication and user profiles
* Deploy the chatbot as a production-ready application

## 🎯 Learning Outcomes

Through this project, I explored:

* Natural Language Processing
* Text preprocessing
* Tokenization and stemming
* TF-IDF feature extraction
* Supervised Machine Learning
* Logistic Regression
* Model evaluation
* Model serialization using Pickle
* Streamlit application development
* Building and deploying an interactive ML application

## 👩‍💻 Author

**Goldi Kumari**

B.Tech Computer Science Engineering

GitHub: **[@higoldi31](https://github.com/higoldi31)**

---
