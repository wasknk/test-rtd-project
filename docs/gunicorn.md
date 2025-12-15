# gunicorn

## Install
```
pip install gunicorn uvicorn 'uvicorn[standard]'
```

## Run 1

```bash
gunicorn app:app --workers 4 --bind 0.0.0.0:8000
```

## Run 2
```bash
gunicorn app.main:app \
         --workers 4 \
         --worker-class uvicorn.workers.UvicornWorker \
         --bind 0.0.0.0:8000

```