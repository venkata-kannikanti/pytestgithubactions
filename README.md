# Python-Selenium-Pytest
## Setup Your Working Enviorment

For Windows:
* Install scoop from www.scoop.sh
* Install allure commandline by running the following command:
```
scoop install allure
```

For Mac OS X:
* Install brew from https://brew.sh/
```
brew install allure
```

* git clone
* cd to project directory 
* Install virtualenv:
```
py -m pip install --user virtualenv
```
* Create a virtual environment: 
```
py -m venv testenv
```
* Activate your virtual environment:
```
.\testenv\Scripts\activate
```
* install pipenv:
```
pip install pipenv
```
* install project dependencies using pipenv: 
```
pipenv install
```

## Run Tests

```
pipenv run pytest --alluredir=allure-results --browser <firefox/remote/chrome_headless>
```
if no browser was selected then chrome will be used.

* Run according to tags:
```
pipenv run pytest -k "<tag_name>" --browser <firefox/chrome/remote/chrome_headless>
```

## View Test Results

* view allure results: 
```
allure serve allure-results
```
## View Help And Custom CLI Options

```
pytest --help
```
