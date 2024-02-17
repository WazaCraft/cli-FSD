# cli-FSD
Natural language interface for your command line. 

A lightweight and portable autopilot utility for CLI tasks. Takes natural language as input and uses the OpenAI API to take the appropriate actions by generating and parsing shell scripts. Find answers to questions and let AI execute commands with your permission in Safe Mode or enable Autopilot to automate tasks or make script modules and microservices on the fly. 

**Warning**: Giving LLMs shell-level access to your computer is dangerous and should only be done in sandbox or otherwise expendable environments. 

## Getting Started

### Prerequisites

- Python 3.10 or later (may work with earlier versions)
- pip 24.0 or later 
- An OpenAI API key

### Installation

0. **Pre-requisites:**
- Upgrade pip
    ```
     python3 -m pip install --upgrade pip
    ```

**Install using pip:**

    ```bash
    pip install cli-FSD
    ```
  (if you are testing the package, follow steps to setup and activate a virtual environment **before** running pip install.).

**Manual Installation**

1. **Clone the repo:**

    ```bash
    git clone https://github.com/WazaCraft/cli-FSD
    cd cli-FSD
    ```

2. **Set up a Python virtual environment:**

    ```bash
    python -m venv FSD
    ```

3. **Activate the virtual environment:**

    - On Windows:

        ```cmd
        .\FSD\Scripts\activate
        ```

    - On Unix or MacOS:

        ```bash
        source FSD/bin/activate
        ```

4. **Install the cli-FSD Python package:**

    ```bash
    pip install .
    ```
   
### Usage

- To start in safe-mode in your Terminal:

    ```bash
    @ what time is it -s
    ```

- To run in companion mode and process a specific task using autopilot type '@' from anywhere in your terminal followed by a command:

    ```bash
   @ what time is it
    ```

- For additional options, you can enter `CMD` mode by typing `CMD` at any prompt.

### Contributing

Contributions to this project are welcome. Please fork the repository, make your changes, and submit a pull request for review.

## License

This project is licensed under the GNU GPL - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

- OpenAI for providing the API used for generating chat responses.
- Flask and Flask-CORS for the web server functionality.
