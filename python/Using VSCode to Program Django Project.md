When we are going to develop a project by python Django framework, we usually create a dedicated virtual environment for the project to avoid libs inclusion compatibility issues.

Reference: https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/

1. Create a python virtual environment for the project

```shell
#Windows command shell
${workspace_folder}\>py -m venv env
```



2. Switch python interpreter to the one in the virtual environment

In VSCode, type `ctrl+shift+p` shortcut to call up the command palette. And then, enter `python: Select Interpreter ` to switch the python interpreter to the virtual environment we just created for the current workspace on the above step.

3. Activate the virtual environment

In the ${workspace_folder}, type `.\env\Scripts\activate` to activate the virtual environment.

4. Upgrade pip

In the best practice, we usually upgrade the pip lib management tool up-to-date before we install any libs.

```shell
#Windows command shell
${workspace_folder}\>py -m pip install --upgrade pip
```



5. Install necessary libs

For example, to install Django framework.

```shell
#Windows command shell
${workspace_folder}\>py -m pip install Django
```

If you've not activated the virtual environment before the lib installation, the lib will be installed under the global python environment.

6. Deactivate the virtual environment

```shell
#Windows command shell
${workspace_folder}\>.\env\Scripts\deactivate
```



