FROM python:3.8
LABEL maintainer="Shohrab Uddin"

COPY . /app
WORKDIR /app
RUN pip install -r requirements.txt
#command to initialize the database
RUN python init_db.py
# command to start the app 
CMD [ "python", "app.py" ]
EXPOSE 3111
