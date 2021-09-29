# Flask App Deployment Demo

This repository demonstrate the steps for setting up a simple ML model and deploy with Flask App that lives on Heroku environment.

### Deployment

Generally speaking, deployment is the mehtod by which we integrate a machine learning model into an existing production environment to make practical business decision based on data. The purpose of deploying a model is so that we can make the predictions from a trained ML model available to others, whether that be users, management, or other systems. Model deployment is closely related to ML system architecture, which refers to the arrangement and interactions of software components within a system to achieve a predefined goal.

### Flask Framework

Flask is a micro web framwork written in Python. It is classified as a mcroframework because it does not require particular tools or libraries.

Project Structure:

1. model.py: This contains the machine learning model to make prediction.
2. app.py: This contains Flask APIs that receives input through API calls, then computes predicted value based on our model and returns it.
3. request.py: This uses requests module to call APIs defined in app.py and displays the retured value.
4. HTML/CSS: This contains the HTML template and CSS styling to allow user to enter the credentials.

### Project Workflow

1. Create a new conda environment for the project

Terminal:

``` sh
conda activiate flask_demo # activate the flask_demo environment for the project
cd __Demo # create the Demo folder to contain the project components
pip install flask # install flask to this project environment
```

Visual Studio Code:

1. Go to the __Demo folder
2. Create the "app.py" file
3. Create the "request.py" file
4. Create the "requirements.txt" file
5. Create the "Profile" file
6. Create a "templates" folder
7. Create the index.html and result.html files inside the "templates" folder
8. Create a "static" folder and a "css" folder within the "static" folder
9. Create the "style.css" file inside the "css" folder
10. Create a "model" folder
11. Copy and paste the "model.py" and "model.pkl" file inside the "model" folder

Structure of the folders and files in the project folder:

~~~
  ├── .gitignore
  ├── Procfile
  ├── app.py
  ├── requirements.txt
  └── runtime.txt
~~~

app.py File: (general structure)

``` Python
# Import Flask 
from flask import Flask, render_template, request

# Create the application
app = Flask(__name__)

# Something in between ....

# Run the app
if __name__ == "__main__"
  app.run()
```





