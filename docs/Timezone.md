# Timezone

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int64** |  | [optional] 
**CountryCode** | Pointer to **string** |  | [optional] 
**TimezoneId** | Pointer to **string** |  | [optional] 
**GmtOffset** | Pointer to **float64** |  | [optional] 
**DstOffset** | Pointer to **float64** |  | [optional] 
**RawOffset** | Pointer to **float64** |  | [optional] 

## Methods

### NewTimezone

`func NewTimezone() *Timezone`

NewTimezone instantiates a new Timezone object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTimezoneWithDefaults

`func NewTimezoneWithDefaults() *Timezone`

NewTimezoneWithDefaults instantiates a new Timezone object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Timezone) GetId() int64`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Timezone) GetIdOk() (*int64, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Timezone) SetId(v int64)`

SetId sets Id field to given value.

### HasId

`func (o *Timezone) HasId() bool`

HasId returns a boolean if a field has been set.

### GetCountryCode

`func (o *Timezone) GetCountryCode() string`

GetCountryCode returns the CountryCode field if non-nil, zero value otherwise.

### GetCountryCodeOk

`func (o *Timezone) GetCountryCodeOk() (*string, bool)`

GetCountryCodeOk returns a tuple with the CountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountryCode

`func (o *Timezone) SetCountryCode(v string)`

SetCountryCode sets CountryCode field to given value.

### HasCountryCode

`func (o *Timezone) HasCountryCode() bool`

HasCountryCode returns a boolean if a field has been set.

### GetTimezoneId

`func (o *Timezone) GetTimezoneId() string`

GetTimezoneId returns the TimezoneId field if non-nil, zero value otherwise.

### GetTimezoneIdOk

`func (o *Timezone) GetTimezoneIdOk() (*string, bool)`

GetTimezoneIdOk returns a tuple with the TimezoneId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimezoneId

`func (o *Timezone) SetTimezoneId(v string)`

SetTimezoneId sets TimezoneId field to given value.

### HasTimezoneId

`func (o *Timezone) HasTimezoneId() bool`

HasTimezoneId returns a boolean if a field has been set.

### GetGmtOffset

`func (o *Timezone) GetGmtOffset() float64`

GetGmtOffset returns the GmtOffset field if non-nil, zero value otherwise.

### GetGmtOffsetOk

`func (o *Timezone) GetGmtOffsetOk() (*float64, bool)`

GetGmtOffsetOk returns a tuple with the GmtOffset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGmtOffset

`func (o *Timezone) SetGmtOffset(v float64)`

SetGmtOffset sets GmtOffset field to given value.

### HasGmtOffset

`func (o *Timezone) HasGmtOffset() bool`

HasGmtOffset returns a boolean if a field has been set.

### GetDstOffset

`func (o *Timezone) GetDstOffset() float64`

GetDstOffset returns the DstOffset field if non-nil, zero value otherwise.

### GetDstOffsetOk

`func (o *Timezone) GetDstOffsetOk() (*float64, bool)`

GetDstOffsetOk returns a tuple with the DstOffset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDstOffset

`func (o *Timezone) SetDstOffset(v float64)`

SetDstOffset sets DstOffset field to given value.

### HasDstOffset

`func (o *Timezone) HasDstOffset() bool`

HasDstOffset returns a boolean if a field has been set.

### GetRawOffset

`func (o *Timezone) GetRawOffset() float64`

GetRawOffset returns the RawOffset field if non-nil, zero value otherwise.

### GetRawOffsetOk

`func (o *Timezone) GetRawOffsetOk() (*float64, bool)`

GetRawOffsetOk returns a tuple with the RawOffset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRawOffset

`func (o *Timezone) SetRawOffset(v float64)`

SetRawOffset sets RawOffset field to given value.

### HasRawOffset

`func (o *Timezone) HasRawOffset() bool`

HasRawOffset returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


