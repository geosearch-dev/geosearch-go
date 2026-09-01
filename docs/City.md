# City

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int64** |  | [optional] 
**GeonameId** | Pointer to **int64** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**AsciiName** | Pointer to **string** |  | [optional] 
**CountryCode** | Pointer to **string** |  | [optional] 
**Admin1Code** | Pointer to **string** |  | [optional] 
**Admin2Code** | Pointer to **string** |  | [optional] 
**Population** | Pointer to **int64** |  | [optional] 
**Elevation** | Pointer to **int32** |  | [optional] 
**Timezone** | Pointer to **string** |  | [optional] 
**Latitude** | Pointer to **float64** |  | [optional] 
**Longitude** | Pointer to **float64** |  | [optional] 
**Country** | Pointer to [**CountryRef**](CountryRef.md) |  | [optional] 
**Region** | Pointer to [**RegionRef**](RegionRef.md) |  | [optional] 

## Methods

### NewCity

`func NewCity() *City`

NewCity instantiates a new City object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCityWithDefaults

`func NewCityWithDefaults() *City`

NewCityWithDefaults instantiates a new City object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *City) GetId() int64`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *City) GetIdOk() (*int64, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *City) SetId(v int64)`

SetId sets Id field to given value.

### HasId

`func (o *City) HasId() bool`

HasId returns a boolean if a field has been set.

### GetGeonameId

`func (o *City) GetGeonameId() int64`

GetGeonameId returns the GeonameId field if non-nil, zero value otherwise.

### GetGeonameIdOk

`func (o *City) GetGeonameIdOk() (*int64, bool)`

GetGeonameIdOk returns a tuple with the GeonameId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGeonameId

`func (o *City) SetGeonameId(v int64)`

SetGeonameId sets GeonameId field to given value.

### HasGeonameId

`func (o *City) HasGeonameId() bool`

HasGeonameId returns a boolean if a field has been set.

### GetName

`func (o *City) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *City) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *City) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *City) HasName() bool`

HasName returns a boolean if a field has been set.

### GetAsciiName

`func (o *City) GetAsciiName() string`

GetAsciiName returns the AsciiName field if non-nil, zero value otherwise.

### GetAsciiNameOk

`func (o *City) GetAsciiNameOk() (*string, bool)`

GetAsciiNameOk returns a tuple with the AsciiName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAsciiName

`func (o *City) SetAsciiName(v string)`

SetAsciiName sets AsciiName field to given value.

### HasAsciiName

`func (o *City) HasAsciiName() bool`

HasAsciiName returns a boolean if a field has been set.

### GetCountryCode

`func (o *City) GetCountryCode() string`

GetCountryCode returns the CountryCode field if non-nil, zero value otherwise.

### GetCountryCodeOk

`func (o *City) GetCountryCodeOk() (*string, bool)`

GetCountryCodeOk returns a tuple with the CountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountryCode

`func (o *City) SetCountryCode(v string)`

SetCountryCode sets CountryCode field to given value.

### HasCountryCode

`func (o *City) HasCountryCode() bool`

HasCountryCode returns a boolean if a field has been set.

### GetAdmin1Code

`func (o *City) GetAdmin1Code() string`

GetAdmin1Code returns the Admin1Code field if non-nil, zero value otherwise.

### GetAdmin1CodeOk

`func (o *City) GetAdmin1CodeOk() (*string, bool)`

GetAdmin1CodeOk returns a tuple with the Admin1Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdmin1Code

`func (o *City) SetAdmin1Code(v string)`

SetAdmin1Code sets Admin1Code field to given value.

### HasAdmin1Code

`func (o *City) HasAdmin1Code() bool`

HasAdmin1Code returns a boolean if a field has been set.

### GetAdmin2Code

`func (o *City) GetAdmin2Code() string`

GetAdmin2Code returns the Admin2Code field if non-nil, zero value otherwise.

### GetAdmin2CodeOk

`func (o *City) GetAdmin2CodeOk() (*string, bool)`

GetAdmin2CodeOk returns a tuple with the Admin2Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdmin2Code

`func (o *City) SetAdmin2Code(v string)`

SetAdmin2Code sets Admin2Code field to given value.

### HasAdmin2Code

`func (o *City) HasAdmin2Code() bool`

HasAdmin2Code returns a boolean if a field has been set.

### GetPopulation

`func (o *City) GetPopulation() int64`

GetPopulation returns the Population field if non-nil, zero value otherwise.

### GetPopulationOk

`func (o *City) GetPopulationOk() (*int64, bool)`

GetPopulationOk returns a tuple with the Population field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPopulation

`func (o *City) SetPopulation(v int64)`

SetPopulation sets Population field to given value.

### HasPopulation

`func (o *City) HasPopulation() bool`

HasPopulation returns a boolean if a field has been set.

### GetElevation

`func (o *City) GetElevation() int32`

GetElevation returns the Elevation field if non-nil, zero value otherwise.

### GetElevationOk

`func (o *City) GetElevationOk() (*int32, bool)`

GetElevationOk returns a tuple with the Elevation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetElevation

`func (o *City) SetElevation(v int32)`

SetElevation sets Elevation field to given value.

### HasElevation

`func (o *City) HasElevation() bool`

HasElevation returns a boolean if a field has been set.

### GetTimezone

`func (o *City) GetTimezone() string`

GetTimezone returns the Timezone field if non-nil, zero value otherwise.

### GetTimezoneOk

`func (o *City) GetTimezoneOk() (*string, bool)`

GetTimezoneOk returns a tuple with the Timezone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimezone

`func (o *City) SetTimezone(v string)`

SetTimezone sets Timezone field to given value.

### HasTimezone

`func (o *City) HasTimezone() bool`

HasTimezone returns a boolean if a field has been set.

### GetLatitude

`func (o *City) GetLatitude() float64`

GetLatitude returns the Latitude field if non-nil, zero value otherwise.

### GetLatitudeOk

`func (o *City) GetLatitudeOk() (*float64, bool)`

GetLatitudeOk returns a tuple with the Latitude field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatitude

`func (o *City) SetLatitude(v float64)`

SetLatitude sets Latitude field to given value.

### HasLatitude

`func (o *City) HasLatitude() bool`

HasLatitude returns a boolean if a field has been set.

### GetLongitude

`func (o *City) GetLongitude() float64`

GetLongitude returns the Longitude field if non-nil, zero value otherwise.

### GetLongitudeOk

`func (o *City) GetLongitudeOk() (*float64, bool)`

GetLongitudeOk returns a tuple with the Longitude field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLongitude

`func (o *City) SetLongitude(v float64)`

SetLongitude sets Longitude field to given value.

### HasLongitude

`func (o *City) HasLongitude() bool`

HasLongitude returns a boolean if a field has been set.

### GetCountry

`func (o *City) GetCountry() CountryRef`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *City) GetCountryOk() (*CountryRef, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *City) SetCountry(v CountryRef)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *City) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetRegion

`func (o *City) GetRegion() RegionRef`

GetRegion returns the Region field if non-nil, zero value otherwise.

### GetRegionOk

`func (o *City) GetRegionOk() (*RegionRef, bool)`

GetRegionOk returns a tuple with the Region field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegion

`func (o *City) SetRegion(v RegionRef)`

SetRegion sets Region field to given value.

### HasRegion

`func (o *City) HasRegion() bool`

HasRegion returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


