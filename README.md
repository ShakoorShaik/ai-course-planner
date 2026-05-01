# UofT AI Course Planner

<img width="1696" height="979" alt="UofT AI Course Planner dashboard" src="https://github.com/user-attachments/assets/e5cb7ef8-cd53-4327-82c8-a40fb4e4c90d" />

UofT AI Course Planner is a course planning tool designed to help students at the University of Toronto efficiently plan their academic journey. The platform provides interactive features for tracking courses, checking prerequisites, verifying program requirements, and making informed course decisions based on peer ratings and recommendations.

> Built by a team of 5 at the University of Toronto Scarborough. This repository is a personal fork for portfolio display — the primary codebase is maintained at [CREATE-UofT/UTSC-Path-Builder](https://github.com/CREATE-UofT/UTSC-Path-Builder).

---

## Features

<img width="1710" height="980" alt="Course prerequisites view" src="https://github.com/user-attachments/assets/159cfc1d-77f0-40a9-a4f6-f66e89e98744" />

| Feature | Description |
|---|---|
| My Courses | View and manage completed and planned courses |
| Course Prerequisites | Explore prerequisite chains to plan your academic path |
| Program Requirements | Verify degree requirements and graduation status |
| Course Ratings | Browse peer ratings and contribute your own |
| Course Feedback | Share insights to improve recommendations for others |
| Course Recommendations | Get personalized suggestions based on your academic history |

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Backend | Flask (Python) |
| Database | MySQL |

---

## Installation

### Prerequisites

- Python 3.8+
- MySQL running locally or via SSH tunnel
- A `.env` file configured as described below

### Setup

**1. Clone the repository**
```bash
git clone https://github.com/CREATE-UofT/UTSC-Path-Builder.git
cd utsc-path-builder
```

**2. Create and activate a virtual environment**
```bash
python -m venv venv
source venv/bin/activate      # macOS/Linux
venv\Scripts\activate         # Windows
```

**3. Install dependencies**
```bash
pip install -r requirements.txt
```

**4. Configure environment variables**

Create a `.env` file in the project root:
```env
SSH_HOST=your-remote-ssh-server
SSH_PORT=your-ssh-port
SSH_USER=your-ssh-username
SSH_PASSWORD=your-ssh-password

DB_HOST=127.0.0.1
DB_PORT=3306
DB_USER=your-db-username
DB_PASSWORD=your-db-password
DB_NAME=AI_CourseCalV2
```

Make sure `.env` is excluded from version control:
```bash
echo ".env" >> .gitignore
```

**5. Start the development server**
```bash
cd flask
python app.py
```

The app will be available at `http://127.0.0.1:5000`.

---

## Getting Started

1. Log in to your account to access personalized features.
2. Add your completed courses under **My Courses**.
3. Browse prerequisite chains for courses you plan to take.
4. Check **Program Requirements** to confirm you are on track to graduate.
