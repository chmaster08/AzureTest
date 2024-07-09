FROM python:3.10

WORKDIR /app

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

COPY . .

RUN apt-get update && apt-get install -y supervisor


EXPOSE 5000

CMD [ "python3" , "app.py" ]