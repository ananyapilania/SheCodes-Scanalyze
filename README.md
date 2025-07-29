# 🧠 Scanalyze – Intelligent Disease Diagnosis & Epidemic Alert System

Scanalyze is a Python-based terminal application designed to help users identify possible diseases based on their symptoms, assess medical emergencies like injuries and pregnancy-related issues, and detect region-based epidemic trends. The application leverages both MySQL and SQLite databases to store, retrieve, and analyze categorized disease data.

---

## 🚀 Features

### 🔎 Symptom Scanner

- Matches user-inputted symptoms to disease records across categories:
  - Fever/Cold/Cough
  - Skin Diseases
  - Mental Health
  - Stomach Issues
  - Bone/Joint Disorders
  - Eye Problems
  - Ear/Nose/Throat Conditions

### 👩‍⚕️ Special Case Detection

- Pregnancy-related symptom tracking and alert system
- Injury severity assessment and emergency guidance

### 🌐 Epidemic Scanner

- Reads from a MySQL epidemic tracker table
- Flags diseases with >50 reported cases in specific locations
- Tabulates results using `tabulate` for clean display

### 🗺️ City-Wise Disease Lookup

- Uses a local SQLite database to map symptoms and diseases to major Indian cities
- Includes information on vaccine availability

---

### 🔐 Scalability and Extensibility:
Modular design makes it easy to plug in:

Additional disease categories

More advanced matching logic (e.g., fuzzy matching, symptom weights)

Real-time API integration for live epidemic alerts

Easily extendable to a GUI (Tkinter or web-based) in the future.

## ⚙️ Technologies Used

| Component      | Technology             |
| -------------- | ---------------------- |
| Programming    | Python 3.7+            |
| Primary DB     | MySQL                  |
| Local DB Cache | SQLite                 |
| UI             | Command-Line Interface |
| Tables         | `tabulate` library     |

---

## 📁 Project Structure

```
scanalyze/
├── main.py                 # Main application logic
├── README.md               # Project documentation
├── diseases.db             # SQLite DB for lookup
├── requirements.txt        # Python dependencies
```

---

## 🔧 Installation

To install and run the Scanalyze application, ensure that Python 3.7 or higher is installed on your system, along with a running instance of MySQL Server on localhost. Start by cloning the project repository using `git clone` and navigate into the project directory. It's recommended to create a virtual environment for dependency management. Install the required Python libraries by manually installing `mysql-connector-python` and `tabulate` using pip. Next, open the `main.py` file and update the MySQL connection details with your local username and password. Upon running `python main.py`, the application will automatically create the necessary MySQL database (`CODERED`) and tables, and populate them with sample disease data. The program also sets up a local SQLite database for city-specific disease lookup. Once launched, Scanalyze provides a clean terminal interface for scanning symptoms, checking epidemic alerts, or viewing disease trends.

---

## 📄 Sample Requirements File

```
mysql-connector-python
tabulate
```

---

## 🚪 Disclaimer

Scanalyze is a prototype developed for educational and demonstration purposes only. It is not intended for use as a professional medical diagnostic tool. Users are encouraged to consult healthcare professionals for accurate diagnosis and treatment.

---



