# Explainable AI: An Explanatory Model for a Shift Scheduling Algorithm

## Overview

This repository is dedicated to a Master's thesis project from [TUM-fml](https://www.mec.ed.tum.de/en/fml/cover-page/), which focuses on developing a web application that provides explanations for a preference-based shift scheduling system powered by Constraint Programming.

For more information, please refer to the [HPAO project](https://www.mec.ed.tum.de/en/fml/forschung/2022/hpao-a-human-prefrerence-aware-optimization-system/).


## Architecture

The software architecture consists of four key components:

- **Frontend**: Developed using React for a dynamic UI.
- **Backend**: Built with Python Flask for managing API calls and COP model data manipulation.
- **COP Model**: Constraint Optimization Programming model for generating optimized shift plans. This is taken from the [HPAO project](https://www.mec.ed.tum.de/en/fml/forschung/2022/hpao-a-human-prefrerence-aware-optimization-system/)

## Features

The Explanatory Model includes the following key features:

- Get-Started Infographic
- What-If Scenarios
- Educational Game: Shift Puzzle Game
- Theory Classroom: FAQ and Quiz

## Project Structure

This repository is organized as follows:

- **backend**: This directory contains all the server-side logic.

- **frontend**: All client-side code is located here.

The backend and the frontend each contain their own README file.

## How to Run Locally

1. Clone this repository.
2. Run `pip install -r requirements.txt` in the `backend` folder to install Flask and other Python dependencies.
3. Run `python backend.py` in a terminal to run the Flask backend locally (per default, it will run on `localhost:5000`).
4. Open a second terminal. There you will run the React Frontend locally.
5. In the new terminal, run `npm install` in the `xai_frontend` folder to install React dependencies.
6. Run `npm start` to start the React development server.
7. Your browser will open automatically and show the web application.

## Contact

E-Mail: giaphong.tran@tum.de or charlotte.haid@tum.de