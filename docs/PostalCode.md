# PostalCode

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int64** |  | [optional] 
**CountryCode** | Pointer to **string** |  | [optional] 
**PostalCode** | Pointer to **string** |  | [optional] 
**PlaceName** | Pointer to **string** |  | [optional] 
**AdminName1** | Pointer to **string** |  | [optional] 
**AdminCode1** | Pointer to **string** |  | [optional] 
**AdminName2** | Pointer to **string** |  | [optional] 
**AdminCode2** | Pointer to **string** |  | [optional] 
**AdminName3** | Pointer to **string** |  | [optional] 
**AdminCode3** | Pointer to **string** |  | [optional] 
**Latitude** | Pointer to **float64** |  | [optional] 
**Longitude** | Pointer to **float64** |  | [optional] 
**Accuracy** | Pointer to **int32** |  | [optional] 
**Country** | Pointer to [**CountryRef**](CountryRef.md) |  | [optional] 

## Methods

### NewPostalCode

`func NewPostalCode() *PostalCode`

NewPostalCode instantiates a new PostalCode object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPostalCodeWithDefaults

`func NewPostalCodeWithDefaults() *PostalCode`

NewPostalCodeWithDefaults instantiates a new PostalCode object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *PostalCode) GetId() int64`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *PostalCode) GetIdOk() (*int64, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *PostalCode) SetId(v int64)`

SetId sets Id field to given value.

### HasId

`func (o *PostalCode) HasId() bool`

HasId returns a boolean if a field has been set.

### GetCountryCode

`func (o *PostalCode) GetCountryCode() string`

GetCountryCode returns the CountryCode field if non-nil, zero value otherwise.

### GetCountryCodeOk

`func (o *PostalCode) GetCountryCodeOk() (*string, bool)`

GetCountryCodeOk returns a tuple with the CountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountryCode

`func (o *PostalCode) SetCountryCode(v string)`

SetCountryCode sets CountryCode field to given value.

### HasCountryCode

`func (o *PostalCode) HasCountryCode() bool`

HasCountryCode returns a boolean if a field has been set.

### GetPostalCode

`func (o *PostalCode) GetPostalCode() string`

GetPostalCode returns the PostalCode field if non-nil, zero value otherwise.

### GetPostalCodeOk

`func (o *PostalCode) GetPostalCodeOk() (*string, bool)`

GetPostalCodeOk returns a tuple with the PostalCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostalCode

`func (o *PostalCode) SetPostalCode(v string)`

SetPostalCode sets PostalCode field to given value.

### HasPostalCode

`func (o *PostalCode) HasPostalCode() bool`

HasPostalCode returns a boolean if a field has been set.

### GetPlaceName

`func (o *PostalCode) GetPlaceName() string`

GetPlaceName returns the PlaceName field if non-nil, zero value otherwise.

### GetPlaceNameOk

`func (o *PostalCode) GetPlaceNameOk() (*string, bool)`

GetPlaceNameOk returns a tuple with the PlaceName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlaceName

`func (o *PostalCode) SetPlaceName(v string)`

SetPlaceName sets PlaceName field to given value.

### HasPlaceName

`func (o *PostalCode) HasPlaceName() bool`

HasPlaceName returns a boolean if a field has been set.

### GetAdminName1

`func (o *PostalCode) GetAdminName1() string`

GetAdminName1 returns the AdminName1 field if non-nil, zero value otherwise.

### GetAdminName1Ok

`func (o *PostalCode) GetAdminName1Ok() (*string, bool)`

GetAdminName1Ok returns a tuple with the AdminName1 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdminName1

`func (o *PostalCode) SetAdminName1(v string)`

SetAdminName1 sets AdminName1 field to given value.

### HasAdminName1

`func (o *PostalCode) HasAdminName1() bool`

HasAdminName1 returns a boolean if a field has been set.

### GetAdminCode1

`func (o *PostalCode) GetAdminCode1() string`

GetAdminCode1 returns the AdminCode1 field if non-nil, zero value otherwise.

### GetAdminCode1Ok

`func (o *PostalCode) GetAdminCode1Ok() (*string, bool)`

GetAdminCode1Ok returns a tuple with the AdminCode1 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdminCode1

`func (o *PostalCode) SetAdminCode1(v string)`

SetAdminCode1 sets AdminCode1 field to given value.

### HasAdminCode1

`func (o *PostalCode) HasAdminCode1() bool`

