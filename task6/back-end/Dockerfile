# use latest ubuntu image as base
FROM ubuntu:latest

# update and upgrade all system package automatically
RUN apt-get update && apt-get upgrade -y

# install Python3 and pip3, remove the "externally-managed" lock
RUN apt-get install -y python3 python3-pip
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# install flask using pip3
RUN pip3 install flask
RUN pip3 install flask-cors


# set the working directory and copy python file
WORKDIR /app
COPY api.py /app/api.py

# expose port 5252 and start flask app
EXPOSE 5252
CMD ["python3", "api.py"]