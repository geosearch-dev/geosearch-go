# Region

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int64** |  | [optional] 
**GeonameId** | Pointer to **int64** |  | [optional] 
**CountryCode** | Pointer to **string** |  | [optional] 
**AdminCode** | Pointer to **string** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**AsciiName** | Pointer to **string** |  | [optional] 
**Level** | Pointer to **int32** |  | [optional] 
**ParentGeonameId** | Pointer to **int64** |  | [optional] 
**Population** | Pointer to **int64** |  | [optional] 
**Latitude** | Pointer to **float64** |  | [optional] 
**Longitude** | Pointer to **float64** |  | [optional] 
**Country** | Pointer to [**CountryRef**](CountryRef.md) |  | [optional] 
**Geometry** | Pointer to [**GeoJSONMultiPolygon**](GeoJSONMultiPolygon.md) | Region boundary. Returned by default on &#x60;GET /v1/regions/{id}&#x60;, and on request via &#x60;?fields&#x3D;geometry&#x60; on &#x60;GET /v1/regions&#x60; and &#x60;GET /v1/countries/{code}/regions&#x60;.  REQUIRES A PAID PLAN. On all three of those routes this key is OMITTED ENTIRELY for a Free-tier key — absent, not null, with a 200 status and no error. A client reading &#x60;data.geometry.type&#x60; unconditionally will fail on a null dereference.  To be told explicitly rather than silently, request the polygon from &#x60;GET /v1/boundaries/{geoname_id}&#x60;, which answers a Free key with a 403 and an upgrade link. | [optional] 

## Methods

### NewRegion

`func NewRegion() *Region`

NewRegion instantiates a new Region object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRegionWithDefaults

`func NewRegionWithDefaults() *Region`

NewRegionWithDefaults instantiates a new Region object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Region) GetId() int64`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Region) GetIdOk() (*int64, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Region) SetId(v int64)`

SetId sets Id field to given value.

### HasId

`func (o *Region) HasId() bool`

HasId returns a boolean if a field has been set.

### GetGeonameId

`func (o *Region) GetGeonameId() int64`

GetGeonameId returns the GeonameId field if non-nil, zero value otherwise.

### GetGeonameIdOk

`func (o *Region) GetGeonameIdOk() (*int64, bool)`

GetGeonameIdOk returns a tuple with the GeonameId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGeonameId

`func (o *Region) SetGeonameId(v int64)`

SetGeonameId sets GeonameId field to given value.

### HasGeonameId

`func (o *Region) HasGeonameId() bool`

HasGeonameId returns a boolean if a field has been set.

### GetCountryCode

`func (o *Region) GetCountryCode() string`

GetCountryCode returns the CountryCode field if non-nil, zero value otherwise.

### GetCountryCodeOk

`func (o *Region) GetCountryCodeOk() (*string, bool)`

GetCountryCodeOk returns a tuple with the CountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountryCode

`func (o *Region) SetCountryCode(v string)`

SetCountryCode sets CountryCode field to given value.

### HasCountryCode

`func (o *Region) HasCountryCode() bool`

HasCountryCode returns a boolean if a field has been set.

### GetAdminCode

`func (o *Region) GetAdminCode() string`

GetAdminCode returns the AdminCode field if non-nil, zero value otherwise.

### GetAdminCodeOk

`func (o *Region) GetAdminCodeOk() (*string, bool)`

GetAdminCodeOk returns a tuple with the AdminCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdminCode

`func (o *Region) SetAdminCode(v string)`

SetAdminCode sets AdminCode field to given value.

### HasAdminCode

`func (o *Region) HasAdminCode() bool`

HasAdminCode returns a boolean if a field has been set.

### GetName

`func (o *Region) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Region) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Region) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *Region) HasName() bool`

HasName returns a boolean if a field has been set.

### GetAsciiName

`func (o *Region) GetAsciiName() string`

