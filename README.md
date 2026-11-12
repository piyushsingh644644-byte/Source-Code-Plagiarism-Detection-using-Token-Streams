# LEXGUARD.AI — Flask Deployment

## Local run
```bash
python -m venv .venv
# Windows:
.venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate

pip install -r requirements.txt
python app.py
```

Open http://localhost:5000

## Deploy
This is a standard Flask web app. On Render, Railway, or another Python host:
- Build command: `pip install -r requirements.txt`
- Start command: `gunicorn app:app`

The plagiarism analysis is performed by the Python API endpoint `/api/scan`.
