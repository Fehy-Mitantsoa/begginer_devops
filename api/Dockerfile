FROM python:3.10

WORKDIR /app

COPY requirements.txt .

RUN pip install -r requirements.txt

COPY . .

FROM nginx:latest

COPY . /usr/share/nginx/html

EXPOSE 5000

CMD ["python", "app.py"]