# openapi_client.EmployeeApi

All URIs are relative to *http://localhost:5283*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_employee_get**](EmployeeApi.md#api_employee_get) | **GET** /api/Employee | Returns all employee.
[**api_employee_id_delete**](EmployeeApi.md#api_employee_id_delete) | **DELETE** /api/Employee/{id} | 
[**api_employee_id_get**](EmployeeApi.md#api_employee_id_get) | **GET** /api/Employee/{id} | Returns employee of given id
[**api_employee_id_put**](EmployeeApi.md#api_employee_id_put) | **PUT** /api/Employee/{id} | Updates employee details
[**api_employee_post**](EmployeeApi.md#api_employee_post) | **POST** /api/Employee | Adds new employee


# **api_employee_get**
> Employee api_employee_get()

Returns all employee.

### Example

```python
import time
import os
import openapi_client
from openapi_client.models.employee import Employee
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
    except Exception as e:
        print("Exception when calling EmployeeApi->api_employee_get: %s\n" % e)
```



### Parameters
This endpoint does not need any parameter.

### Return type

[**Employee**](Employee.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_employee_id_delete**
> List[Employee] api_employee_id_delete(id)



### Example

```python
import time
import os
import openapi_client
from openapi_client.models.employee import Employee
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
    id = 56 # int | 

    try:
        api_response = api_instance.api_employee_id_delete(id)
        print("The response of EmployeeApi->api_employee_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmployeeApi->api_employee_id_delete: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 

### Return type

[**List[Employee]**](Employee.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_employee_id_get**
> Employee api_employee_id_get(id)

Returns employee of given id

### Example

```python
import time
import os
import openapi_client
from openapi_client.models.employee import Employee
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
    id = 56 # int | 

    try:
        # Returns employee of given id
        api_response = api_instance.api_employee_id_get(id)
        print("The response of EmployeeApi->api_employee_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmployeeApi->api_employee_id_get: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 

### Return type

[**Employee**](Employee.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_employee_id_put**
> Employee api_employee_id_put(id)

Updates employee details

### Example

```python
import time
import os
import openapi_client
from openapi_client.models.employee import Employee
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
    id = 56 # int | 

    try:
        # Updates employee details
        api_response = api_instance.api_employee_id_put(id)
        print("The response of EmployeeApi->api_employee_id_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmployeeApi->api_employee_id_put: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 

### Return type

[**Employee**](Employee.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_employee_post**
> List[Employee] api_employee_post(employee=employee)

Adds new employee

### Example

```python
import time
import os
import openapi_client
from openapi_client.models.employee import Employee
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
    employee = openapi_client.Employee() # Employee |  (optional)

    try:
        # Adds new employee
        api_response = api_instance.api_employee_post(employee=employee)
        print("The response of EmployeeApi->api_employee_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmployeeApi->api_employee_post: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **employee** | [**Employee**](Employee.md)|  | [optional] 

### Return type

[**List[Employee]**](Employee.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

