# \VpnApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**StartLetheand**](VpnApi.md#StartLetheand) | **Get** /letheand/start | 



## StartLetheand

> StartLetheand(ctx).DataDir(dataDir).Version(version).Execute()



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "./openapi"
)

func main() {
    dataDir := "dataDir_example" // string | Returns the binary version
    version := true // bool | Returns the binary version (optional)

    configuration := openapiclient.NewConfiguration()
    api_client := openapiclient.NewAPIClient(configuration)
    resp, r, err := api_client.VpnApi.StartLetheand(context.Background()).DataDir(dataDir).Version(version).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `VpnApi.StartLetheand``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiStartLetheandRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dataDir** | **string** | Returns the binary version | 
 **version** | **bool** | Returns the binary version | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

