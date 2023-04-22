FROM python:3.11-alpine

WORKDIR /usr/src/stocks_products

COPY . .

RUN pip3 install --no-cache-dir --upgrade -r requirements.txt
RUN python manage.py migrate
RUN python manage.py loaddata stocks_products.json

EXPOSE 1010

CMD ["python", "manage.py", "runserver", "0.0.0.0:1010"]
