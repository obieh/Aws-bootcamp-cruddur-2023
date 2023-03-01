FROM python:3.10-slim-buster

# Inside the container. 
# make a new folder inside the container
WORKDIR /backend-flask

# Outside container -> Inside container
# This contains the libraries that we want to install
COPY requirements.txt requirements.txt

# Inside the container
# Install the python libraries used for the app
RUN pip3 install -r requirements.txt

# Outside container -> Inside Container
# . means everything in the current directory
# first period . - /backend-flask (outside container)
# second period . - /backend-flask (inside container)
COPY . .

# Set Enviroment variables (Env Var)
ENV FLASK_ENV=development

EXPOSE ${PORT}
# CMD (command)
# python3 -m flask run --host --port4567
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]