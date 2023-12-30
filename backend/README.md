# Backend for XAI Model

This backend serves as part of the XAI Scheduling Model and facilitates the computation of shift schedules considering preferences and availabilities.

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