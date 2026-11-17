# 💧 Water Drinking Reminder

## 📌 Project Description
Water Drinking Reminder is a simple Python project that reminds users to drink water at regular intervals.

The program sends desktop notifications using the `plyer` library. It helps users maintain a regular water-drinking habit.

## 🚀 Features
- Sends desktop notifications automatically.
- Reminds users to drink water at regular intervals.
- Customizable reminder interval.
- Simple and beginner-friendly Python project.

## 🛠️ Technologies Used
- Python
- Time Module
- Plyer Library

## 📂 Project Structure

```text
project_py_7/
│
├── main.py
└── README.md
```

## ⚙️ Installation

**Step 1: Install Python**

Make sure Python is installed on your system.

**Step 2: Install Required Library**

Open your terminal and run:

```bash
python -m pip install plyer
```

**Step 3: Clone or Download the Project**

Download the project and open its folder in VS Code.

## ▶️ How to Run

Run the following command in the terminal:

```bash
python main.py
```

The reminder will start running and display a desktop notification every 30 minutes.

## 💻 Code Example

```python
import time
from plyer import notification

def water_reminder(interval_minutes):
    interval_seconds = interval_minutes * 60

    print("Water Drinking Reminder Started")
    print(f"You will get a notification every {interval_minutes} minutes\n")

    while True:
        time.sleep(interval_seconds)

        notification.notify(
            title="Drink Water",
            message="Time to drink water and stay hydrated.",
            timeout=10
        )

water_reminder(30)
```

## ⏰ Customize Reminder Time

You can change the reminder interval by modifying:

```python
water_reminder(30)
```

Examples:

- `water_reminder(5)` – Every 5 minutes.
- `water_reminder(15)` – Every 15 minutes.
- `water_reminder(30)` – Every 30 minutes.
- `water_reminder(60)` – Every 60 minutes.

## 📚 Python Concepts Used
- Functions
- Variables
- Loops (`while`)
- Time module
- External Python libraries
- Desktop notifications

## 👨‍💻 Author
**Aman Kushwaha**

## 📄 License
This project is created for educational and learning purposes.