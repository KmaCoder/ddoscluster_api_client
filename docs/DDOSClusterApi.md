# swagger_client.DDOSClusterApi

All URIs are relative to *https://api.ddoscluster.in.ua/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**d_dos_get_active_tasks**](DDOSClusterApi.md#d_dos_get_active_tasks) | **GET** /active-tasks | 
[**d_dos_get_active_workers**](DDOSClusterApi.md#d_dos_get_active_workers) | **GET** /active-workers | 
[**d_dos_get_damage_stats**](DDOSClusterApi.md#d_dos_get_damage_stats) | **GET** /damage-stats | 
[**d_dos_upsert_worker**](DDOSClusterApi.md#d_dos_upsert_worker) | **POST** /submit-progress | 

# **d_dos_get_active_tasks**
> list[str] d_dos_get_active_tasks()



### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.DDOSClusterApi()

try:
    api_response = api_instance.d_dos_get_active_tasks()
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DDOSClusterApi->d_dos_get_active_tasks: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

**list[str]**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **d_dos_get_active_workers**
> list[DDOSWorker] d_dos_get_active_workers(minutes_interval=minutes_interval)



### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.DDOSClusterApi()
minutes_interval = 1.2 # float |  (optional)

try:
    api_response = api_instance.d_dos_get_active_workers(minutes_interval=minutes_interval)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DDOSClusterApi->d_dos_get_active_workers: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **minutes_interval** | **float**|  | [optional] 

### Return type

[**list[DDOSWorker]**](DDOSWorker.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **d_dos_get_damage_stats**
> list[DDOSTaskDTO] d_dos_get_damage_stats(minutes_interval=minutes_interval)



### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.DDOSClusterApi()
minutes_interval = 1.2 # float |  (optional)

try:
    api_response = api_instance.d_dos_get_damage_stats(minutes_interval=minutes_interval)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DDOSClusterApi->d_dos_get_damage_stats: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **minutes_interval** | **float**|  | [optional] 

### Return type

[**list[DDOSTaskDTO]**](DDOSTaskDTO.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **d_dos_upsert_worker**
> DDOSWorker d_dos_upsert_worker(body)



### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.DDOSClusterApi()
body = swagger_client.DDOSWorkerDTO() # DDOSWorkerDTO | 

try:
    api_response = api_instance.d_dos_upsert_worker(body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DDOSClusterApi->d_dos_upsert_worker: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DDOSWorkerDTO**](DDOSWorkerDTO.md)|  | 

### Return type

[**DDOSWorker**](DDOSWorker.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

