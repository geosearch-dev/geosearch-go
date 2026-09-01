# GeoJSONGeometry

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** | &#x60;MultiPolygon&#x60; for most areas, &#x60;Polygon&#x60; for areas with a single ring — including areas that BECOME single-ring under &#x60;?simplify&#x3D;&#x60;. Do not pin this to one value. | 
**Coordinates** | **[]interface{}** | Nesting depth depends on &#x60;type&#x60;: three levels for &#x60;Polygon&#x60;, four for &#x60;MultiPolygon&#x60;. Positions are &#x60;[longitude, latitude]&#x60; in EPSG:4326, per the GeoJSON specification. | 

## Methods

### NewGeoJSONGeometry

`func NewGeoJSONGeometry(type_ string, coordinates []interface{}, ) *GeoJSONGeometry`

NewGeoJSONGeometry instantiates a new GeoJSONGeometry object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGeoJSONGeometryWithDefaults

`func NewGeoJSONGeometryWithDefaults() *GeoJSONGeometry`

NewGeoJSONGeometryWithDefaults instantiates a new GeoJSONGeometry object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *GeoJSONGeometry) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *GeoJSONGeometry) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *GeoJSONGeometry) SetType(v string)`

SetType sets Type field to given value.


### GetCoordinates

`func (o *GeoJSONGeometry) GetCoordinates() []interface{}`

GetCoordinates returns the Coordinates field if non-nil, zero value otherwise.

### GetCoordinatesOk

`func (o *GeoJSONGeometry) GetCoordinatesOk() (*[]interface{}, bool)`

GetCoordinatesOk returns a tuple with the Coordinates field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCoordinates

`func (o *GeoJSONGeometry) SetCoordinates(v []interface{})`

SetCoordinates sets Coordinates field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


