# \SearchAPI

All URIs are relative to *https://geosearch.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Autocomplete**](SearchAPI.md#Autocomplete) | **Get** /v1/autocomplete | Autocomplete search
[**ResolveCoordinate**](SearchAPI.md#ResolveCoordinate) | **Get** /v1/resolve | Resolve coordinates to their containing administrative areas
[**ReverseGeocode**](SearchAPI.md#ReverseGeocode) | **Get** /v1/reverse | Reverse geocode coordinates
[**Search**](SearchAPI.md#Search) | **Get** /v1/search | Cross-type search



## Autocomplete

> AutocompleteListResponse Autocomplete(ctx).Q(q).Lang(lang).Limit(limit).Fields(fields).Execute()

Autocomplete search



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/geosearch-dev/geosearch-go"
)

func main() {
	q := "San Fran" // string | Search query (minimum 2 characters)
	lang := "de" // string | ISO 639-1 language code for localized names (e.g., de, fr, ja) (optional)
	limit := int32(10) // int32 | Maximum results to return (1-25, default 10) (optional) (default to 10)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SearchAPI.Autocomplete(context.Background()).Q(q).Lang(lang).Limit(limit).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SearchAPI.Autocomplete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Autocomplete`: AutocompleteListResponse
	fmt.Fprintf(os.Stdout, "Response from `SearchAPI.Autocomplete`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAutocompleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search query (minimum 2 characters) | 
 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **limit** | **int32** | Maximum results to return (1-25, default 10) | [default to 10]
 **fields** | **string** | Comma-separated list of fields to include in the response | 

### Return type

[**AutocompleteListResponse**](AutocompleteListResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ResolveCoordinate

> HierarchyListResponse ResolveCoordinate(ctx).Lat(lat).Lon(lon).Lang(lang).Execute()

Resolve coordinates to their containing administrative areas



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/geosearch-dev/geosearch-go"
)

func main() {
	lat := float64(37.7749) // float64 | Latitude (-90 to 90). Must be a finite number: `NaN` and `Infinity` are rejected with a 400 rather than being passed to the spatial index, which would answer them with an ordinary \"not found\".
	lon := float64(-122.4194) // float64 | Longitude (-180 to 180). Must be a finite number; see `lat`.
	lang := "de" // string | ISO 639-1 language code for localized names (e.g., de, fr, ja) (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SearchAPI.ResolveCoordinate(context.Background()).Lat(lat).Lon(lon).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SearchAPI.ResolveCoordinate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ResolveCoordinate`: HierarchyListResponse
	fmt.Fprintf(os.Stdout, "Response from `SearchAPI.ResolveCoordinate`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiResolveCoordinateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lat** | **float64** | Latitude (-90 to 90). Must be a finite number: &#x60;NaN&#x60; and &#x60;Infinity&#x60; are rejected with a 400 rather than being passed to the spatial index, which would answer them with an ordinary \&quot;not found\&quot;. | 
 **lon** | **float64** | Longitude (-180 to 180). Must be a finite number; see &#x60;lat&#x60;. | 
 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 

### Return type

[**HierarchyListResponse**](HierarchyListResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ReverseGeocode

> ReverseGeocodeSingleResponse ReverseGeocode(ctx).Lat(lat).Lon(lon).Fields(fields).Execute()

Reverse geocode coordinates



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/geosearch-dev/geosearch-go"
)

func main() {
	lat := float64(37.7749) // float64 | Latitude (-90 to 90)
	lon := float64(-122.4194) // float64 | Longitude (-180 to 180)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SearchAPI.ReverseGeocode(context.Background()).Lat(lat).Lon(lon).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SearchAPI.ReverseGeocode``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ReverseGeocode`: ReverseGeocodeSingleResponse
	fmt.Fprintf(os.Stdout, "Response from `SearchAPI.ReverseGeocode`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiReverseGeocodeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lat** | **float64** | Latitude (-90 to 90) | 
 **lon** | **float64** | Longitude (-180 to 180) | 
 **fields** | **string** | Comma-separated list of fields to include in the response | 

### Return type

[**ReverseGeocodeSingleResponse**](ReverseGeocodeSingleResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## Search

> SearchListResponse Search(ctx).Q(q).Lang(lang).Type_(type_).Limit(limit).Fields(fields).Execute()

Cross-type search



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/geosearch-dev/geosearch-go"
)

func main() {
	q := "San Fran" // string | Search query (minimum 2 characters)
	lang := "de" // string | ISO 639-1 language code for localized names (e.g., de, fr, ja) (optional)
	type_ := "city" // string | Filter by entity type (comma-separated). Allowed: country, region, city. (optional)
	limit := int32(10) // int32 | Maximum results to return (1-100, default 25) (optional) (default to 25)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SearchAPI.Search(context.Background()).Q(q).Lang(lang).Type_(type_).Limit(limit).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SearchAPI.Search``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Search`: SearchListResponse
	fmt.Fprintf(os.Stdout, "Response from `SearchAPI.Search`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search query (minimum 2 characters) | 
 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **type_** | **string** | Filter by entity type (comma-separated). Allowed: country, region, city. | 
 **limit** | **int32** | Maximum results to return (1-100, default 25) | [default to 25]
 **fields** | **string** | Comma-separated list of fields to include in the response | 

### Return type

[**SearchListResponse**](SearchListResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

