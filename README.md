# Djangae Template Project

This is a barebones project template configured for use on Google App Engine Standard
using the [Djangae](https://github.com/potatolondon/djangae) framework.

# Using the Djangae Scaffold template

1. Install any version of Django supported by Djangae
2. Run the following command, replacing `myproject` with the name of your project

```
$ django-admin.py startproject --template https://github.com/potatolondon/djangae-scaffold/zipball/master --extension py,yaml,md myproject
```

3. Create a virtualenv and activate it (e.g. `virtualenv .venv && source .venv/bin/activate`)
4. Install the requirements: `pip3 install -r requirements.txt`
