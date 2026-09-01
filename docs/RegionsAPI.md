# \RegionsAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetRegion**](RegionsAPI.md#GetRegion) | **Get** /v1/regions/{id} | Get region by ID
[**ListRegionCities**](RegionsAPI.md#ListRegionCities) | **Get** /v1/regions/{id}/cities | List cities in a region
[**ListRegions**](RegionsAPI.md#ListRegions) | **Get** /v1/regions | List regions
[**RegionChildren**](RegionsAPI.md#RegionChildren) | **Get** /v1/regions/{id}/children | List child cities of a region



## GetRegion

> RegionSingleResponse GetRegion(ctx, id).Lang(lang).Fields(fields).Execute()

Get region by ID



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
	id := int64(5332921) // int64 | Region ID
	lang := "de" // string | ISO 639-1 language code for localized names (e.g., de, fr, ja) (optional)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RegionsAPI.GetRegion(context.Background(), id).Lang(lang).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RegionsAPI.GetRegion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetRegion`: RegionSingleResponse
	fmt.Fprintf(os.Stdout, "Response from `RegionsAPI.GetRegion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int64** | Region ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetRegionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **fields** | **string** | Comma-separated list of fields to include in the response | 

### Return type

[**RegionSingleResponse**](RegionSingleResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListRegionCities

> CityListResponse ListRegionCities(ctx, id).Lang(lang).Cursor(cursor).Limit(limit).Fields(fields).Sort(sort).Execute()

List cities in a region



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
	id := int64(5332921) // int64 | Region ID
	lang := "de" // string | ISO 639-1 language code for localized names (e.g., de, fr, ja) (optional)
	cursor := "eyJpZCI6MjV9" // string | Pagination cursor from a previous response (optional)
	limit := int32(25) // int32 | Number of results per page (1-100, default 25) (optional) (default to 25)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)
	sort := "-population" // string | Sort field. Allowed: name, population. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RegionsAPI.ListRegionCities(context.Background(), id).Lang(lang).Cursor(cursor).Limit(limit).Fields(fields).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RegionsAPI.ListRegionCities``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListRegionCities`: CityListResponse
	fmt.Fprintf(os.Stdout, "Response from `RegionsAPI.ListRegionCities`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int64** | Region ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiListRegionCitiesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **cursor** | **string** | Pagination cursor from a previous response | 
 **limit** | **int32** | Number of results per page (1-100, default 25) | [default to 25]
 **fields** | **string** | Comma-separated list of fields to include in the response | 
 **sort** | **string** | Sort field. Allowed: name, population. | 

### Return type

[**CityListResponse**](CityListResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListRegions

> RegionListResponse ListRegions(ctx).Lang(lang).Country(country).Level(level).PopulationMin(populationMin).PopulationMax(populationMax).Cursor(cursor).Limit(limit).Fields(fields).Sort(sort).Execute()

List regions



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
	level := int32(1) // int32 | Filter by administrative level (optional)
	populationMin := int64(1000000) // int64 | Minimum population filter (optional)
	populationMax := int64(10000000) // int64 | Maximum population filter (optional)
	cursor := "eyJpZCI6MjV9" // string | Pagination cursor from a previous response (optional)
	limit := int32(25) // int32 | Number of results per page (1-100, default 25) (optional) (default to 25)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)
	sort := "-population" // string | Sort field. Allowed: name, population. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RegionsAPI.ListRegions(context.Background()).Lang(lang).Country(country).Level(level).PopulationMin(populationMin).PopulationMax(populationMax).Cursor(cursor).Limit(limit).Fields(fields).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RegionsAPI.ListRegions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListRegions`: RegionListResponse
	fmt.Fprintf(os.Stdout, "Response from `RegionsAPI.ListRegions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListRegionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **country** | **string** | Filter by ISO alpha-2 country code | 
 **level** | **int32** | Filter by administrative level | 
 **populationMin** | **int64** | Minimum population filter | 
 **populationMax** | **int64** | Maximum population filter | 
 **cursor** | **string** | Pagination cursor from a previous response | 
 **limit** | **int32** | Number of results per page (1-100, default 25) | [default to 25]
 **fields** | **string** | Comma-separated list of fields to include in the response | 
 **sort** | **string** | Sort field. Allowed: name, population. | 

### Return type

[**RegionListResponse**](RegionListResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RegionChildren

> CityListResponse RegionChildren(ctx, id).Lang(lang).Fields(fields).Execute()

List child cities of a region



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
	id := int64(5332921) // int64 | Region ID
	lang := "de" // string | ISO 639-1 language code for localized names (e.g., de, fr, ja) (optional)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RegionsAPI.RegionChildren(context.Background(), id).Lang(lang).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RegionsAPI.RegionChildren``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RegionChildren`: CityListResponse
	fmt.Fprintf(os.Stdout, "Response from `RegionsAPI.RegionChildren`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int64** | Region ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiRegionChildrenRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **fields** | **string** | Comma-separated list of fields to include in the response | 

### Return type

[**CityListResponse**](CityListResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