GetAsciiName returns the AsciiName field if non-nil, zero value otherwise.

### GetAsciiNameOk

`func (o *Region) GetAsciiNameOk() (*string, bool)`

GetAsciiNameOk returns a tuple with the AsciiName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAsciiName

`func (o *Region) SetAsciiName(v string)`

SetAsciiName sets AsciiName field to given value.

### HasAsciiName

`func (o *Region) HasAsciiName() bool`

HasAsciiName returns a boolean if a field has been set.

### GetLevel

`func (o *Region) GetLevel() int32`

GetLevel returns the Level field if non-nil, zero value otherwise.

### GetLevelOk

`func (o *Region) GetLevelOk() (*int32, bool)`

GetLevelOk returns a tuple with the Level field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLevel

`func (o *Region) SetLevel(v int32)`

SetLevel sets Level field to given value.

### HasLevel

`func (o *Region) HasLevel() bool`

HasLevel returns a boolean if a field has been set.

### GetParentGeonameId

`func (o *Region) GetParentGeonameId() int64`

GetParentGeonameId returns the ParentGeonameId field if non-nil, zero value otherwise.

### GetParentGeonameIdOk

`func (o *Region) GetParentGeonameIdOk() (*int64, bool)`

GetParentGeonameIdOk returns a tuple with the ParentGeonameId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParentGeonameId

`func (o *Region) SetParentGeonameId(v int64)`

SetParentGeonameId sets ParentGeonameId field to given value.

### HasParentGeonameId

`func (o *Region) HasParentGeonameId() bool`

HasParentGeonameId returns a boolean if a field has been set.

### GetPopulation

`func (o *Region) GetPopulation() int64`

GetPopulation returns the Population field if non-nil, zero value otherwise.

### GetPopulationOk

`func (o *Region) GetPopulationOk() (*int64, bool)`

GetPopulationOk returns a tuple with the Population field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPopulation

`func (o *Region) SetPopulation(v int64)`

SetPopulation sets Population field to given value.

### HasPopulation

`func (o *Region) HasPopulation() bool`

HasPopulation returns a boolean if a field has been set.

### GetLatitude

`func (o *Region) GetLatitude() float64`

GetLatitude returns the Latitude field if non-nil, zero value otherwise.

### GetLatitudeOk

`func (o *Region) GetLatitudeOk() (*float64, bool)`

GetLatitudeOk returns a tuple with the Latitude field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatitude

`func (o *Region) SetLatitude(v float64)`

SetLatitude sets Latitude field to given value.

### HasLatitude

`func (o *Region) HasLatitude() bool`

HasLatitude returns a boolean if a field has been set.

### GetLongitude

`func (o *Region) GetLongitude() float64`

GetLongitude returns the Longitude field if non-nil, zero value otherwise.

### GetLongitudeOk

`func (o *Region) GetLongitudeOk() (*float64, bool)`

GetLongitudeOk returns a tuple with the Longitude field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLongitude

`func (o *Region) SetLongitude(v float64)`

SetLongitude sets Longitude field to given value.

### HasLongitude

`func (o *Region) HasLongitude() bool`

HasLongitude returns a boolean if a field has been set.

### GetCountry

`func (o *Region) GetCountry() CountryRef`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *Region) GetCountryOk() (*CountryRef, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *Region) SetCountry(v CountryRef)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *Region) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetGeometry

`func (o *Region) GetGeometry() GeoJSONMultiPolygon`

GetGeometry returns the Geometry field if non-nil, zero value otherwise.

### GetGeometryOk

`func (o *Region) GetGeometryOk() (*GeoJSONMultiPolygon, bool)`

GetGeometryOk returns a tuple with the Geometry field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGeometry

`func (o *Region) SetGeometry(v GeoJSONMultiPolygon)`

SetGeometry sets Geometry field to given value.

### HasGeometry

`func (o *Region) HasGeometry() bool`

HasGeometry returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


