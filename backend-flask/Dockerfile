FROM python:3.8.16-slim-bullseye

RUN mkdir flask/

COPY . flask/

WORKDIR /flask/

RUN pip3 install -r requirements.txt

RUN pip3 install python-dotenv

EXPOSE 4567

CMD [ "python3", "-m", "flask", "run", "--host=0.0.0.0", "--port=4567" ]