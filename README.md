This project has code samples to illustrate the use of poetry.

To install poetry dependencies:
"""poetry install"""

To add a new library to the project:
"""poetry add requests"""

To add a new library only to the dev group:
"""poetry add sphinx --group dev"""

After adding manually a dependency to the project.toml file:
1) Run the following to add it to the current poetry.lock file
"""poetry lock"""
2) Run install again to update the installed environment:
""" poetry install"""

In case you do not want to update the versions of the current dependencies:
"""poetry lock --no-update"""

Open a python REPL within poetry environment:
"""poetry run python"""

Update all dependencies (it affects the toml, lock file and environment):
"""poetry update"""

Update an specific dependency (it affects the toml, lock file and environment):
"""poetry update requests beautifulsoup4"""

Create a poetry project from an existing folder:
"""poetry init"""

Add dependencies from an existing requirements.txt file:
"""poetry add $(cat requirements.txt)"""

Create a requirements file from lock file:
"""poetry export --output requirements_from_lock.txt"""

To execute a script in poetry environment:
"""poetry run some_script.py"""

To activate the poetry environment in a nested shell:
"""poetry shell"""

To find the poetry environment path to activate it manually:
"""poetry env info --path"""
"""path_to_venv\Scripts\activate.ps1"""
"""& ((poetry env info --path) + "\Scripts\activate.ps1")""" (one liner)
