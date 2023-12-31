# Contributing to the Shift Scheduling XAI Model

Thank you for your interest in contributing to the Shift Scheduling XAI Model! Here are some guidelines to help you get started:

## Setting Up Your Development Environment

To contribute to the web application, you'll need to set up your development environment. Our application consists of a Flask backend for the server-side logic and a React frontend for the user interface. Follow these steps to get started:

### Prerequisites
Before you begin, ensure you have the following prerequisites installed on your system:

- **Python**: The Flask backend is written in Python. You can download it from the official Python website or use a package manager like Conda.

- **Node.js** and **npm**: We use Node.js and npm for managing dependencies and building the React frontend. You can download them from the official Node.js website.


### Backend Setup (Flask)
- Clone the Repository: Fork and clone the Git repository to your local machine.

- Create a Virtual Environment (optional but recommended): It is recommended to use a virtual environment to manage Python dependencies.

- Activate the Virtual Environment (if used): Activate the virtual environment to isolate dependencies.

- Install Python Dependencies: Install the required Python packages using the `requirements.txt`.

- Run the Flask App: Start the Flask development server by running `python backend.py` in the backend folder. This command will run the Python program.

- Your Flask backend should now be running locally (per default on `localhost:5000`).

### Frontend Setup (React)
Navigate to the `xai_frontend` directory:

- Install Frontend Dependencies using `npm install`. This will parse the `package.json` file.

- Start the React Development Server using `npm start`. Per default it will run on `localhost:3000`.

The React development server will start, and you can access the application's frontend locally.

## Making Changes

- Fork the repository on GitLab.
- Create a new branch from the main branch for your feature or bug fix.
- Test your changes thoroughly.

## Submitting a Pull Request

- Create a merge request (MR) with your changes.
- Provide a clear and descriptive title for your MR.
- Explain the purpose and scope of your changes in the PR description.
- Be responsive to any feedback or review comments by the maintainers of this repository. The current contact person is [Charlotte Haid](mailto:charlotte.haid@tum.de)  (as at: 31.12.2023)

Thank you for contributing to the Shift Scheduling XAI Model!

## License

By contributing to this project, you agree to abide by its [License](https://gitlab.lrz.de/00000000014A933A/xai_cp_scheduling/-/blob/main/LICENSE).

