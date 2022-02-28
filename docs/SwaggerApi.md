# swagger_client.SwaggerApi

All URIs are relative to *https://api.ddoscluster.in.ua/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**swagger_get_json**](SwaggerApi.md#swagger_get_json) | **GET** /swagger/json | 
[**swagger_get_ui**](SwaggerApi.md#swagger_get_ui) | **GET** /swagger | 

# **swagger_get_json**
> object swagger_get_json()



### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.SwaggerApi()

try:
    api_response = api_instance.swagger_get_json()
    pprint(api_response)
except ApiException as e:
    print("Exception when calling SwaggerApi->swagger_get_json: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **swagger_get_ui**
> str swagger_get_ui()



### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.SwaggerApi()

try:
    api_response = api_instance.swagger_get_ui()
    pprint(api_response)
except ApiException as e:
    print("Exception when calling SwaggerApi->swagger_get_ui: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

**str**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/html

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

