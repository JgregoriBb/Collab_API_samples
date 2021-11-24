# Collab_API_samples
Blackboard Collaborate and Learn API samples for session report by course and session patching

This repository contains code samples covering REST API usage for Blackboard Collaborate and Blackboard Learn for the following use cases

1. Check the Collaborate sessions that have guest access enabled and patch them
2. Create a report on the Collaborate sessions per Learn course that outputs a CSV file

These examples are written in python 3 by leveraging the Bb-rest-helper library and Jupyter notebooks (as it is easy and convenient to run different parts of the code). 

## Disclaimer

These code samples and the underlying Bb-rest-helper library are not supported by Blackboard and no warranties of any kind are provided.The intended usage is as tool to understand the REST Apis and the technical possiblities.

## Setup

1. Get the credentials for the Blackboard Collaborate API (The same LTI credentials configured in the Learn instance)and configure an application in Learn [guide](https://docs.blackboard.com/rest-apis/learn/getting-started/first-steps)
2. Clone this repository or download the files.
3. Navigate to the credentials folder and edit `collab_config.json`and `learn_config.json`

```json
{
    "url":"your server url",
    "key":"your key",
    "secret":"your secret"
}
```
4. Set up your development environment, I have used VS Studio Code with python, jupyter and github extensions.
5. Create a virtual environment

```python
python3 -m venv env
```

6. Use `pip` to install the `Bb-rest-helper` and the `Jupyiter library`

```python
pip3 install Bb-rest-helper
pip3 install jupyter
```
7. Configure the virtual environment as the kernel for the jupyter notebook. Follow the [guide](https://code.visualstudio.com/docs/datascience/jupyter-notebooks)
8. Run or modify the examples at your leisure
