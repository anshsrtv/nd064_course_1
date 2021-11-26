FROM python:3.6
LABEL maintainer="Ansh Srivastava"

WORKDIR /app
COPY techtrends /app

EXPOSE  3111

RUN pip install -r requirements.txt

# initialize database
CMD ["python", "init_db.py"]

# command to run on container start
CMD [ "python", "app.py" ]