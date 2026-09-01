# \IPGeolocationAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**LookupIP**](IPGeolocationAPI.md#LookupIP) | **Get** /v1/ip/{address} | IP geolocation lookup
[**LookupMyIP**](IPGeolocationAPI.md#LookupMyIP) | **Get** /v1/ip/me | Caller&#39;s IP geolocation



## LookupIP

> IPSingleResponse LookupIP(ctx, address).Lang(lang).Fields(fields).Execute()

IP geolocation lookup



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/geosearch-dev/geoapi-go"
)

func main() {
	address := "8.8.8.8" // string | IPv4 or IPv6 address
	lang := "de" // string | ISO 639-1 language code for localized names (e.g., de, fr, ja) (optional)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IPGeolocationAPI.LookupIP(context.Background(), address).Lang(lang).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IPGeolocationAPI.LookupIP``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LookupIP`: IPSingleResponse
	fmt.Fprintf(os.Stdout, "Response from `IPGeolocationAPI.LookupIP`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**address** | **string** | IPv4 or IPv6 address | 

### Other Parameters

Other parameters are passed through a pointer to a apiLookupIPRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **fields** | **string** | Comma-separated list of fields to include in the response | 

### Return type

[**IPSingleResponse**](IPSingleResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## LookupMyIP

> IPSingleResponse LookupMyIP(ctx).Lang(lang).Fields(fields).Execute()

Caller's IP geolocation



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/geosearch-dev/geoapi-go"
)

func main() {
	lang := "de" // string | ISO 639-1 language code for localized names (e.g., de, fr, ja) (optional)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IPGeolocationAPI.LookupMyIP(context.Background()).Lang(lang).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IPGeolocationAPI.LookupMyIP``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LookupMyIP`: IPSingleResponse
	fmt.Fprintf(os.Stdout, "Response from `IPGeolocationAPI.LookupMyIP`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiLookupMyIPRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **fields** | **string** | Comma-separated list of fields to include in the response | 

### Return type

[**IPSingleResponse**](IPSingleResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

