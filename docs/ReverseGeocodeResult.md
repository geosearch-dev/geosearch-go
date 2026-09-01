# ReverseGeocodeResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**City** | Pointer to [**NearbyCity**](NearbyCity.md) |  | [optional] 
**DistanceKm** | Pointer to **float64** |  | [optional] 

## Methods

### NewReverseGeocodeResult

`func NewReverseGeocodeResult() *ReverseGeocodeResult`

NewReverseGeocodeResult instantiates a new ReverseGeocodeResult object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReverseGeocodeResultWithDefaults

`func NewReverseGeocodeResultWithDefaults() *ReverseGeocodeResult`

NewReverseGeocodeResultWithDefaults instantiates a new ReverseGeocodeResult object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCity

`func (o *ReverseGeocodeResult) GetCity() NearbyCity`

GetCity returns the City field if non-nil, zero value otherwise.

### GetCityOk

`func (o *ReverseGeocodeResult) GetCityOk() (*NearbyCity, bool)`

GetCityOk returns a tuple with the City field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCity

`func (o *ReverseGeocodeResult) SetCity(v NearbyCity)`

SetCity sets City field to given value.

### HasCity

`func (o *ReverseGeocodeResult) HasCity() bool`

HasCity returns a boolean if a field has been set.

### GetDistanceKm

`func (o *ReverseGeocodeResult) GetDistanceKm() float64`

GetDistanceKm returns the DistanceKm field if non-nil, zero value otherwise.

### GetDistanceKmOk

`func (o *ReverseGeocodeResult) GetDistanceKmOk() (*float64, bool)`

GetDistanceKmOk returns a tuple with the DistanceKm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDistanceKm

`func (o *ReverseGeocodeResult) SetDistanceKm(v float64)`

SetDistanceKm sets DistanceKm field to given value.

### HasDistanceKm

`func (o *ReverseGeocodeResult) HasDistanceKm() bool`

HasDistanceKm returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


