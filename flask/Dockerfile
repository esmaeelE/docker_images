---
# syntax=docker/dockerfile:1



FROM python:alpine

WORKDIR /app

COPY requirements.txt requirements.txt

ENV PIP_ROOT_USER_ACTION=ignore
RUN pip3 install -r requirements.txt

COPY . .

# ?
#ENTRYPOINT ["python3"] 
#CMD ["app.py"] 

EXPOSE 5000 

# how to not use host and listen on localhost
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0"]

