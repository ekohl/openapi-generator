<a name="__pageTop"></a>
# unit_test_api.apis.tags.one_of_api.OneOfApi

All URIs are relative to *https://someserver.com/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**post_nested_oneof_to_check_validation_semantics_request_body**](#post_nested_oneof_to_check_validation_semantics_request_body) | **post** /requestBody/postNestedOneofToCheckValidationSemanticsRequestBody | 
[**post_nested_oneof_to_check_validation_semantics_response_body_for_content_types**](#post_nested_oneof_to_check_validation_semantics_response_body_for_content_types) | **post** /responseBody/postNestedOneofToCheckValidationSemanticsResponseBodyForContentTypes | 
[**post_oneof_complex_types_request_body**](#post_oneof_complex_types_request_body) | **post** /requestBody/postOneofComplexTypesRequestBody | 
[**post_oneof_complex_types_response_body_for_content_types**](#post_oneof_complex_types_response_body_for_content_types) | **post** /responseBody/postOneofComplexTypesResponseBodyForContentTypes | 
[**post_oneof_request_body**](#post_oneof_request_body) | **post** /requestBody/postOneofRequestBody | 
[**post_oneof_response_body_for_content_types**](#post_oneof_response_body_for_content_types) | **post** /responseBody/postOneofResponseBodyForContentTypes | 
[**post_oneof_with_base_schema_request_body**](#post_oneof_with_base_schema_request_body) | **post** /requestBody/postOneofWithBaseSchemaRequestBody | 
[**post_oneof_with_base_schema_response_body_for_content_types**](#post_oneof_with_base_schema_response_body_for_content_types) | **post** /responseBody/postOneofWithBaseSchemaResponseBodyForContentTypes | 
[**post_oneof_with_empty_schema_request_body**](#post_oneof_with_empty_schema_request_body) | **post** /requestBody/postOneofWithEmptySchemaRequestBody | 
[**post_oneof_with_empty_schema_response_body_for_content_types**](#post_oneof_with_empty_schema_response_body_for_content_types) | **post** /responseBody/postOneofWithEmptySchemaResponseBodyForContentTypes | 

# **post_nested_oneof_to_check_validation_semantics_request_body**
<a name="post_nested_oneof_to_check_validation_semantics_request_body"></a>
> post_nested_oneof_to_check_validation_semantics_request_body(nested_oneof_to_check_validation_semantics)



### Example

```python
import unit_test_api
from unit_test_api.apis.tags import one_of_api
from unit_test_api.model.nested_oneof_to_check_validation_semantics import NestedOneofToCheckValidationSemantics
from pprint import pprint
# Defining the host is optional and defaults to https://someserver.com/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = unit_test_api.Configuration(
    host = "https://someserver.com/v1"
)

# Enter a context with an instance of the API client
with unit_test_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = one_of_api.OneOfApi(api_client)

    # example passing only required values which don't have defaults set
    body = NestedOneofToCheckValidationSemantics(None)
    try:
        api_response = api_instance.post_nested_oneof_to_check_validation_semantics_request_body(
            body=body,
        )
    except unit_test_api.ApiException as e:
        print("Exception when calling OneOfApi->post_nested_oneof_to_check_validation_semantics_request_body: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
body | typing.Union[SchemaForRequestBodyApplicationJson] | required |
content_type | str | optional, default is 'application/json' | Selects the schema and serialization of the request body
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### body

#### SchemaForRequestBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**NestedOneofToCheckValidationSemantics**](NestedOneofToCheckValidationSemantics.md) |  | 


### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | ApiResponseFor200 | success

#### ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | Unset | body was not defined |
headers | Unset | headers were not defined |


void (empty response body)

### Authorization

No authorization required

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **post_nested_oneof_to_check_validation_semantics_response_body_for_content_types**
<a name="post_nested_oneof_to_check_validation_semantics_response_body_for_content_types"></a>
> NestedOneofToCheckValidationSemantics post_nested_oneof_to_check_validation_semantics_response_body_for_content_types()



### Example

```python
import unit_test_api
from unit_test_api.apis.tags import one_of_api
from unit_test_api.model.nested_oneof_to_check_validation_semantics import NestedOneofToCheckValidationSemantics
from pprint import pprint
# Defining the host is optional and defaults to https://someserver.com/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = unit_test_api.Configuration(
    host = "https://someserver.com/v1"
)

# Enter a context with an instance of the API client
with unit_test_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = one_of_api.OneOfApi(api_client)

    # example, this endpoint has no required or optional parameters
    try:
        api_response = api_instance.post_nested_oneof_to_check_validation_semantics_response_body_for_content_types()
        pprint(api_response)
    except unit_test_api.ApiException as e:
        print("Exception when calling OneOfApi->post_nested_oneof_to_check_validation_semantics_response_body_for_content_types: %s\n" % e)
```
### Parameters
This endpoint does not need any parameter.

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | ApiResponseFor200 | success

#### ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, ] |  |
headers | Unset | headers were not defined |

#### SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**NestedOneofToCheckValidationSemantics**](NestedOneofToCheckValidationSemantics.md) |  | 



[**NestedOneofToCheckValidationSemantics**](NestedOneofToCheckValidationSemantics.md)

### Authorization

No authorization required

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **post_oneof_complex_types_request_body**
<a name="post_oneof_complex_types_request_body"></a>
> post_oneof_complex_types_request_body(oneof_complex_types)



### Example

```python
import unit_test_api
from unit_test_api.apis.tags import one_of_api
from unit_test_api.model.oneof_complex_types import OneofComplexTypes
from pprint import pprint
# Defining the host is optional and defaults to https://someserver.com/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = unit_test_api.Configuration(
    host = "https://someserver.com/v1"
)

# Enter a context with an instance of the API client
with unit_test_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = one_of_api.OneOfApi(api_client)

    # example passing only required values which don't have defaults set
    body = OneofComplexTypes(None)
    try:
        api_response = api_instance.post_oneof_complex_types_request_body(
            body=body,
        )
    except unit_test_api.ApiException as e:
        print("Exception when calling OneOfApi->post_oneof_complex_types_request_body: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
body | typing.Union[SchemaForRequestBodyApplicationJson] | required |
content_type | str | optional, default is 'application/json' | Selects the schema and serialization of the request body
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### body

#### SchemaForRequestBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**OneofComplexTypes**](OneofComplexTypes.md) |  | 


### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | ApiResponseFor200 | success

#### ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | Unset | body was not defined |
headers | Unset | headers were not defined |


void (empty response body)

### Authorization

No authorization required

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **post_oneof_complex_types_response_body_for_content_types**
<a name="post_oneof_complex_types_response_body_for_content_types"></a>
> OneofComplexTypes post_oneof_complex_types_response_body_for_content_types()



### Example

```python
import unit_test_api
from unit_test_api.apis.tags import one_of_api
from unit_test_api.model.oneof_complex_types import OneofComplexTypes
from pprint import pprint
# Defining the host is optional and defaults to https://someserver.com/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = unit_test_api.Configuration(
    host = "https://someserver.com/v1"
)

# Enter a context with an instance of the API client
with unit_test_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = one_of_api.OneOfApi(api_client)

    # example, this endpoint has no required or optional parameters
    try:
        api_response = api_instance.post_oneof_complex_types_response_body_for_content_types()
        pprint(api_response)
    except unit_test_api.ApiException as e:
        print("Exception when calling OneOfApi->post_oneof_complex_types_response_body_for_content_types: %s\n" % e)
```
### Parameters
This endpoint does not need any parameter.

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | ApiResponseFor200 | success

#### ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, ] |  |
headers | Unset | headers were not defined |

#### SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**OneofComplexTypes**](OneofComplexTypes.md) |  | 



[**OneofComplexTypes**](OneofComplexTypes.md)

### Authorization

No authorization required

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **post_oneof_request_body**
<a name="post_oneof_request_body"></a>
> post_oneof_request_body(oneof)



### Example

```python
import unit_test_api
from unit_test_api.apis.tags import one_of_api
from unit_test_api.model.oneof import Oneof
from pprint import pprint
# Defining the host is optional and defaults to https://someserver.com/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = unit_test_api.Configuration(
    host = "https://someserver.com/v1"
)

# Enter a context with an instance of the API client
with unit_test_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = one_of_api.OneOfApi(api_client)

    # example passing only required values which don't have defaults set
    body = Oneof(None)
    try:
        api_response = api_instance.post_oneof_request_body(
            body=body,
        )
    except unit_test_api.ApiException as e:
        print("Exception when calling OneOfApi->post_oneof_request_body: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
body | typing.Union[SchemaForRequestBodyApplicationJson] | required |
content_type | str | optional, default is 'application/json' | Selects the schema and serialization of the request body
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### body

#### SchemaForRequestBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**Oneof**](Oneof.md) |  | 


### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | ApiResponseFor200 | success

#### ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | Unset | body was not defined |
headers | Unset | headers were not defined |


void (empty response body)

### Authorization

No authorization required

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **post_oneof_response_body_for_content_types**
<a name="post_oneof_response_body_for_content_types"></a>
> Oneof post_oneof_response_body_for_content_types()



### Example

```python
import unit_test_api
from unit_test_api.apis.tags import one_of_api
from unit_test_api.model.oneof import Oneof
from pprint import pprint
# Defining the host is optional and defaults to https://someserver.com/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = unit_test_api.Configuration(
    host = "https://someserver.com/v1"
)

# Enter a context with an instance of the API client
with unit_test_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = one_of_api.OneOfApi(api_client)

    # example, this endpoint has no required or optional parameters
    try:
        api_response = api_instance.post_oneof_response_body_for_content_types()
        pprint(api_response)
    except unit_test_api.ApiException as e:
        print("Exception when calling OneOfApi->post_oneof_response_body_for_content_types: %s\n" % e)
```
### Parameters
This endpoint does not need any parameter.

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | ApiResponseFor200 | success

#### ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, ] |  |
headers | Unset | headers were not defined |

#### SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**Oneof**](Oneof.md) |  | 



[**Oneof**](Oneof.md)

### Authorization

No authorization required

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **post_oneof_with_base_schema_request_body**
<a name="post_oneof_with_base_schema_request_body"></a>
> post_oneof_with_base_schema_request_body(body)



### Example

```python
import unit_test_api
from unit_test_api.apis.tags import one_of_api
from unit_test_api.model.oneof_with_base_schema import OneofWithBaseSchema
from pprint import pprint
# Defining the host is optional and defaults to https://someserver.com/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = unit_test_api.Configuration(
    host = "https://someserver.com/v1"
)

# Enter a context with an instance of the API client
with unit_test_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = one_of_api.OneOfApi(api_client)

    # example passing only required values which don't have defaults set
    body = OneofWithBaseSchema("body_example")
    try:
        api_response = api_instance.post_oneof_with_base_schema_request_body(
            body=body,
        )
    except unit_test_api.ApiException as e:
        print("Exception when calling OneOfApi->post_oneof_with_base_schema_request_body: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
body | typing.Union[SchemaForRequestBodyApplicationJson] | required |
content_type | str | optional, default is 'application/json' | Selects the schema and serialization of the request body
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### body

#### SchemaForRequestBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**OneofWithBaseSchema**](OneofWithBaseSchema.md) |  | 


### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | ApiResponseFor200 | success

#### ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | Unset | body was not defined |
headers | Unset | headers were not defined |


void (empty response body)

### Authorization

No authorization required

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **post_oneof_with_base_schema_response_body_for_content_types**
<a name="post_oneof_with_base_schema_response_body_for_content_types"></a>
> OneofWithBaseSchema post_oneof_with_base_schema_response_body_for_content_types()



### Example

```python
import unit_test_api
from unit_test_api.apis.tags import one_of_api
from unit_test_api.model.oneof_with_base_schema import OneofWithBaseSchema
from pprint import pprint
# Defining the host is optional and defaults to https://someserver.com/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = unit_test_api.Configuration(
    host = "https://someserver.com/v1"
)

# Enter a context with an instance of the API client
with unit_test_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = one_of_api.OneOfApi(api_client)

    # example, this endpoint has no required or optional parameters
    try:
        api_response = api_instance.post_oneof_with_base_schema_response_body_for_content_types()
        pprint(api_response)
    except unit_test_api.ApiException as e:
        print("Exception when calling OneOfApi->post_oneof_with_base_schema_response_body_for_content_types: %s\n" % e)
```
### Parameters
This endpoint does not need any parameter.

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | ApiResponseFor200 | success

#### ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, ] |  |
headers | Unset | headers were not defined |

#### SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**OneofWithBaseSchema**](OneofWithBaseSchema.md) |  | 



[**OneofWithBaseSchema**](OneofWithBaseSchema.md)

### Authorization

No authorization required

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **post_oneof_with_empty_schema_request_body**
<a name="post_oneof_with_empty_schema_request_body"></a>
> post_oneof_with_empty_schema_request_body(oneof_with_empty_schema)



### Example

```python
import unit_test_api
from unit_test_api.apis.tags import one_of_api
from unit_test_api.model.oneof_with_empty_schema import OneofWithEmptySchema
from pprint import pprint
# Defining the host is optional and defaults to https://someserver.com/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = unit_test_api.Configuration(
    host = "https://someserver.com/v1"
)

# Enter a context with an instance of the API client
with unit_test_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = one_of_api.OneOfApi(api_client)

    # example passing only required values which don't have defaults set
    body = OneofWithEmptySchema(None)
    try:
        api_response = api_instance.post_oneof_with_empty_schema_request_body(
            body=body,
        )
    except unit_test_api.ApiException as e:
        print("Exception when calling OneOfApi->post_oneof_with_empty_schema_request_body: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
body | typing.Union[SchemaForRequestBodyApplicationJson] | required |
content_type | str | optional, default is 'application/json' | Selects the schema and serialization of the request body
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### body

#### SchemaForRequestBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**OneofWithEmptySchema**](OneofWithEmptySchema.md) |  | 


### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | ApiResponseFor200 | success

#### ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | Unset | body was not defined |
headers | Unset | headers were not defined |


void (empty response body)

### Authorization

No authorization required

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **post_oneof_with_empty_schema_response_body_for_content_types**
<a name="post_oneof_with_empty_schema_response_body_for_content_types"></a>
> OneofWithEmptySchema post_oneof_with_empty_schema_response_body_for_content_types()



### Example

```python
import unit_test_api
from unit_test_api.apis.tags import one_of_api
from unit_test_api.model.oneof_with_empty_schema import OneofWithEmptySchema
from pprint import pprint
# Defining the host is optional and defaults to https://someserver.com/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = unit_test_api.Configuration(
    host = "https://someserver.com/v1"
)

# Enter a context with an instance of the API client
with unit_test_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = one_of_api.OneOfApi(api_client)

    # example, this endpoint has no required or optional parameters
    try:
        api_response = api_instance.post_oneof_with_empty_schema_response_body_for_content_types()
        pprint(api_response)
    except unit_test_api.ApiException as e:
        print("Exception when calling OneOfApi->post_oneof_with_empty_schema_response_body_for_content_types: %s\n" % e)
```
### Parameters
This endpoint does not need any parameter.

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | ApiResponseFor200 | success

#### ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, ] |  |
headers | Unset | headers were not defined |

#### SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**OneofWithEmptySchema**](OneofWithEmptySchema.md) |  | 



[**OneofWithEmptySchema**](OneofWithEmptySchema.md)

### Authorization

No authorization required

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

