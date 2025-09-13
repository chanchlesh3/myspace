# Event Log App

A simple **Flask-based web application** to record and manage events.  
Each event is stored with:  
- **Event ID**  
- **Event Description**  
- **Timestamp (date & time automatically recorded)**  

---

## 🚀 Features
- Add new events with a unique Event ID.  
- Automatically logs the current date and time.  
- View a list of all logged events.  
- Lightweight and easy to set up.  

---

## 🛠️ Installation & Setup

```bash
# Clone the repository
git clone https://github.com/your-username/event-log-app.git
cd event-log-app

# Create and activate virtual environment
python -m venv venv
# On Linux/Mac
source venv/bin/activate
# On Windows
venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the app
python app.py
