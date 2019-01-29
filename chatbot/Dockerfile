FROM python:3.7
RUN apt-get update && apt-get install -y git python3-dev gcc 
COPY requirements.txt /src/requirements.txt
WORKDIR /src
RUN pip install -r requirements.txt
COPY ./src /src
ENTRYPOINT ["python", "-u", "main.py"]