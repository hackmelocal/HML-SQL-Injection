# 🔐 Boolean-Based SQL Injection Challenge — hackmelocal.com

Welcome to the **Boolean-Based SQLi** challenge on [hackmelocal.com](https://hackmelocal.com) — a hands-on, real-world-style web security lab where you will learn how to identify and exploit **Boolean-Based SQL Injection** vulnerabilities, even when no direct database errors or messages are shown.

> ⚠️ This challenge is designed **strictly for educational and research purposes** inside the controlled lab environment of `hackmelocal.com`. Any misuse on live systems is **illegal** and **unethical**.

---

## 🎯 Challenge Objective

Your goal is to **detect** and **exploit** a Boolean-Based SQL Injection vulnerability in the provided web app, and extract insights about the backend database — even when no SQL errors are exposed.

### 📌 Key Concepts:
- Boolean-Based (Inferential) SQL Injection
- Logic-based testing using `AND 1=1` and `AND 1=2`
- Manual testing and automation using tools like `ghauri` or `SQLMap`
- Prevention techniques using secure coding practices

---

## ⚙️ How to Run the Challenge

You can run this app in two easy ways:

* ✅ **Option 1:** Run online with GitHub Codespaces  
* ✅ **Option 2:** Run locally with Docker

---

## ☁️ Option 1: Run in GitHub Codespaces (No Installation Needed)

1. Click the green **`Code`** button on the GitHub repository page  
2. Go to the **`Codespaces`** tab  
3. Click **`Create codespace on main`**  
4. Once the Codespace loads, open the terminal with <kbd>Ctrl</kbd> + <kbd>`</kbd>  
5. Start the app:

   ```bash
   docker compose up
````

6. Use the **port preview** link in Codespaces to access the challenge in your browser.

---

## 🖥️ Option 2: Run Locally (Using Docker)

### ✅ Requirements

* [Docker Desktop](https://www.docker.com/products/docker-desktop)
* [Git](https://git-scm.com/downloads)

### 🔧 Steps

1. Clone the repository:

   ```bash
   git clone https://github.com/hackmelocal/HML-base
   cd HML-base
   ```

2. Start the application:

   ```bash
   docker compose up
   ```

3. Open your browser and go to:

   ```
   http://localhost:8000
   ```

> 🧭 **Note:**
>
> * The **main website** runs on **port 8000**
> * The **payment service** runs on **port 8080**

---

## 🔒 How to Prevent This

**Best practices to mitigate SQL Injection:**

* Use **Prepared Statements (Parameterized Queries)**
* Sanitize and validate all user inputs on the server side
* Avoid concatenating SQL with untrusted input
* Use **ORMs** that abstract query building securely
* Implement **least privilege** for database access
* Enable **logging** and monitor for suspicious patterns

---

## 📚 Recommended Reading

* [PayloadsAllTheThings - SQL Injection](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/SQL%20Injection)
* [HackTricks - SQL Injection](https://hacktricks.boitatech.com.br/pentesting-web/sql-injection)
* [PortSwigger Web Security Academy - SQL Injection](https://portswigger.net/web-security/sql-injection)
* [OWASP - SQL Injection](https://owasp.org/www-community/attacks/SQL_Injection)

---

## 🧾 License & Legal

This lab is developed by **hackmelocal.com** for ethical hacking and education only.
Do **not** use this knowledge on systems you don’t own or have permission to test.
