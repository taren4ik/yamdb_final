FROM python:3.7-slim

RUN mkdir /app

COPY . .

RUN pip3 install -r /app/requirements.txt --no-cache-dir

WORKDIR /app
CMD ["gunicorn", "api_yamdb.wsgi:application", "--bind", "0:8000" ] 

LABEL author='turgenevski@yandex.ru' version=1.0