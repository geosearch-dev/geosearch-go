# IPResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Ip** | Pointer to **string** |  | [optional] 
**Network** | Pointer to **string** |  | [optional] 
**Continent** | Pointer to [**IPResultContinent**](IPResultContinent.md) |  | [optional] 
**Country** | Pointer to [**IPResultCountry**](IPResultCountry.md) |  | [optional] 
**Region** | Pointer to [**IPResultRegion**](IPResultRegion.md) |  | [optional] 
**City** | Pointer to [**IPResultCity**](IPResultCity.md) |  | [optional] 
**Postal** | Pointer to [**IPResultPostal**](IPResultPostal.md) |  | [optional] 
**Location** | Pointer to [**IPResultLocation**](IPResultLocation.md) |  | [optional] 
**IsAnonymousProxy** | Pointer to **bool** |  | [optional] 
**IsSatelliteProvider** | Pointer to **bool** |  | [optional] 

## Methods

### NewIPResult

`func NewIPResult() *IPResult`

NewIPResult instantiates a new IPResult object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewIPResultWithDefaults

`func NewIPResultWithDefaults() *IPResult`

NewIPResultWithDefaults instantiates a new IPResult object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIp

`func (o *IPResult) GetIp() string`

GetIp returns the Ip field if non-nil, zero value otherwise.

### GetIpOk

`func (o *IPResult) GetIpOk() (*string, bool)`

GetIpOk returns a tuple with the Ip field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIp

`func (o *IPResult) SetIp(v string)`

SetIp sets Ip field to given value.

### HasIp

`func (o *IPResult) HasIp() bool`

HasIp returns a boolean if a field has been set.

### GetNetwork

`func (o *IPResult) GetNetwork() string`

GetNetwork returns the Network field if non-nil, zero value otherwise.

### GetNetworkOk

`func (o *IPResult) GetNetworkOk() (*string, bool)`

GetNetworkOk returns a tuple with the Network field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNetwork

`func (o *IPResult) SetNetwork(v string)`

SetNetwork sets Network field to given value.

### HasNetwork

`func (o *IPResult) HasNetwork() bool`

HasNetwork returns a boolean if a field has been set.

### GetContinent

`func (o *IPResult) GetContinent() IPResultContinent`

GetContinent returns the Continent field if non-nil, zero value otherwise.

### GetContinentOk

`func (o *IPResult) GetContinentOk() (*IPResultContinent, bool)`

GetContinentOk returns a tuple with the Continent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContinent

`func (o *IPResult) SetContinent(v IPResultContinent)`

SetContinent sets Continent field to given value.

### HasContinent

`func (o *IPResult) HasContinent() bool`

HasContinent returns a boolean if a field has been set.

### GetCountry

`func (o *IPResult) GetCountry() IPResultCountry`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *IPResult) GetCountryOk() (*IPResultCountry, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *IPResult) SetCountry(v IPResultCountry)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *IPResult) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetRegion

`func (o *IPResult) GetRegion() IPResultRegion`

GetRegion returns the Region field if non-nil, zero value otherwise.

### GetRegionOk

`func (o *IPResult) GetRegionOk() (*IPResultRegion, bool)`

GetRegionOk returns a tuple with the Region field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegion

`func (o *IPResult) SetRegion(v IPResultRegion)`

SetRegion sets Region field to given value.

### HasRegion

`func (o *IPResult) HasRegion() bool`

HasRegion returns a boolean if a field has been set.

### GetCity

`func (o *IPResult) GetCity() IPResultCity`

GetCity returns the City field if non-nil, zero value otherwise.

### GetCityOk

`func (o *IPResult) GetCityOk() (*IPResultCity, bool)`

GetCityOk returns a tuple with the City field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCity

`func (o *IPResult) SetCity(v IPResultCity)`

SetCity sets City field to given value.

### HasCity

`func (o *IPResult) HasCity() bool`

HasCity returns a boolean if a field has been set.

### GetPostal

`func (o *IPResult) GetPostal() IPResultPostal`

GetPostal returns the Postal field if non-nil, zero value otherwise.

### GetPostalOk

`func (o *IPResult) GetPostalOk() (*IPResultPostal, bool)`

GetPostalOk returns a tuple with the Postal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostal

`func (o *IPResult) SetPostal(v IPResultPostal)`

SetPostal sets Postal field to given value.

### HasPostal

`func (o *IPResult) HasPostal() bool`

HasPostal returns a boolean if a field has been set.

### GetLocation

`func (o *IPResult) GetLocation() IPResultLocation`

GetLocation returns the Location field if non-nil, zero value otherwise.

### GetLocationOk

`func (o *IPResult) GetLocationOk() (*IPResultLocation, bool)`

GetLocationOk returns a tuple with the Location field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocation

`func (o *IPResult) SetLocation(v IPResultLocation)`

SetLocation sets Location field to given value.

### HasLocation

`func (o *IPResult) HasLocation() bool`

HasLocation returns a boolean if a field has been set.

### GetIsAnonymousProxy

`func (o *IPResult) GetIsAnonymousProxy() bool`

GetIsAnonymousProxy returns the IsAnonymousProxy field if non-nil, zero value otherwise.

### GetIsAnonymousProxyOk

`func (o *IPResult) GetIsAnonymousProxyOk() (*bool, bool)`

GetIsAnonymousProxyOk returns a tuple with the IsAnonymousProxy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsAnonymousProxy

`func (o *IPResult) SetIsAnonymousProxy(v bool)`

SetIsAnonymousProxy sets IsAnonymousProxy field to given value.

### HasIsAnonymousProxy

`func (o *IPResult) HasIsAnonymousProxy() bool`

HasIsAnonymousProxy returns a boolean if a field has been set.

### GetIsSatelliteProvider

`func (o *IPResult) GetIsSatelliteProvider() bool`

GetIsSatelliteProvider returns the IsSatelliteProvider field if non-nil, zero value otherwise.

### GetIsSatelliteProviderOk

`func (o *IPResult) GetIsSatelliteProviderOk() (*bool, bool)`

GetIsSatelliteProviderOk returns a tuple with the IsSatelliteProvider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsSatelliteProvider

`func (o *IPResult) SetIsSatelliteProvider(v bool)`

SetIsSatelliteProvider sets IsSatelliteProvider field to given value.

### HasIsSatelliteProvider

`func (o *IPResult) HasIsSatelliteProvider() bool`

HasIsSatelliteProvider returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


