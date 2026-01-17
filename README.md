# gem3-hackathon

## Running locally
(create a virtual environment)
### 1. Djangoproj
```bash
cd djangoproj
pip3 install -r requirements.txt 
gunicorn djangoproj.asgi:application -k uvicorn.workers.UvicornWorker
```
### 2. frontend
```bash
npm install
npm run dev
```
### 3. Fastapi (agentic service)
```bash
cd agenticService
pip3 install -r requirements.txt
uvicorn main:app --reload --port 8080
```
