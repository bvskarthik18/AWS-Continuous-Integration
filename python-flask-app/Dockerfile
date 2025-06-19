#Base Image
FROM python:3.8

#set the working directory
WORKDIR /app

#copy the requirements file into the container
COPY requirements.txt .

#Install the dependencies
RUN pip install -r requirements.txt

#copy the application code into the container
COPY . .

#expose the port the app runs on
EXPOSE 5000

#set the environment variable
# ENV MY_ENV_VAR=app.py

#Run the application
CMD ["python", "app.py"]