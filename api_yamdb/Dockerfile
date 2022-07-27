FROM python:3.7

WORKDIR /app

COPY . .
COPY ./api_yamdb .

RUN pip install --upgrade pip
RUN pip install -r requirements.txt --no-cache-dir

CMD ["gunicorn", "api_yamdb.wsgi:application", "--bind", "0:8000"]
