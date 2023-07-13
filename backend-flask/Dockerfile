# Base image
FROM python:3-alpine

# Create working directory
WORKDIR /app

RUN python3 -m venv venv

RUN source venv/bin/activate

COPY requirements.txt .

RUN pip install -r requirements.txt

# Bundle app source
COPY . .

EXPOSE 5000

RUN pip install python-dotenv

ENV FLASK_APP=app.py

CMD [ "flask", "run","--host","0.0.0.0","--port","5000"]
