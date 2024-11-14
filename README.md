# Hospital-Appointment-Scheduler

A web-based appointment scheduling system where patients can schedule appointments with doctors, validate patient IDs, and ensure no time conflicts.

## Features
- Schedule appointments with **Dr. Ahmad (Neurologist)** or **Dr. Fatima (Dermatologist)**.
- Validate patient ID range for each doctor.
- Avoid conflicting appointment times.
- User-friendly interface built with **Bootstrap**.

## Technologies
- **Backend**: Flask, Python
- **Frontend**: HTML, CSS (Bootstrap)
- **Machine Learning**: Scikit-learn (for future predictions)
- **API Communication**: JSON over HTTP
- **Cross-Origin Requests**: Flask-CORS

## Setup

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/doctor-appointment-scheduling.git
cd doctor-appointment-scheduling
```

### 2. Install Backend Dependencies

```bash
python -m venv venv  # Create virtual environment
# Activate it:
# On Windows: venv\Scripts\activate
# On macOS/Linux: source venv/bin/activate
pip install -r requirements.txt  # Install dependencies
```

### 3. Run Backend

```bash
python app.py  # Start the Flask server
```

The server will run at `http://127.0.0.1:5000/`.

### 4. Frontend

Open `index.html` in your browser to access the scheduling form.

## API Endpoint

### `POST /schedule`

- **Request**: JSON data (name, gender, doctor, patient_id, hour, duration, date)
- **Response**: Success or failure message in JSON format.

