## LEGENDS
[] - not Started
[-] - completed
[~] - in Progress
[x] - discontinued


## To Remember
```
1. Always run "git checkout develop" and "git checkout -b feature/{feature_name}" before starting a new feature.

2. Always confirm the feature branch before making and pushing changes.

3. After implementing a feature run
  |-"git add ."
  |-"git commit -m "{commit_message}"
  |-"git push -u origin feature/{feature_name}"

```

## DATA VARIABLES
1. GITIGNORE_CONTENT ={
  # Python
__pycache__/
*.py[cod]
*.pyo
*.pyd

# Virtual Environment
venv/
.venv/
env/

# Environment Variables
.env

# Django
db.sqlite3
media/
staticfiles/

# Logs
*.log

# Migrations (optional)
# */migrations/*
# !*/migrations/__init__.py

# IDE
.vscode/
.idea/

# OS
.DS_Store
Thumbs.db

# Testing
.coverage
htmlcov/
.pytest_cache/

# Type Checking
.mypy_cache/

# Distribution
build/
dist/
*.egg-info/
}


#


## Initialize Django
1. [-] Django Setup
      [-] run "python -m venv venv" to setup the virtual environment called venv.
      [-] run "venv/Scripts/activate" to activate the virtual environment.
      [-] run "pip install django" to install django
      [-] run "django-admin startproject backend ."
      [-] run "python manage.py runserver" to confirm the initial django setup is done.

2. [-] Git and Github Setup
      [-] create a ".gitignore" file.
      [-] Paste GITIGNORE_CONTENT in the file.
      [-] run "git init" to initialize git in the project.
      [-] run "git status" to confirm.
      [-] run "git add ." to track the files.
      [-] run "git commit -m "initial project setup" to commit the changes.
      [-] run "git remote add origin https://github.com/{USERNAME}/{REPO_NAME}.git" to add the project to github.
      [-] run "git remote -v" to confirm.
      [-] run "git branch -M main" to rename the master branch "main".
      [-] run "git push -u origin main" to push all changes to the master branch. '-u' is for the first push.
      [-] run "git checkout -b develop" to create the develop branch.
      [-] run "git push -u origin develop" to push the changes to the develop branch.

## StartApp
