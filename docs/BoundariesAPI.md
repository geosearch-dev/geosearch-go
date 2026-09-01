# \BoundariesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetBoundary**](BoundariesAPI.md#GetBoundary) | **Get** /v1/boundaries/{geoname_id} | Fetch an area&#39;s boundary polygon as GeoJSON



## GetBoundary

> BoundarySingleResponse GetBoundary(ctx, geonameId).Simplify(simplify).Lang(lang).Execute()

Fetch an area's boundary polygon as GeoJSON



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
	geonameId := int64(6252001) // int64 | GeoNames id of a country or a region. A city id — or any id that does not name an area — is a 404 `area_not_an_area`, not a 400.
	simplify := float64(0.01) // float64 | Douglas-Peucker tolerance in EPSG:4326 DEGREES, applied before the polygon is serialised. Omit it for full precision.  DEGREES, NOT METRES. The upper bound of 10 is roughly 1,100 km, chosen to make the unit obviously wrong to anyone who typed a value in metres. Simplification stops changing the shape above about 1 degree, so values beyond that buy nothing.  `0` is accepted and is a no-op: the response reports `simplify: null`, because no tolerance was actually applied.  A negative, non-finite or out-of-range value is a 422, never a 500.  SUPPLY IT AT MOST ONCE. `?simplify=0.01&simplify=0.5` is a 422 rather than a request served with one of the two values silently dropped: two tolerances are two conflicting instructions, and the server does not guess which was meant. (optional)
	lang := "de" // string | ISO 639-1 language code for localized names (e.g., de, fr, ja) (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BoundariesAPI.GetBoundary(context.Background(), geonameId).Simplify(simplify).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BoundariesAPI.GetBoundary``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetBoundary`: BoundarySingleResponse
	fmt.Fprintf(os.Stdout, "Response from `BoundariesAPI.GetBoundary`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**geonameId** | **int64** | GeoNames id of a country or a region. A city id — or any id that does not name an area — is a 404 &#x60;area_not_an_area&#x60;, not a 400. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetBoundaryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **simplify** | **float64** | Douglas-Peucker tolerance in EPSG:4326 DEGREES, applied before the polygon is serialised. Omit it for full precision.  DEGREES, NOT METRES. The upper bound of 10 is roughly 1,100 km, chosen to make the unit obviously wrong to anyone who typed a value in metres. Simplification stops changing the shape above about 1 degree, so values beyond that buy nothing.  &#x60;0&#x60; is accepted and is a no-op: the response reports &#x60;simplify: null&#x60;, because no tolerance was actually applied.  A negative, non-finite or out-of-range value is a 422, never a 500.  SUPPLY IT AT MOST ONCE. &#x60;?simplify&#x3D;0.01&amp;simplify&#x3D;0.5&#x60; is a 422 rather than a request served with one of the two values silently dropped: two tolerances are two conflicting instructions, and the server does not guess which was meant. | 
 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 

### Return type

[**BoundarySingleResponse**](BoundarySingleResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

