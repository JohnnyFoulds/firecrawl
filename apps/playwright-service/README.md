# Playwright Service

## Create Environment

```bash
conda create -n firecrawl python=3.11
conda activate firecrawl  

pip install -r requirements.txt  
playwright install chromium && playwright install-deps chromium
```

## Run Service

```bash
uvicorn main:app --host 0.0.0.0 --port 5003
```