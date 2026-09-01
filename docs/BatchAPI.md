# \BatchAPI

All URIs are relative to *https://geosearch.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**BatchCities**](BatchAPI.md#BatchCities) | **Post** /v1/batch/cities | Batch lookup cities by IDs
[**BatchCountries**](BatchAPI.md#BatchCountries) | **Post** /v1/batch/countries | Batch lookup countries by IDs
[**BatchRegions**](BatchAPI.md#BatchRegions) | **Post** /v1/batch/regions | Batch lookup regions by IDs



## BatchCities

> CityListResponse BatchCities(ctx).BatchRequest(batchRequest).Lang(lang).Fields(fields).Execute()

Batch lookup cities by IDs



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
	batchRequest := *openapiclient.NewBatchRequest([]int64{int64(123)}) // BatchRequest | 
	lang := "de" // string | ISO 639-1 language code for localized names (e.g., de, fr, ja) (optional)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BatchAPI.BatchCities(context.Background()).BatchRequest(batchRequest).Lang(lang).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BatchAPI.BatchCities``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BatchCities`: CityListResponse
	fmt.Fprintf(os.Stdout, "Response from `BatchAPI.BatchCities`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBatchCitiesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **batchRequest** | [**BatchRequest**](BatchRequest.md) |  | 
 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **fields** | **string** | Comma-separated list of fields to include in the response | 

### Return type

[**CityListResponse**](CityListResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BatchCountries

> CountryListResponse BatchCountries(ctx).BatchRequest(batchRequest).Lang(lang).Fields(fields).Execute()

Batch lookup countries by IDs



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
	batchRequest := *openapiclient.NewBatchRequest([]int64{int64(123)}) // BatchRequest | 
	lang := "de" // string | ISO 639-1 language code for localized names (e.g., de, fr, ja) (optional)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BatchAPI.BatchCountries(context.Background()).BatchRequest(batchRequest).Lang(lang).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BatchAPI.BatchCountries``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BatchCountries`: CountryListResponse
	fmt.Fprintf(os.Stdout, "Response from `BatchAPI.BatchCountries`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBatchCountriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **batchRequest** | [**BatchRequest**](BatchRequest.md) |  | 
 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **fields** | **string** | Comma-separated list of fields to include in the response | 

### Return type

[**CountryListResponse**](CountryListResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BatchRegions

> RegionListResponse BatchRegions(ctx).BatchRequest(batchRequest).Lang(lang).Fields(fields).Execute()

Batch lookup regions by IDs



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
	batchRequest := *openapiclient.NewBatchRequest([]int64{int64(123)}) // BatchRequest | 
	lang := "de" // string | ISO 639-1 language code for localized names (e.g., de, fr, ja) (optional)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BatchAPI.BatchRegions(context.Background()).BatchRequest(batchRequest).Lang(lang).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BatchAPI.BatchRegions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BatchRegions`: RegionListResponse
	fmt.Fprintf(os.Stdout, "Response from `BatchAPI.BatchRegions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBatchRegionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **batchRequest** | [**BatchRequest**](BatchRequest.md) |  | 
 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **fields** | **string** | Comma-separated list of fields to include in the response | 

### Return type

[**RegionListResponse**](RegionListResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

