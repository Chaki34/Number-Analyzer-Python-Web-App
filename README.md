# 🔢 Number Analyzer — Python Flask Web App

<p align="center">
  <strong>A simple and interactive Flask-based web application for analyzing numbers.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python" alt="Python">
  <img src="https://img.shields.io/badge/Flask-Web%20Framework-black?style=for-the-badge&logo=flask" alt="Flask">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge" alt="Status">
</p>

---

## 📌 About The Project

**Number Analyzer** is a Python Flask web application that allows users to enter a number and instantly analyze its mathematical properties.

The application checks whether the entered number is:

* 🟢 Even or Odd
* ➕ Positive, Negative, or Zero
* 🔢 Prime or Not Prime
* 🔄 Palindrome or Not
* 💪 Armstrong Number or Not

The project demonstrates how **Python logic can be integrated with a Flask web application** to create an interactive browser-based tool.

---

## ✨ Features

<table>
<tr>
<td>🔢 <strong>Even / Odd</strong></td>
<td>Checks whether a number is even or odd.</td>
</tr>
<tr>
<td>📈 <strong>Positive / Negative</strong></td>
<td>Determines whether the number is positive, negative, or zero.</td>
</tr>
<tr>
<td>🔐 <strong>Prime Number</strong></td>
<td>Checks whether the entered number is a prime number.</td>
</tr>
<tr>
<td>🔄 <strong>Palindrome</strong></td>
<td>Checks whether the number reads the same forwards and backwards.</td>
</tr>
<tr>
<td>💪 <strong>Armstrong Number</strong></td>
<td>Checks whether the number satisfies the Armstrong number property.</td>
</tr>
<tr>
<td>🌐 <strong>Web Interface</strong></td>
<td>Provides a simple browser-based interface using Flask.</td>
</tr>
</table>

---

## 🛠️ Technologies Used

<p>
<img src="https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white" alt="Python">
<img src="https://img.shields.io/badge/Flask-3.x-000000?logo=flask&logoColor=white" alt="Flask">
<img src="https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white" alt="HTML5">
<img src="https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white" alt="CSS3">
</p>

### Core Technologies

* **Python** — Number-analysis logic
* **Flask** — Backend web framework
* **HTML** — Web page structure
* **CSS** — User interface styling
* **Jinja2** — Flask template rendering

---

## 📂 Project Structure

```text
Number-Analyzer-Python-Web-App/
│
├── app.py
│
├── templates/
│   └── index.html
│
├── static/
│   └── style.css
│
├── requirements.txt
│
└── README.md
```

> Your exact structure may differ depending on how you organize your Flask files.

---

## 🚀 Getting Started

Follow these steps to run the project locally.

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Chaki34/Number-Analyzer-Python-Web-App.git
```

### 2️⃣ Navigate Into The Project

```bash
cd Number-Analyzer-Python-Web-App
```

### 3️⃣ Create a Virtual Environment

#### Windows

```bash
python -m venv .venv
```

Activate it:

```bash
.venv\Scripts\activate
```

#### macOS / Linux

```bash
python3 -m venv .venv
```

Activate it:

```bash
source .venv/bin/activate
```

---

### 4️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

If Flask is not included in `requirements.txt`, install it with:

```bash
pip install flask
```

---

### 5️⃣ Run the Flask Application

```bash
python app.py
```

You should see something similar to:

```text
* Serving Flask app 'app'
* Debug mode: off
* Running on http://127.0.0.1:5000
```

---

### 6️⃣ Open The Application

Open your browser and visit:

```text
http://127.0.0.1:5000
```

or:

```text
http://localhost:5000
```

---

## 🔍 How It Works

The application follows a simple request-response flow:

```text
          👤 User
             │
             ▼
      Enter a Number
             │
             ▼
      🌐 Flask Web App
             │
             ▼
      🐍 Python Logic
             │
       ┌─────┼─────┐
       ▼     ▼     ▼
     Even   Prime  Palindrome
       │     │     │
       └─────┼─────┘
             ▼
       Armstrong Check
             │
             ▼
       📊 Analysis Result
             │
             ▼
          👤 User
```

---

## 🧮 Example

Suppose the user enters:

```text
153
```

The application analyzes the number and can return:

```text
Positive: Yes
Even: No
Prime: No
Palindrome: No
Armstrong: Yes
```

### Why is 153 an Armstrong number?

For a 3-digit number:

```text
153 = 1³ + 5³ + 3³
```

```text
153 = 1 + 125 + 27
```

```text
153 = 153
```

Therefore, **153 is an Armstrong number**.

---

## 🌐 Flask Route

The application can be accessed through the Flask server:

```text
GET /
```

The main page provides the interface where users can enter a number and receive its analysis.

---

## 📋 Example Numbers

| Number | Even/Odd | Positive/Negative | Prime | Palindrome | Armstrong |
| -----: | -------- | ----------------- | ----- | ---------- | --------- |
|      2 | Even     | Positive          | ✅     | ❌          | ❌         |
|      7 | Odd      | Positive          | ✅     | ❌          | ❌         |
|    121 | Odd      | Positive          | ❌     | ✅          | ❌         |
|    153 | Odd      | Positive          | ❌     | ❌          | ✅         |
|    -10 | Even     | Negative          | ❌     | ❌          | ❌         |
|      0 | Even     | Zero              | ❌     | ✅*         | ❌         |

> `0` is generally not considered prime. Palindrome handling for `0` depends on the implementation.

---

## 🎯 Learning Objectives

This project is useful for learning:

* 🐍 Python fundamentals
* 🔢 Mathematical programming logic
* 🌐 Flask web development
* 🧩 Routing in Flask
* 📄 HTML templates
* 🎨 CSS styling
* 🔄 Form submission
* 📊 Processing user input
* 🛡️ Basic input validation
* 📁 Flask project structure

---

## 🔮 Future Improvements

Possible future features include:

* [ ] REST API endpoints
* [ ] JSON response support
* [ ] Number history
* [ ] Batch number analysis
* [ ] Prime factorization
* [ ] Fibonacci check
* [ ] Perfect number check
* [ ] Strong number check
* [ ] Perfect square check
* [ ] Better input validation
* [ ] Responsive UI
* [ ] Dark mode
* [ ] Deployment with Gunicorn
* [ ] Docker support

---

## 🧪 Local Development

For development, Flask can be started using:

```bash
python app.py
```

Then open:

```text
http://127.0.0.1:5000
```

Stop the development server with:

```text
CTRL + C
```

---

## 📜 License

This project is available for educational and personal use.

---

## 👨‍💻 Author

<p align="center">
  <strong>Debmalya Chaki</strong>
</p>

<p align="center">
  B.Tech CSE | Python | Java | Spring Boot | Flask
</p>

<p align="center">
  ⭐ If you found this project useful, consider giving the repository a star!
</p>

---

<p align="center">
  <strong>🔢 Analyze Numbers. Learn Python. Build with Flask. 🚀</strong>
</p>
