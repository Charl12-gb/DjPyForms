# DjPyForms

## Description
DjPyForms is an automatic form generation tool for Django projects. It simplifies the creation of forms based on Django class models, taking into account field types and relationships.

## Installation
To install DjPyForms, simply run the following command:

```
pip install DjPyForms
```

## Usage
After installation, you can use DjPyForms directly from the Django command line. Here are some command examples:

But first you need to import DjPyForms into your Django project Settings.py file:

### Generate a Form for Public Part
To generate a form based on a Django model for the public part:

```
python manage.py createform ModelName --app AppName
```

Replace `ModelName` with the name of your Django model and `AppName` with the name of the application containing the model.

### Generate a Form for Administration
To generate a form intended to be used in the Django admin interface:

```
python manage.py createform ModelName --app AppName --for-admin
```

This command will add the model to Django's administration.

### Advanced Options
- To generate an HTML form instead of a Django form:

  ```
  python manage.py createform ModelName --app AppName --type html
  ```

- To specify a custom file extension for the HTML form:

  ```
  python manage.py createform ModelName --app AppName --type html --ext xml
  ```

---

## Features
- Automatic generation of Django or HTML forms from models.
- Updating `views.py` and `urls.py` files.
- Support for forms for both public and admin parts.
- Checking the existence of existing forms with an option to replace.
- Customizable parameters for form generation.

## Contribution
Contributions to the project are welcome. Please review the contribution guidelines before submitting a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.