# 🚀 Code Editor Web Application

A **web-based online code editor** with compilation, execution, authentication, and collaborative learning features. This project is designed to help students and developers write, compile, and test code directly in the browser while supporting future scalability for collaboration and learning-focused features.

---

## 📌 Features

### 🔐 User Authentication

* Secure **login system** using PHP and MySQL
* Displays logged-in user information
* Restricts editor access to authenticated users

### 💻 Online Code Editor

* Integrated **CodeMirror editor** for syntax highlighting
* Supports multiple programming languages (C, C++, Java, Python, etc.)
* Clean and responsive UI using HTML & CSS

### ⚙️ Code Compilation & Execution

* Backend powered by **Node.js + Express**
* Uses the `compilex` module to compile and run code
* Handles temporary files securely
* Prevents server crashes using controlled file flushing and `nodemon`

### 🤝 Collaborative Learning & Coding Pages

* Separate pages for:

  * **Collaborative Coding**
  * **Collaborative Learning**
* Accessible after user login
* Designed for future real-time collaboration extensions

### 🗄️ Database Integration

* MySQL database for:

  * User authentication
  * User session management

---

## 🛠️ Tech Stack

### Frontend

* HTML5
* CSS3
* JavaScript
* CodeMirror (via Cloudflare CDN)

### Backend

* Node.js
* Express.js
* PHP (for authentication)
* compilex (code compilation & execution)

### Database

* MySQL

### Tools & Environment

* Visual Studio Code
* Nodemon
* XAMPP / WAMP (for PHP & MySQL)

---

## 📂 Project Structure

```
CodeEditorApp/
│
├── public/
│   ├── IDE.html
│   ├── IDE.css
│   ├── LoginPage.html
│   └── assets/
│
├── server/
│   ├── server.js
│   ├── compile.js
│   └── temp/
│
├── php/
│   ├── login.php
│   └── config.php
│
├── database/
│   └── users.sql
│
└── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/code-editor-app.git
cd code-editor-app
```

### 2️⃣ Backend Setup (Node.js)

```bash
npm install
npm install compilex express nodemon
```

Run the server:

```bash
nodemon server.js
```

### 3️⃣ Database Setup

* Start **MySQL** using XAMPP/WAMP
* Create a database (e.g., `code_editor`)
* Import `users.sql`
* Update database credentials in `config.php`

### 4️⃣ PHP Setup

* Place PHP files inside `htdocs` (XAMPP)
* Ensure Apache & MySQL are running

### 5️⃣ Access the Application

* Login Page: `http://localhost/LoginPage.html`
* Code Editor: `http://localhost/IDE.html`

---

## 🔐 Security Considerations

* Input validation for user credentials
* Controlled execution environment for code compilation
* Temporary file cleanup to prevent memory leaks

---

## 🚧 Future Enhancements

* Real-time collaboration using **WebSockets / Socket.io**
* Live cursor and code sharing
* Chat functionality for collaborative sessions
* User roles (admin / student)
* Code saving & version history
* Online judge style test cases

---

## 🧠 Learning Outcomes

* Full-stack web development
* Client-server architecture
* Secure authentication
* Compiler integration
* Handling real-time execution environments
