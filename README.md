# Djangae Template Project

This is a barebones project template configured for use on Google App Engine Standard
using the [Djangae](https://github.com/potatolondon/djangae) framework.

# Using the Djangae Scaffold template

1. Create a virtualenv and activate it (e.g. `virtualenv .venv && source .venv/bin/activate`)
1. Install the requirements: `pip3 install -r requirements.txt`
1. Install the local development requirements: `pip3 install -r requirements-dev.txt`
1. Run the following command, replacing `myproject` with the name of your project

```
$ django-admin.py startproject --template https://gitlab.com/potato-oss/djangae/djangae-scaffold/-/archive/master/djangae-scaffold-master.zip --extension py,yaml,md myproject
```

# Differences to the Standard Template

 - Settings are divided into "default" and "production". Production sets DEBUG=False, and a number of security
   settings
 - App Engine specific files are included (e.g. app.yaml, .gcloudignore)
 - requirements.txt and requirements-dev.txt are provided for basic Djangae functionality
 - manage.py is updated to run various Google Cloud emulators locally when running management commands
 - '.appspot.com' is added to ALLOWED_HOSTS by default
 - [Google Cloud Logging](https://cloud.google.com/logging/docs) is enabled in production
 - [Google Cloud Debugger](https://cloud.google.com/debugger/docs/setup/python) is enabled in production
 - Google IAP authentication, and the `djangae.contrib.googleauth` User model are both configured by default
 - Username/password authentication backend is disabled by default
 - The default database is configured to use Google Cloud Datastore
 - Staticfiles is configured to serve from the 'static' folder by default
