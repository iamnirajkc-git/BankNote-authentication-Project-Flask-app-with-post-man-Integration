#### Bank Note Authentication Project #########
This is a project that uses a Random Forest model to authenticate bank notes. It includes a Flask app that serves as the API for the model and a Postman app that allows you to test the API.

# Getting Started
To get started with this project, you will need to do the following:

Clone the repository to your local machine.
Install the required packages.
Run the Flask app by running python flaskApp.py in your terminal.
Open Postman and test the API by sending a POST request to http://localhost:5000/predict with a JSON payload or csv file containing the bank note features to authenticate.

# Usage
Bank Note Authentication
To authenticate a bank note, send a POST request to http://localhost:5000/predict with a JSON payload containing the following features:

variance
skewness
curtosis
entropy
The API will return a JSON response indicating whether or not the bank note is authentic.

##### Sample Request #######

POST http://localhost:5000/predict
Content-Type: application/json

{
    "variance": -2.432,
    "skewness": 4.321,
    "curtosis": 2.543,
    "entropy": -1.234
}


###### Sample Response #####


{
    "result": "authentic"
}

### License
This project is licensed under theApache License - see the LICENSE.md file for details.
