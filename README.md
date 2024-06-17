# calc_design_patterns

## Project Overview

This project focuses on the development of an interactive command-line application that operates continuously, transitioning from a single-execution script to a fully functional application. Through this assignment, you will explore the command pattern, learn how to dynamically load commands using a simple plugin architecture, and understand the appropriate use of exceptions versus conditional statements to manage invalid data inputs. This unit lays the foundational skills for application development, preparing you for the midterm project, which requires a thorough explanation of your program's architecture, design patterns, and functionality.


## Prerequisites

- Python 3.10 or higher
- pip (Python package installer)

  
## Installation

1. Clone the repository:

```
git clone https://github.com/chaitanya-kumar33/calc_design_patterns.git
```

2. Navigate to the project directory:

```
cd calc_design_patterns
```

3. Install the required dependencies:

```
pip install -r requirements.txt
```

## Usage

To start the calculator, run the following command:

```
python main.py
```

This will launch the REPL interface, where you can perform arithmetic operations, manage calculation history, and access additional functionalities through plugins.

### Commands

- `add <operand1> <operand2>`: Performs addition of two numbers.
- `subtract <operand1> <operand2>`: Performs subtraction of two numbers.
- `multiply <operand1> <operand2>`: Performs multiplication of two numbers.
- `divide <operand1> <operand2>`: Performs division of two numbers.
- `history`: Displays the calculation history.
- `clear`: Clears the calculation history.
- `load <plugin_name>`: Loads a plugin and makes its commands available.
- `plugins`: Lists all available plugins and their commands.
- `exit`: Exits the calculator application.

### Plugins

The calculator supports dynamic loading of plugins. To load a plugin, use the `load <plugin_name>` command. Once a plugin is loaded, its commands become available within the REPL.

## Features

- **Command-Line Interface (REPL)**: An interactive environment for performing arithmetic operations and managing calculation history.
- **Plugin System**: A system to extend functionalities through dynamically loaded plugins.
- **Calculation History Management with Pandas**: Leverages Pandas for robust management and manipulation of calculation history.
- **Comprehensive Logging**: Implements detailed logging for operations, errors, and informational messages.
- **Design Patterns**: Utilizes Facade, Command, Factory Method, Singleton, and Strategy Patterns for a scalable and flexible architecture.
  
The design patterns used in this project promote modularity, extensibility, and maintainability. For more details on their implementation and impact, please refer to the respective sections in the source code.

## Logging

The calculator application uses a comprehensive logging system to record detailed application operations, data manipulations, errors, and informational messages. The logging system supports different log levels (INFO, WARNING, ERROR) and can be configured to output logs to various destinations (console, file) through environment variables.

The following environment variables can be used to configure logging:

- `LOGGING_LEVEL`: Sets the logging level (DEBUG, INFO, WARNING, ERROR, CRITICAL).
- `LOGGING_FILE`: Specifies the file path for logging output.

## Testing

Run the following command to execute tests and ensure the application behaves as expected:

```bash
pytest
```


