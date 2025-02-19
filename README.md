# 🚀 Space Management System Database  

## 📌 Overview  
The **Space Management System** database is designed to efficiently manage 🚀 spacecraft, 🛰️ missions, 🌌 space stations, and astronaut assignments.  

---

## 🛠️ Technologies Used  
- 🐘 **PostgreSQL** (Database)  
- 📜 **SQL Queries** (Schema & Data Management)  

---

## 📂 Database Schema  
The database consists of the following tables:  

1️⃣ **🚀 Spaceships** – Stores information about spacecraft.  
2️⃣ **🛰️ Missions** – Details of space missions.  
3️⃣ **👨‍🚀 Astronauts** – Information about astronauts.  
4️⃣ **🏢 Space Stations** – Data about space stations.  
5️⃣ **🔗 Assignments** – Links astronauts to missions.  

---

## ⚙️ Setup Instructions  
Follow these steps to set up the database:  

1️⃣ **Clone the repository**  
   ```bash
   git clone https://github.com/your-repo/space-management-db.git
   cd space-management-db
   ```  
   
2️⃣ **Install PostgreSQL** (if not installed)  
   
3️⃣ **Create the Database**  
   ```sql
   CREATE DATABASE space_management;
   ```  

4️⃣ **Run Schema File**  
   ```bash
   psql -d space_management -f schema.sql
   ```  

5️⃣ **Insert Sample Data (Optional)**  
   ```bash
   psql -d space_management -f seed.sql
   ```  

---

## 📌 Example Queries  
Here are some example queries you can run:  

✅ **Get all astronauts assigned to a mission**  
   ```sql
   SELECT a.name FROM Astronauts a 
   JOIN Assignments asg ON a.id = asg.astronaut_id 
   WHERE asg.mission_id = 1;
   ```  

✅ **List all active missions**  
   ```sql
   SELECT * FROM Missions WHERE status = 'Active';
   ```  

✅ **Find spaceships launched after 2020**  
   ```sql
   SELECT * FROM Spaceships WHERE launch_year > 2020;
   ```  

---

## 🤝 Contribution Guidelines  
Want to contribute? Follow these steps:  

🔹 **Fork the repository**  
🔹 **Create a new branch** (`git checkout -b feature-name`)  
🔹 **Commit your changes** (`git commit -m "Added a new feature"`)  
🔹 **Push and create a pull request**  

---

## 📧 Contact  
For any queries, feel free to reach out:  

📩 Email:hifzaofpk@gmail.com 
🌐 GitHub: [Hifza-Khalid](https://github.com/Hifza-Khalid)  

