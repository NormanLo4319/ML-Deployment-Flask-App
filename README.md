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

```
conda activiate flask_demo # activate the flask_demo environment for the project
cd __Demo # create the Demo folder to contain the project components
pip install flask # install flask to this project environment
```

