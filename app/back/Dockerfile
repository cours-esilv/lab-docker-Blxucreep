# use an official python runtime
FROM python:3.8-slim

# set the working directory in the container
WORKDIR /app

# copy the app.py file into the container at /app
COPY . /app

# install dependencies (here, it should install flask)
RUN pip install -r requirements.txt

# expose port 8080
EXPOSE 8080

# run the flask api when the container launches
CMD ["python", "-m", "flask", "run", "--host=0.0.0.0"]