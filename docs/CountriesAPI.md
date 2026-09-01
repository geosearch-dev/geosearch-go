# \CountriesAPI

All URIs are relative to *https://geosearch.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CountryNeighbors**](CountriesAPI.md#CountryNeighbors) | **Get** /v1/countries/{code}/neighbors | List neighboring countries
[**GetCountry**](CountriesAPI.md#GetCountry) | **Get** /v1/countries/{code} | Get country by ISO code
[**ListCountries**](CountriesAPI.md#ListCountries) | **Get** /v1/countries | List countries
[**ListCountryRegions**](CountriesAPI.md#ListCountryRegions) | **Get** /v1/countries/{code}/regions | List regions in a country



## CountryNeighbors

> CountryListResponse CountryNeighbors(ctx, code).Lang(lang).Fields(fields).Execute()

List neighboring countries



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
	code := "DE" // string | ISO alpha-2 country code
	lang := "de" // string | ISO 639-1 language code for localized names (e.g., de, fr, ja) (optional)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CountriesAPI.CountryNeighbors(context.Background(), code).Lang(lang).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CountriesAPI.CountryNeighbors``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CountryNeighbors`: CountryListResponse
	fmt.Fprintf(os.Stdout, "Response from `CountriesAPI.CountryNeighbors`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**code** | **string** | ISO alpha-2 country code | 

### Other Parameters

Other parameters are passed through a pointer to a apiCountryNeighborsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **fields** | **string** | Comma-separated list of fields to include in the response | 

### Return type

[**CountryListResponse**](CountryListResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetCountry

> CountrySingleResponse GetCountry(ctx, code).Lang(lang).Fields(fields).Execute()

Get country by ISO code



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
	code := "US" // string | ISO alpha-2 country code
	lang := "de" // string | ISO 639-1 language code for localized names (e.g., de, fr, ja) (optional)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CountriesAPI.GetCountry(context.Background(), code).Lang(lang).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CountriesAPI.GetCountry``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetCountry`: CountrySingleResponse
	fmt.Fprintf(os.Stdout, "Response from `CountriesAPI.GetCountry`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**code** | **string** | ISO alpha-2 country code | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetCountryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **fields** | **string** | Comma-separated list of fields to include in the response | 

### Return type

[**CountrySingleResponse**](CountrySingleResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCountries

> CountryListResponse ListCountries(ctx).Lang(lang).Continent(continent).IsoCode(isoCode).PopulationMin(populationMin).PopulationMax(populationMax).Cursor(cursor).Limit(limit).Fields(fields).Sort(sort).Execute()

List countries



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
	continent := "EU" // string | Filter by continent code (AF, AN, AS, EU, NA, OC, SA) (optional)
	isoCode := "US,CA,GB" // string | Filter by ISO alpha-2 codes (comma-separated) (optional)
	populationMin := int64(1000000) // int64 | Minimum population filter (optional)
	populationMax := int64(10000000) // int64 | Maximum population filter (optional)
	cursor := "eyJpZCI6MjV9" // string | Pagination cursor from a previous response (optional)
	limit := int32(25) // int32 | Number of results per page (1-100, default 25) (optional) (default to 25)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)
	sort := "-population" // string | Sort field and direction. Allowed: name, population, area_sq_km. Prefix with - for descending. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CountriesAPI.ListCountries(context.Background()).Lang(lang).Continent(continent).IsoCode(isoCode).PopulationMin(populationMin).PopulationMax(populationMax).Cursor(cursor).Limit(limit).Fields(fields).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CountriesAPI.ListCountries``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCountries`: CountryListResponse
	fmt.Fprintf(os.Stdout, "Response from `CountriesAPI.ListCountries`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListCountriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **continent** | **string** | Filter by continent code (AF, AN, AS, EU, NA, OC, SA) | 
 **isoCode** | **string** | Filter by ISO alpha-2 codes (comma-separated) | 
 **populationMin** | **int64** | Minimum population filter | 
 **populationMax** | **int64** | Maximum population filter | 
 **cursor** | **string** | Pagination cursor from a previous response | 
 **limit** | **int32** | Number of results per page (1-100, default 25) | [default to 25]
 **fields** | **string** | Comma-separated list of fields to include in the response | 
 **sort** | **string** | Sort field and direction. Allowed: name, population, area_sq_km. Prefix with - for descending. | 

### Return type

[**CountryListResponse**](CountryListResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCountryRegions

> RegionListResponse ListCountryRegions(ctx, code).Lang(lang).Cursor(cursor).Limit(limit).Fields(fields).Sort(sort).Execute()

List regions in a country



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
	code := "US" // string | ISO alpha-2 country code
	lang := "de" // string | ISO 639-1 language code for localized names (e.g., de, fr, ja) (optional)
	cursor := "eyJpZCI6MjV9" // string | Pagination cursor from a previous response (optional)
	limit := int32(25) // int32 | Number of results per page (1-100, default 25) (optional) (default to 25)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)
	sort := "name" // string | Sort field. Allowed: name, population. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CountriesAPI.ListCountryRegions(context.Background(), code).Lang(lang).Cursor(cursor).Limit(limit).Fields(fields).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CountriesAPI.ListCountryRegions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCountryRegions`: RegionListResponse
	fmt.Fprintf(os.Stdout, "Response from `CountriesAPI.ListCountryRegions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**code** | **string** | ISO alpha-2 country code | 

### Other Parameters

Other parameters are passed through a pointer to a apiListCountryRegionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
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

