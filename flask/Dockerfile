# syntax=docker/dockerfile:1

FROM python:alpine

WORKDIR /app

COPY requirements.txt requirements.txt

# Not generate __pycache__
ENV PYTHONDONTWRITEBYTECODE=1
ENV PIP_ROOT_USER_ACTION=ignore
RUN pip install --upgrade pip && pip install -r requirements.txt

COPY app.py .

# ?
#ENTRYPOINT ["python3"] 
#CMD ["app.py"] 

# Our docker container serve on this port
EXPOSE 5000 

# how to not use host and listen on localhost, flask default port is 5000
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0"]

# Not work
#CMD [ "python3", "-m" , "flask", "run"]
