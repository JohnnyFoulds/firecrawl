# Playwright Service

## Create Environment

```bash
conda create -n firecrawl python=3.11
conda activate firecrawl  

pip install -r requirements.txt -r requirements_dev.txt 
playwright install chromium && playwright install-deps chromium
```

## Run Service

```bash
uvicorn main:app --host 0.0.0.0 --port 5003 --reload
```

The swagger documentation can then be viewed at `http://localhost:5003/docs`.