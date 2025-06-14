# 🚀 Secure Login System Simulation (Java + Swing + BCrypt)

## 📌 Project Overview
This is a simple **Java GUI-based Secure Login System Simulation** designed to demonstrate secure login practices. It includes password hashing, basic input validation, and a login attempt limiter. The goal is to simulate a secure login mechanism suitable for academic or demo purposes.

---

## 🔧 Features Implemented
- ✅ **Email + Password Login GUI** (using Java Swing)
- ✅ **Password Hashing** using `BCrypt` (via `jbcrypt-0.4.jar`)
- ✅ **Basic Input Validation** (email format, empty fields)
- ✅ **Login Attempt Limiter** (locks out after 3 failed attempts)
- 🚧 *Optional features like 2FA mock can be added easily*

---

## 🛠️ Technologies & Tools Used

| Tool/Library      | Purpose                                      |
|-------------------|----------------------------------------------|
| Java (JDK 8+)     | Core programming and GUI development         |
| Java Swing        | GUI components for login window              |
| jBCrypt (0.4)     | Secure password hashing & validation         |
| HashMap           | Simulated in-memory user database            |

---

## 🧠 Project Structure

```
SecureLoginSystem/
├── SecureLogin.java        # Main GUI and login logic
├── UserDatabase.java       # Simulated user data with hashed passwords
├── PasswordUtil.java       # Utility for hashing and verifying passwords
├── jbcrypt-0.4.jar         # External BCrypt library (required)
└── README.md               # Documentation and setup instructions
```

---

## 📥 How to Run

### ✅ Prerequisites:
- Java JDK 8+ installed
- Download `jbcrypt-0.4.jar` from [Maven Repo](https://mvnrepository.com/artifact/org.mindrot/jbcrypt/0.4)

### 💻 Compile:

**Windows:**
```bash
javac -cp .;jbcrypt-0.4.jar SecureLogin.java UserDatabase.java PasswordUtil.java
```

**Linux/macOS:**
```bash
javac -cp .:jbcrypt-0.4.jar SecureLogin.java UserDatabase.java PasswordUtil.java
```

### ▶️ Run:

**Windows:**
```bash
java -cp .;jbcrypt-0.4.jar SecureLogin
```

**Linux/macOS:**
```bash
java -cp .:jbcrypt-0.4.jar SecureLogin
```

---

## 👤 Test User Credentials

Use the following test credentials to login:

- **Email:** `user@example.com`
- **Password:** `password123`

---

## 🔐 Security Highlights

- Passwords are never stored in plain text.
- Hashing is done using a secure one-way algorithm (BCrypt).
- Input validation is performed before login checks.
- Login is blocked after 3 incorrect attempts.

---

## 📌 Future Improvements

- 2FA with OTP simulation
- Integration with real database (e.g., SQLite or MySQL)
- Account registration interface
- Password recovery system
