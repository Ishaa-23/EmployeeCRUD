# openapi-client
Endpoints of CRUD of employee.

This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: 1.0.0
- Package version: 1.0.0
- Build package: org.openapitools.codegen.languages.PythonClientCodegen

## Requirements.

Python 3.7+

## Installation & Usage
### pip install

If the python package is hosted on a repository, you can install directly using:

```sh
pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
```
(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)

Then import the package:
```python
import openapi_client
```

### Setuptools

Install via [Setuptools](http://pypi.python.org/pypi/setuptools).

```sh
python setup.py install --user
```
(or `sudo python setup.py install` to install the package for all users)

Then import the package:
```python
import openapi_client
```

### Tests

Execute `pytest` to run the tests.

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```python

import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5283
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:5283"
)



# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.EmployeeApi(api_client)

    try:
        # Returns all employee.
        api_response = api_instance.api_employee_get()
        print("The response of EmployeeApi->api_employee_get:\n")
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling EmployeeApi->api_employee_get: %s\n" % e)

```

## Documentation for API Endpoints

All URIs are relative to *http://localhost:5283*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*EmployeeApi* | [**api_employee_get**](docs/EmployeeApi.md#api_employee_get) | **GET** /api/Employee | Returns all employee.
*EmployeeApi* | [**api_employee_id_delete**](docs/EmployeeApi.md#api_employee_id_delete) | **DELETE** /api/Employee/{id} | 
*EmployeeApi* | [**api_employee_id_get**](docs/EmployeeApi.md#api_employee_id_get) | **GET** /api/Employee/{id} | Returns employee of given id
*EmployeeApi* | [**api_employee_id_put**](docs/EmployeeApi.md#api_employee_id_put) | **PUT** /api/Employee/{id} | Updates employee details
*EmployeeApi* | [**api_employee_post**](docs/EmployeeApi.md#api_employee_post) | **POST** /api/Employee | Adds new employee


## Documentation For Models

 - [Employee](docs/Employee.md)


<a id="documentation-for-authorization"></a>
## Documentation For Authorization

Endpoints do not require authorization.


## Author




