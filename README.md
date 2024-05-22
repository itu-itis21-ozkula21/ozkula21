# PROJECT REPORT FOR YZV104E  

**150210312 Ahsen Beyza Özkul**

_ozkula21@itu.edu.tr_


# QUIZOPIA - A Web-Based Quiz Application 


QUIZOPIA is a simple and interactive web-based quiz application built using Flask. It allows users to test their general knowledge, receive instant feedback on their performance, and visualize their scores over time. This project serves as an excellent example of integrating Python with web technologies to create dynamic and user-friendly applications.

## Table of Contents

- [Features](#features)
- [Project Structure](#project-structure)
- [Requirements](#requirements)
- [Python Version](#python-version)
- [Installation and Setup](#installation-and-setup)
- [Usage](#usage)
- [Visualization](#visualization)
- [Acknowledgments](#acknowledgments)

## Features

- **User-Friendly Interface**: Simple and intuitive design for an enhanced user experience.
- **Real-Time Scoring**: Immediate feedback on quiz performance.
- **Score Visualization**: Bar charts to visualize user scores and track progress over time.
- **Responsive Design**: Compatible with various devices, ensuring a seamless experience on both desktops and mobiles.

## Project Structure

The project is organized as follows:

- `app.py`: The main application file that defines the Flask routes and handles user interactions.
- `visualization.py`: A script for generating bar charts to visualize user scores.
- `templates/`: Directory containing HTML templates for the application.
  - `index.html`: The homepage where users enter their username to start the quiz.
  - `quiz.html`: Displays each quiz question and captures user responses.
  - `result.html`: Shows the user's score and a bar chart of scores.
- `quiz_data.csv`: A CSV file that stores quiz data, including usernames and scores.
- `generated_charts/`: Directory where generated chart images are saved.
- `requirements.txt`: Lists all the dependencies required for the project.

## Requirements

To run this project, you need the following Python libraries:

- Flask
- Flask-Bootstrap
- matplotlib
- numpy
- csv

You can install all required libraries using the following command:

```
pip install -r requirements.txt
```

## Python Version

This project was developed using Python 3.11. It is recommended to use this version to ensure compatibility and smooth running of the application.

## Installation and Setup

Follow these steps to set up the project on your local machine:

1. Create a virtual environment:
```
python3 -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

3. Install the required libraries:
```
pip install -r requirements.txt
```
3. Run the Flask application:
```
python app.py
```
5. Open your web browser and navigate to **http://127.0.0.1:5000** to access the application.

## Usage

1. Start the application by running the **app.py** file.
2. Enter your username on the index page to begin the quiz.
3. Answer the quiz questions presented on the subsequent pages.
4. Submit your answers to see your score and a bar chart of user scores.

## Visualization

The bar chart visualizing the scores is generated using the **visualization.py** script. The chart is saved in the **generated_charts** directory and is dynamically loaded on the result page when the user finishes the quiz. This visual representation helps users track their performance and compare their scores with others.

To generate the chart, the **visualization.py** script reads the **quiz_data.csv** file, which contains the quiz results. It then creates a bar chart and saves it as an image in the **generated_charts** directory. This image is displayed on the result page.

## Acknowledgments

- [Flask](https://flask.palletsprojects.com/en/3.0.x/): A lightweight WSGI web application framework in Python.

- [Bootstrap](https://getbootstrap.com/): A popular front-end open source toolkit for developing with HTML, CSS, and JS.

- [matplotlib](https://matplotlib.org/): A comprehensive library for creating static, animated, and interactive visualizations in Python.



