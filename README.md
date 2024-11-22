
---

# 🐦 Flappy Bird with Login & Register System  

Welcome to the **Flappy Bird** game with a fully functional **user authentication system**! This project combines the addictive gameplay of Flappy Bird with modern authentication features, all integrated with a **MySQL database**.  

[![GitHub Repo](https://img.shields.io/badge/GitHub-sheelthecoder/Flappy--Bird-blue?style=flat&logo=github)](https://github.com/sheelthecoder/Flappy-Bird)

---

## 🎮 Features  

- **Classic Flappy Bird Gameplay**: Play the timeless game built using **Pygame**.  
- **Login & Registration System**:  
  - **Register**: New users can create accounts with their details.  
  - **Login**: Existing users can log in and start playing.  
- **Database Integration**:  
  - User details are securely stored in a **MySQL database**.  
  - Validation ensures correct credentials during login.  
- **User Interface**: Built using **Tkinter** for registration and login pages.  

---

## 📂 Project Repository  

The full source code for this project can be found here: [Flappy Bird on GitHub](https://github.com/sheelthecoder/Flappy-Bird).  

---

## 🚀 Installation  

### Prerequisites  

1. **Python** (Version 3.8 or later)  
2. **Pip** for installing Python packages.  
3. **MySQL Server** to host the database.  

### Steps to Run  

1. Clone the repository:  
   ```bash
   git clone https://github.com/sheelthecoder/Flappy-Bird.git
   cd Flappy-Bird
   ```  

2. Install required libraries:  
   ```bash
   pip install pygame mysql-connector-python sympy tkinter
   ```  

3. Configure the MySQL database:  
   - Create a database (e.g., `flappy_bird_db`).  
   - Add the required tables:  
     ```sql
     CREATE TABLE login (
         uname VARCHAR(50),
         password VARCHAR(50)
     );

     CREATE TABLE Flappyacc (
         player_id VARCHAR(10),
         player_name VARCHAR(100),
         player_email VARCHAR(100),
         player_contact VARCHAR(15),
         city VARCHAR(50)
     );
     ```  
   - Update the database credentials in the `mysql.connector.connect()` calls in the script.  

4. Run the program:  
   ```bash
   python main.py
   ```  

---

## 🎨 Project Structure  

```
Flappy-Bird/
├── assets/             # Game assets (images, sounds, etc.)
├── main.py             # Main game logic
├── README.md           # Project documentation
├── requirements.txt    # Required Python libraries
└── ... (other Python files for authentication and database)
```  

---

## 🧑‍💻 Technologies Used  

- **Python**  
  - `pygame`: For game mechanics and visuals.  
  - `mysql.connector`: For connecting and interacting with the MySQL database.  
  - `Tkinter`: For building the login and registration UI.  
  - `sympy`: Additional utilities and mathematical functions.  

---

## 🌟 Future Improvements  

- **Leaderboard**: Add a high-score leaderboard.  
- **Enhanced UI**: Improve the design of the login and registration pages.  
- **Session Management**: Keep users logged in during a single session.  

---

## 🤝 Contributing  

Contributions are welcome! Feel free to fork the repository and create a pull request.  

---

