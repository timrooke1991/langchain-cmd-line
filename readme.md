# LangChain Command Line - Create code and test it

## Overview

This project utilizes the `langchain` library to create a customizable code generation and testing pipeline. It leverages OpenAI's language models to generate Python code based on specified tasks and then creates tests for that code.

## Installation

Before using this project, ensure you have Python installed. Then, install the required packages using pip:

bashCopy code

`pip install langchain dotenv argparse`

## Configuration

The project uses environment variables to manage sensitive information like API keys. Place your environment variables in a `.env` file in the root directory.

## Usage

To use the script, run it with the desired task and programming language as arguments. The default language is Python, and the default task is to return a list of numbers.

Example:

bashCopy code

`python your_script.py --task "calculate factorial" --language "python"`

This command will generate Python code for calculating a factorial and its corresponding test.

## Components

1.  **LLM and Prompt Template**: Utilizes `OpenAI` and `PromptTemplate` from the `langchain` library to define the structure of the prompts for generating code and tests.
2.  **Chains**: Uses `LLMChain` for generating code and tests separately, and `SequentialChain` to link these processes.
3.  **Argument Parser**: Employs `argparse` for command-line argument parsing to specify the task and programming language.
4.  **Result**: The script outputs the generated code and test to the console.

## Customization

You can customize the tasks and the programming language by modifying the arguments passed to the script.

## Contribution

Contributions to improve the script or add more features are welcome. Please ensure to follow the coding standards and write tests for new features.

## License

This project is licensed under the [MIT License](https://chat.openai.com/c/LICENSE.md).

---

**Note**: This README assumes basic familiarity with Python and command-line operations. It's important to keep the `.env` file secure as it may contain sensitive API keys.
