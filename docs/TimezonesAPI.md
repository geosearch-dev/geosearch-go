# \TimezonesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetTimezone**](TimezonesAPI.md#GetTimezone) | **Get** /v1/timezones/{tzId} | Get timezone by IANA ID
[**ListTimezones**](TimezonesAPI.md#ListTimezones) | **Get** /v1/timezones | List timezones



## GetTimezone

> TimezoneSingleResponse GetTimezone(ctx, tzId).Lang(lang).Fields(fields).Execute()

Get timezone by IANA ID



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
	tzId := "America/New_York" // string | IANA timezone ID (e.g., America/New_York)
	lang := "de" // string | ISO 639-1 language code for localized names (e.g., de, fr, ja) (optional)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TimezonesAPI.GetTimezone(context.Background(), tzId).Lang(lang).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TimezonesAPI.GetTimezone``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTimezone`: TimezoneSingleResponse
	fmt.Fprintf(os.Stdout, "Response from `TimezonesAPI.GetTimezone`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tzId** | **string** | IANA timezone ID (e.g., America/New_York) | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTimezoneRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **fields** | **string** | Comma-separated list of fields to include in the response | 

### Return type

[**TimezoneSingleResponse**](TimezoneSingleResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListTimezones

> TimezoneListResponse ListTimezones(ctx).Lang(lang).Country(country).Cursor(cursor).Limit(limit).Fields(fields).Sort(sort).Execute()

List timezones



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
	country := "US" // string | Filter by ISO alpha-2 country code (optional)
	cursor := "eyJpZCI6MjV9" // string | Pagination cursor from a previous response (optional)
	limit := int32(25) // int32 | Number of results per page (1-100, default 25) (optional) (default to 25)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)
	sort := "gmt_offset" // string | Sort field. Allowed: timezone_id, gmt_offset, country_code. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TimezonesAPI.ListTimezones(context.Background()).Lang(lang).Country(country).Cursor(cursor).Limit(limit).Fields(fields).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TimezonesAPI.ListTimezones``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTimezones`: TimezoneListResponse
	fmt.Fprintf(os.Stdout, "Response from `TimezonesAPI.ListTimezones`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListTimezonesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **country** | **string** | Filter by ISO alpha-2 country code | 
 **cursor** | **string** | Pagination cursor from a previous response | 
 **limit** | **int32** | Number of results per page (1-100, default 25) | [default to 25]
 **fields** | **string** | Comma-separated list of fields to include in the response | 
 **sort** | **string** | Sort field. Allowed: timezone_id, gmt_offset, country_code. | 

### Return type

[**TimezoneListResponse**](TimezoneListResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

