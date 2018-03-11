#Monarch Inspection Database
---
[Monarch Safety Management](http://monarchsafetymanagement.com) inspection database website project. Intended to allow user-friendly industrial safety and health inspections to be performed in a browser, then tracked, reviewed with the same interface. Currently uses [django](https:djangoproject.com "django homepage") web framework for both frontend and backend database management. Database management may have to be ported if usage grows.
---

#Getting Started

The database is built on the django framework, which in turn is built on python. Tests use the Selenium web driver with python bindings.

##Prerequisites
Requires [Python 3.6](https://python.org/downloads/ "Python download page") or higher.

After installing python according to the instructions for your environment, install the django and Selenium packages.
```python
pip install django
pip install selenium
```
Selenium also requires a browser driver from the browser vendor. Development has only used [Chrome](https://chromedriver.storage.googleapis.com/index.html?path=2.35/ "Chrome driver download") so far. Whichever browser you use, the driver will have to be added to your system PATH variable for selenium to access. [Selenium](http://www.seleniumhq.org/download/ "Selenium download page") download page with alternate language bindings and all available browser drivers.

##Installation
Installation just requires downloading source code into a single user-accessible directory.
---

#First Run
---

##Setup
Navigate your terminal to the project directory.
`cd ~/Project/Path/InspectionDatabase`

Before running the first time, run database migrations to make sure all django components are playing nicely.
`python manage.py makemigrations`
`python manage.py migrate`

Then run the local server.
`python manage.py runserver`

Point your browser at [localhost port 8000](http://localhost:8000/) to start exploring the interface.
---

#Testing, deployment, etc.
Still in development...
