FROM python:3.10

WORKDIR /app

COPY api.py /app/
COPY model /app/model

RUN pip install fastapi uvicorn torch transformers

EXPOSE 80

CMD ["uvicorn", "api:app", "--host", "0.0.0.0", "--port", "80"]