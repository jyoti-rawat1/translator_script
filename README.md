# 🌐 Translator Script (Powered by RapidAPI)

A simple yet powerful **language translator** built in **Python (Jupyter Notebook)** that uses **RapidAPI’s Translation API** to translate text between multiple languages.  
This project demonstrates how to integrate external APIs in Python for Natural Language Processing tasks.

---

## 🚀 Features

- 🌍 Translate text between 100+ languages  
- ⚡ Fast and accurate results using **RapidAPI**  
- 📓 Easy to run in Jupyter Notebook or Google Colab  
- 🔑 Uses secure API key authentication  

---

## 🧰 Technologies Used

- **Python 3**  
- **Jupyter Notebook**  
- **RapidAPI (Google Translate API / Text Translation API)**  
- **Requests** library for API calls  

---

## 🔑 API Integration (via RapidAPI)

This project uses the **Google Translate API** available on **[RapidAPI](https://rapidapi.com/)**.

### 📦 Setup Instructions
1. Go to [RapidAPI](https://rapidapi.com)  
2. Search for **Google Translate API** or **Text Translation API**  
3. Subscribe to the **Free Plan**  
4. Copy your **X-RapidAPI-Key** and **X-RapidAPI-Host**

Example API setup in Python:
```python
import requests

url = "https://google-translate1.p.rapidapi.com/language/translate/v2"

payload = {"q": "Hello, how are you?", "target": "hi", "source": "en"}
headers = {
    "content-type": "application/x-www-form-urlencoded",
    "Accept-Encoding": "application/gzip",
    "X-RapidAPI-Key": "your_api_key_here",
    "X-RapidAPI-Host": "google-translate1.p.rapidapi.com"
}

response = requests.post(url, data=payload, headers=headers)
print(response.json())

#Screenshot

![Translator Output](images/output.jpeg)
