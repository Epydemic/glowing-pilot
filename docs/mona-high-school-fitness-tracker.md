# Getting started - app frontend and backend creation

## Explain to GitHub Copilot the goals and steps

```text
I want to build an monafit Tracker app that will include the following:

* User authentication and profiles
* Activity logging and tracking
* Team creation and management
* Competitive leader board
* Personalized workout suggestions

It should be in one app

generate instructions in this order

1. Create the frontend and backend in the monafit-tracker directory structure of this repository in one command
2. Setup backend python venv and create a monafit-tracker/backend/requirements.txt file
3. Install all required Python packages listed in requirements.txt
```

### Commands to create the directory structure and setup backend

```bash
# Step 1: Create the directory structure
mkdir -p octofit-tracker/{backend,frontend}

# Step 2: Setup Python virtual environment for the backend
python3 -m venv octofit-tracker/backend/venv
source octofit-tracker/backend/venv/bin/activate

# Step 3: Create requirements.txt and install dependencies
cat <<EOL > octofit-tracker/backend/requirements.txt
Django==4.1
djangorestframework==3.14.0
django-allauth==0.51.0
django-cors-headers==4.5.0
dj-rest-auth
djongo==1.3.6
pymongo==3.12
sqlparse==0.2.4
stack-data==0.6.3
sympy==1.12
tenacity==9.0.0
terminado==0.18.1
threadpoolctl==3.5.0
tinycss2==1.3.0
tornado==6.4.1
traitlets==5.14.3
types-python-dateutil==2.9.0.20240906
typing_extensions==4.9.0
tzdata==2024.2
uri-template==1.3.0
urllib3==2.2.3
wcwidth==0.2.13
webcolors==24.8.0
webencodings==0.5.1
websocket-client==1.8.0
EOL

pip install -r octofit-tracker/backend/requirements.txt
```
