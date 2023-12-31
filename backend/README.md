# Backend for XAI Model
This backend serves as part of the Shift Scheduling XAI Model and provides data for the XAI frontend. 

## Installation

Before using this backend, please follow these steps:

1. **Python and pip:** Ensure that you have Python 3.6+ and pip (Python package manager) installed on your system. You can download Python from the official website: [Python Downloads](https://www.python.org/downloads/).

2. **Virtual Environment (Optional):** It's recommended to create a virtual environment to isolate project dependencies. You can create one using the `venv` module:

    ```bash
    # Create a virtual environment (optional)
    python -m venv venv

    # Activate the virtual environment (Windows)
    .\venv\Scripts\activate

    # Activate the virtual environment (macOS/Linux)
    source venv/bin/activate
    ```

3. **Install Dependencies:** Use the provided `requirements.txt` file to install the required Python packages. Run the following command within the project directory:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

After completing the installation steps, you can run the backend to create or modify shift schedules. Here are the key endpoints and their usage:

- **/schedule:** This endpoint generates the current shift schedule.
- **/solve_shifts_what_if:** This endpoint allows for the calculation of shift schedules taking into account user preferences and availabilities.

By default, the backend runs on port 5000 (this can be adjusted in the code), which can be reached via `localhost:5000`.

## Code Structure

The backend code is organized as follows:

- `backend.py`: This file contains the main Flask application and the API endpoints for generating shift schedules.

- `requirements.txt`: This file lists the required Python packages and their versions. You can use it to install the dependencies for the project.

- `cop_model/ShiftOptimizer.py`: The `ShiftOptimizer.py` file in the `cop_model` subfolder contains the constraint optimization model for an exemplary shift scheduling problem. It defines the optimization model, decision variables, and constraints using the [OR-Tools CP-SAT solver](https://developers.google.com/optimization/cp/cp_solver).

## ShiftOptimizer.py
  
The `ShiftOptimizer.py` contains classes and methods for optimizing employee shift scheduling based on preferences and constraints. Here's a brief description of the key components in the file:

1.  `VarArraySolutionPrinter` Class:
    
    -   This is a custom callback class for the CP-SAT solver.
    -   It is used to collect and structure employee shift-scheduling solutions.
    -   The class overrides the `on_solution_callback` method to adapt the solution to a human-readable format.
    -   It stores the solutions and their total preference values in a structured format.
    -   It also provides methods for accessing the solutions and the total preference values.
2.  `ShiftOptimizer` Class:
    
    -   This is the main class for optimizing employee shift scheduling.
    -   It takes into account various preferences and constraints, including employee preferences, qualifications, availability, and rotation preferences.
    -   The class allows you to initialize the shift optimization problem with various parameters.
    -   It defines the optimization model, decision variables, and constraints using the OR-Tools CP-SAT solver.
    -   The class provides methods for updating preferences and availabilities, solving the shift scheduling problem, and retrieving the results.
    -   It also includes methods for calculating the number of shifts per employee and individual preference scores.

## Additional Resources

- [Flask Documentation](https://flask.palletsprojects.com/en/2.1.x/): For more information on using Flask to build web applications.

- The shift scheduling COP model used in this project is taken from [TUM-fml](https://www.mec.ed.tum.de/en/fml/cover-page/). You can find the source code and more information in the corresponding TUM-fml repository: [algorithmic- scheduling](https://github.com/tum-fml/algorithmic-scheduling) (Code related to the paper "Accommodating Employee Preferences in Algorithmic Worker-Workplace Allocation").
- Google OR-Tools:  The Shift Scheduling algorithm uses the [OR-Tools CP-SAT solver](https://developers.google.com/optimization/cp/cp_solver).
