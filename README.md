# Medical Appointment System

## 📌 Overview
The **Medical Appointment System** is a project designed to manage and schedule medical appointments efficiently. This system helps patients book appointments, doctors manage schedules, and administrators oversee the appointment process.

# Dataset Description: 
A person makes a doctor appointment, receives all the instructions and no-show. Who to blame?
This dataset collects information from 100k medical appointments in Brazil and is focused on the question of whether or not patients show up for their appointment. A number of characteristics about the patient are included in each row.

# Data Wrangling:
Our data can be found on `noshowappointments-kagglev2-may-2016.csv` file provided on this repository, downloaded from [Kaggle](https://www.kaggle.com/datasets/joniarroba/noshowappointments). 

## 🔧 Features
- Patient registration and login system
- Appointment booking and cancellation
- Doctor availability management
- Notification system for appointment reminders
- Data visualization for appointment trends

## 📂 Project Structure

📁 medical_appointment/
├── 📄 main.py            # Main script to run the project

├── 📄 database.sql       # SQL file with database schema

├── 📄 config.py          # Configuration file for database connection

├── 📂 data/              # Sample datasets (if applicable)

├── 📂 templates/         # HTML templates for frontend (if applicable)

├── 📂 static/            # CSS & JS files for UI (if applicable)

├── 📂 scripts/           # Python scripts for automation

└── 📄 README.md          # Project documentation


## 🚀 Installation & Setup
1. **Clone the repository**:
   
   git clone https://github.com/Somakshi1/medical_appointment.git
   cd medical_appointment
   
2. **Create a virtual environment (optional but recommended)**:
   
   python -m venv venv
   source venv/bin/activate  # For Mac/Linux
   venv\Scripts\activate     # For Windows

3. **Install dependencies**:
4. 
   pip install -r requirements.txt

5. **Configure the database connection**:
   - Update `config.py` with your database credentials.
   - Ensure the database server is running.
6. **Run the project**:
  
   python main.py


## 🛠 Technologies Used
- **Python** 🐍
- **SQL (SQLite/MySQL/PostgreSQL)** 🗄️
- **Flask/Django (if applicable)** 🌍
- **HTML, CSS, JavaScript** 🎨
- **Pandas & Matplotlib** 📊

## 📖 Usage
- Patients can register and book appointments.
- Doctors can manage their schedules.
- Admins can oversee and analyze appointment data.


These are derived conclusions after completing our data visualisation phase.

# Q1: How often do men go to hospitals compared to women? Which of them is more likely to show up?
- Nearly half of our dataset conists of women with wider age destribution and some outliers, all of which achiees a rate higher than men.
- It is obvious that 79.8% of our patients did show up on their appointments and only 20.1% of them did not.
- Women do show up on their appointments more often than men do, but this may b affected by the percentage of women on this dataset.

# Q2: Does recieving an SMS as a reminder affect whether or not a patient may show up? is it correlated with number of days before the appointment?
- 67.8% of our patients did not reciee any SMS reminder of their appointments, yet they showed up on their appointments.
- It is clear that there is a positive correlation between number of due days and whether a patient shows up or not.
- Patient with appointments from 0 to 30 days tend to show up more regularly, while patients with higher number of days tend to not show up.
- gender does not affect number of due days and showing up at an appointment that much.

# Q3: Does having a scholarship affects showing up on a hospital appointment? What are the age groups affected by this?
- Having a scholarship does not affect showing up to a doctor appointment that much.
- Huge age group is enrolled to that scholarship and also enrol their babies on.
- 
# Q4: Does having certain deseases affect whather or not a patient may show up to their appointment? is it affected by gender?
- We can conclude that the vast majority of our dataset does not have chronic deseases, yet, they are existed in so many young people.
- Having a chronic deseas may affect your showing up at a hospital's appointment.

# Built with:		
- JupyterLab	
- Python3	   	
- Pandas		
- Numpy			
- Matplotlib	
- Seaborn		
