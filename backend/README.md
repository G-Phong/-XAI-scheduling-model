# Backend for XAI Scheduling Model

This backend serves as part of the XAI Scheduling Model and facilitates the computation of shift schedules considering preferences and availabilities.

## Installation:

To run this backend, ensure you have the required dependencies installed. Use the requirements.txt file to install these de# Backend for XAI Scheduling Model

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

3. **Install Dependencies:** Use the provided `requirements.txt` file to install the required Python packages. Run the following command within your project directory:

    ```bash
    pip install -r requirements.txt
    ```


## Usage

After completing the installation steps, you can run the backend to create or modify shift schedules. Here are the key endpoints and their usage:

- **/schedule:** This endpoint generates the current shift schedule.
- **/solve_shifts_what_if:** This endpoint allows for the calculation of shift schedules taking into account user preferences and availabilities.

For more detailed information on usage and configuration of the backend, please refer to the documentation.

pendencies.


```bash
pip install -r requirements.txt
```
## Usage:

After installing the dependencies, you can run the backend to create or modify shift schedules. The key endpoints and their usage are:
```bash
/schedule 
```
This endpoint generates the current shift schedule.
```bash
/solve_shifts_what_if
```
This endpoint allows for the calculation of shift schedules taking into account user preferences and availabilities.




## License:

This project is licensed under the MIT License. For more information, see the LICENSE file.

We welcome contributions and feedback from developers. Please open an issue or a pull request to help us improve this project.