HasAdminCode1 returns a boolean if a field has been set.

### GetAdminName2

`func (o *PostalCode) GetAdminName2() string`

GetAdminName2 returns the AdminName2 field if non-nil, zero value otherwise.

### GetAdminName2Ok

`func (o *PostalCode) GetAdminName2Ok() (*string, bool)`

GetAdminName2Ok returns a tuple with the AdminName2 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdminName2

`func (o *PostalCode) SetAdminName2(v string)`

SetAdminName2 sets AdminName2 field to given value.

### HasAdminName2

`func (o *PostalCode) HasAdminName2() bool`

HasAdminName2 returns a boolean if a field has been set.

### GetAdminCode2

`func (o *PostalCode) GetAdminCode2() string`

GetAdminCode2 returns the AdminCode2 field if non-nil, zero value otherwise.

### GetAdminCode2Ok

`func (o *PostalCode) GetAdminCode2Ok() (*string, bool)`

GetAdminCode2Ok returns a tuple with the AdminCode2 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdminCode2

`func (o *PostalCode) SetAdminCode2(v string)`

SetAdminCode2 sets AdminCode2 field to given value.

### HasAdminCode2

`func (o *PostalCode) HasAdminCode2() bool`

HasAdminCode2 returns a boolean if a field has been set.

### GetAdminName3

`func (o *PostalCode) GetAdminName3() string`

GetAdminName3 returns the AdminName3 field if non-nil, zero value otherwise.

### GetAdminName3Ok

`func (o *PostalCode) GetAdminName3Ok() (*string, bool)`

GetAdminName3Ok returns a tuple with the AdminName3 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdminName3

`func (o *PostalCode) SetAdminName3(v string)`

SetAdminName3 sets AdminName3 field to given value.

### HasAdminName3

`func (o *PostalCode) HasAdminName3() bool`

HasAdminName3 returns a boolean if a field has been set.

### GetAdminCode3

`func (o *PostalCode) GetAdminCode3() string`

GetAdminCode3 returns the AdminCode3 field if non-nil, zero value otherwise.

### GetAdminCode3Ok

`func (o *PostalCode) GetAdminCode3Ok() (*string, bool)`

GetAdminCode3Ok returns a tuple with the AdminCode3 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdminCode3

`func (o *PostalCode) SetAdminCode3(v string)`

SetAdminCode3 sets AdminCode3 field to given value.

### HasAdminCode3

`func (o *PostalCode) HasAdminCode3() bool`

HasAdminCode3 returns a boolean if a field has been set.

### GetLatitude

`func (o *PostalCode) GetLatitude() float64`

GetLatitude returns the Latitude field if non-nil, zero value otherwise.

### GetLatitudeOk

`func (o *PostalCode) GetLatitudeOk() (*float64, bool)`

GetLatitudeOk returns a tuple with the Latitude field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatitude

`func (o *PostalCode) SetLatitude(v float64)`

SetLatitude sets Latitude field to given value.

### HasLatitude

`func (o *PostalCode) HasLatitude() bool`

HasLatitude returns a boolean if a field has been set.

### GetLongitude

`func (o *PostalCode) GetLongitude() float64`

GetLongitude returns the Longitude field if non-nil, zero value otherwise.

### GetLongitudeOk

`func (o *PostalCode) GetLongitudeOk() (*float64, bool)`

GetLongitudeOk returns a tuple with the Longitude field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLongitude

`func (o *PostalCode) SetLongitude(v float64)`

SetLongitude sets Longitude field to given value.

### HasLongitude

`func (o *PostalCode) HasLongitude() bool`

HasLongitude returns a boolean if a field has been set.

### GetAccuracy

`func (o *PostalCode) GetAccuracy() int32`

GetAccuracy returns the Accuracy field if non-nil, zero value otherwise.

### GetAccuracyOk

`func (o *PostalCode) GetAccuracyOk() (*int32, bool)`

GetAccuracyOk returns a tuple with the Accuracy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccuracy

`func (o *PostalCode) SetAccuracy(v int32)`

SetAccuracy sets Accuracy field to given value.

### HasAccuracy

`func (o *PostalCode) HasAccuracy() bool`

HasAccuracy returns a boolean if a field has been set.

### GetCountry

`func (o *PostalCode) GetCountry() CountryRef`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *PostalCode) GetCountryOk() (*CountryRef, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *PostalCode) SetCountry(v CountryRef)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *PostalCode) HasCountry() bool`

HasCountry returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


