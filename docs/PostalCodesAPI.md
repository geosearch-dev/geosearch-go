# \PostalCodesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListPostalCodes**](PostalCodesAPI.md#ListPostalCodes) | **Get** /v1/postal-codes | List postal codes
[**NearestPostalCode**](PostalCodesAPI.md#NearestPostalCode) | **Get** /v1/postal-codes/nearest | Find nearest postal codes



## ListPostalCodes

> PostalCodeListResponse ListPostalCodes(ctx).Lang(lang).Country(country).Code(code).Within(within).Bbox(bbox).Cursor(cursor).Limit(limit).Fields(fields).Sort(sort).Execute()

List postal codes



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
	country := "US" // string | Filter by ISO alpha-2 country codes (comma-separated) (optional)
	code := "94105" // string | Filter by postal code (optional)
	within := int64(6252001) // int64 | Return only results whose coordinates fall geometrically inside the boundary of the given area, identified by its GeoNames id. Countries and administrative regions are valid areas; a city id is not.  Accepts exactly one id. A COMMA-SEPARATED LIST IS REJECTED with a 422 naming the limit — a deliberate departure from the comma-separated convention `country` uses, because each value would be a separate polygon intersection. Ask for one area per request.  COST: a request using this parameter consumes 2 quota units instead of 1, on every plan including Free. Combining it with `bbox` still costs 2, not 3 — the highest multiplier applies rather than the sum, and adding a box makes the query cheaper to serve, so it is never penalised.  This asks a GEOMETRIC question and can therefore return a different set of cities than `/v1/regions/{id}/cities`, which asks an administrative one. See that endpoint's description for when and why the two disagree.  Two failures are reported with distinct 400 codes so a typo is distinguishable from a coverage gap: `area_not_an_area` means the id does not name a country or region at all, and `area_no_boundary` means it does but no boundary polygon is available for it yet. (optional)
	bbox := "-122.6,37.6,-122.2,37.9" // string | Return only results inside the bounding box, given as four comma-separated numbers in the order `w,s,e,n` — west longitude, south latitude, east longitude, north latitude.  Longitudes must be within [-180, 180] and latitudes within [-90, 90].  A box where WEST IS GREATER THAN EAST wraps the antimeridian and is fully supported: `bbox=170,-20,-170,-10` is a box around Fiji, evaluated as the union of the two halves it spans. Latitude has no equivalent wrap-around meaning, so `s` greater than `n` is a validation error rather than a wrapped box.  Charged at the standard request cost of 1 unit. Adding it to a `within` query narrows the candidate set before the polygon test and does not raise the charge. (optional)
	cursor := "eyJpZCI6MjV9" // string | Pagination cursor from a previous response (optional)
	limit := int32(25) // int32 | Number of results per page (1-100, default 25) (optional) (default to 25)
	fields := "name,population,iso_code" // string | Comma-separated list of fields to include in the response (optional)
	sort := "postal_code" // string | Sort field. Allowed: postal_code, country_code, place_name, id. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PostalCodesAPI.ListPostalCodes(context.Background()).Lang(lang).Country(country).Code(code).Within(within).Bbox(bbox).Cursor(cursor).Limit(limit).Fields(fields).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PostalCodesAPI.ListPostalCodes``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPostalCodes`: PostalCodeListResponse
	fmt.Fprintf(os.Stdout, "Response from `PostalCodesAPI.ListPostalCodes`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListPostalCodesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **country** | **string** | Filter by ISO alpha-2 country codes (comma-separated) | 
 **code** | **string** | Filter by postal code | 
 **within** | **int64** | Return only results whose coordinates fall geometrically inside the boundary of the given area, identified by its GeoNames id. Countries and administrative regions are valid areas; a city id is not.  Accepts exactly one id. A COMMA-SEPARATED LIST IS REJECTED with a 422 naming the limit — a deliberate departure from the comma-separated convention &#x60;country&#x60; uses, because each value would be a separate polygon intersection. Ask for one area per request.  COST: a request using this parameter consumes 2 quota units instead of 1, on every plan including Free. Combining it with &#x60;bbox&#x60; still costs 2, not 3 — the highest multiplier applies rather than the sum, and adding a box makes the query cheaper to serve, so it is never penalised.  This asks a GEOMETRIC question and can therefore return a different set of cities than &#x60;/v1/regions/{id}/cities&#x60;, which asks an administrative one. See that endpoint&#39;s description for when and why the two disagree.  Two failures are reported with distinct 400 codes so a typo is distinguishable from a coverage gap: &#x60;area_not_an_area&#x60; means the id does not name a country or region at all, and &#x60;area_no_boundary&#x60; means it does but no boundary polygon is available for it yet. | 
 **bbox** | **string** | Return only results inside the bounding box, given as four comma-separated numbers in the order &#x60;w,s,e,n&#x60; — west longitude, south latitude, east longitude, north latitude.  Longitudes must be within [-180, 180] and latitudes within [-90, 90].  A box where WEST IS GREATER THAN EAST wraps the antimeridian and is fully supported: &#x60;bbox&#x3D;170,-20,-170,-10&#x60; is a box around Fiji, evaluated as the union of the two halves it spans. Latitude has no equivalent wrap-around meaning, so &#x60;s&#x60; greater than &#x60;n&#x60; is a validation error rather than a wrapped box.  Charged at the standard request cost of 1 unit. Adding it to a &#x60;within&#x60; query narrows the candidate set before the polygon test and does not raise the charge. | 
 **cursor** | **string** | Pagination cursor from a previous response | 
 **limit** | **int32** | Number of results per page (1-100, default 25) | [default to 25]
 **fields** | **string** | Comma-separated list of fields to include in the response | 
 **sort** | **string** | Sort field. Allowed: postal_code, country_code, place_name, id. | 

### Return type

[**PostalCodeListResponse**](PostalCodeListResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## NearestPostalCode

> PostalCodeListResponse NearestPostalCode(ctx).Lat(lat).Lon(lon).Lang(lang).Limit(limit).Execute()

Find nearest postal codes



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
	lat := float64(37.7749) // float64 | Latitude (-90 to 90)
	lon := float64(-122.4194) // float64 | Longitude (-180 to 180)
	lang := "de" // string | ISO 639-1 language code for localized names (e.g., de, fr, ja) (optional)
	limit := int32(3) // int32 | Number of results (1-10, default 1) (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PostalCodesAPI.NearestPostalCode(context.Background()).Lat(lat).Lon(lon).Lang(lang).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PostalCodesAPI.NearestPostalCode``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `NearestPostalCode`: PostalCodeListResponse
	fmt.Fprintf(os.Stdout, "Response from `PostalCodesAPI.NearestPostalCode`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiNearestPostalCodeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lat** | **float64** | Latitude (-90 to 90) | 
 **lon** | **float64** | Longitude (-180 to 180) | 
 **lang** | **string** | ISO 639-1 language code for localized names (e.g., de, fr, ja) | 
 **limit** | **int32** | Number of results (1-10, default 1) | [default to 1]

### Return type

[**PostalCodeListResponse**](PostalCodeListResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

