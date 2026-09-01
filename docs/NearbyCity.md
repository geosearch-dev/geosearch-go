# NearbyCity

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int64** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**CountryCode** | Pointer to **string** |  | [optional] 
**Population** | Pointer to **int64** |  | [optional] 
**Timezone** | Pointer to **string** |  | [optional] 
**Latitude** | Pointer to **float64** |  | [optional] 
**Longitude** | Pointer to **float64** |  | [optional] 
**DistanceKm** | Pointer to **float64** |  | [optional] 
**Country** | Pointer to [**CountryRef**](CountryRef.md) |  | [optional] 
**Region** | Pointer to [**RegionRef**](RegionRef.md) |  | [optional] 

## Methods

### NewNearbyCity

`func NewNearbyCity() *NearbyCity`

NewNearbyCity instantiates a new NearbyCity object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewNearbyCityWithDefaults

`func NewNearbyCityWithDefaults() *NearbyCity`

NewNearbyCityWithDefaults instantiates a new NearbyCity object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *NearbyCity) GetId() int64`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *NearbyCity) GetIdOk() (*int64, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *NearbyCity) SetId(v int64)`

SetId sets Id field to given value.

### HasId

`func (o *NearbyCity) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *NearbyCity) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *NearbyCity) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *NearbyCity) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *NearbyCity) HasName() bool`

HasName returns a boolean if a field has been set.

### GetCountryCode

`func (o *NearbyCity) GetCountryCode() string`

GetCountryCode returns the CountryCode field if non-nil, zero value otherwise.

### GetCountryCodeOk

`func (o *NearbyCity) GetCountryCodeOk() (*string, bool)`

GetCountryCodeOk returns a tuple with the CountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountryCode

`func (o *NearbyCity) SetCountryCode(v string)`

SetCountryCode sets CountryCode field to given value.

### HasCountryCode

`func (o *NearbyCity) HasCountryCode() bool`

HasCountryCode returns a boolean if a field has been set.

### GetPopulation

`func (o *NearbyCity) GetPopulation() int64`

GetPopulation returns the Population field if non-nil, zero value otherwise.

### GetPopulationOk

`func (o *NearbyCity) GetPopulationOk() (*int64, bool)`

GetPopulationOk returns a tuple with the Population field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPopulation

`func (o *NearbyCity) SetPopulation(v int64)`

SetPopulation sets Population field to given value.

### HasPopulation

`func (o *NearbyCity) HasPopulation() bool`

HasPopulation returns a boolean if a field has been set.

### GetTimezone

`func (o *NearbyCity) GetTimezone() string`

GetTimezone returns the Timezone field if non-nil, zero value otherwise.

### GetTimezoneOk

`func (o *NearbyCity) GetTimezoneOk() (*string, bool)`

GetTimezoneOk returns a tuple with the Timezone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimezone

`func (o *NearbyCity) SetTimezone(v string)`

SetTimezone sets Timezone field to given value.

### HasTimezone

`func (o *NearbyCity) HasTimezone() bool`

HasTimezone returns a boolean if a field has been set.

### GetLatitude

`func (o *NearbyCity) GetLatitude() float64`

GetLatitude returns the Latitude field if non-nil, zero value otherwise.

### GetLatitudeOk

`func (o *NearbyCity) GetLatitudeOk() (*float64, bool)`

GetLatitudeOk returns a tuple with the Latitude field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatitude

`func (o *NearbyCity) SetLatitude(v float64)`

SetLatitude sets Latitude field to given value.

### HasLatitude

`func (o *NearbyCity) HasLatitude() bool`

HasLatitude returns a boolean if a field has been set.

### GetLongitude

`func (o *NearbyCity) GetLongitude() float64`

GetLongitude returns the Longitude field if non-nil, zero value otherwise.

### GetLongitudeOk

`func (o *NearbyCity) GetLongitudeOk() (*float64, bool)`

GetLongitudeOk returns a tuple with the Longitude field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLongitude

`func (o *NearbyCity) SetLongitude(v float64)`

SetLongitude sets Longitude field to given value.

### HasLongitude

`func (o *NearbyCity) HasLongitude() bool`

HasLongitude returns a boolean if a field has been set.

### GetDistanceKm

`func (o *NearbyCity) GetDistanceKm() float64`

GetDistanceKm returns the DistanceKm field if non-nil, zero value otherwise.

### GetDistanceKmOk

`func (o *NearbyCity) GetDistanceKmOk() (*float64, bool)`

GetDistanceKmOk returns a tuple with the DistanceKm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDistanceKm

`func (o *NearbyCity) SetDistanceKm(v float64)`

SetDistanceKm sets DistanceKm field to given value.

### HasDistanceKm

`func (o *NearbyCity) HasDistanceKm() bool`

HasDistanceKm returns a boolean if a field has been set.

### GetCountry

`func (o *NearbyCity) GetCountry() CountryRef`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *NearbyCity) GetCountryOk() (*CountryRef, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *NearbyCity) SetCountry(v CountryRef)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *NearbyCity) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetRegion

`func (o *NearbyCity) GetRegion() RegionRef`

GetRegion returns the Region field if non-nil, zero value otherwise.

### GetRegionOk

`func (o *NearbyCity) GetRegionOk() (*RegionRef, bool)`

GetRegionOk returns a tuple with the Region field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegion

`func (o *NearbyCity) SetRegion(v RegionRef)`

SetRegion sets Region field to given value.

### HasRegion

`func (o *NearbyCity) HasRegion() bool`

HasRegion returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


