# CityListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | Pointer to [**[]City**](City.md) |  | [optional] 
**Meta** | Pointer to [**PaginationMeta**](PaginationMeta.md) |  | [optional] 

## Methods

### NewCityListResponse

`func NewCityListResponse() *CityListResponse`

NewCityListResponse instantiates a new CityListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCityListResponseWithDefaults

`func NewCityListResponseWithDefaults() *CityListResponse`

NewCityListResponseWithDefaults instantiates a new CityListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *CityListResponse) GetData() []City`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *CityListResponse) GetDataOk() (*[]City, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *CityListResponse) SetData(v []City)`

SetData sets Data field to given value.

### HasData

`func (o *CityListResponse) HasData() bool`

HasData returns a boolean if a field has been set.

### GetMeta

`func (o *CityListResponse) GetMeta() PaginationMeta`

GetMeta returns the Meta field if non-nil, zero value otherwise.

### GetMetaOk

`func (o *CityListResponse) GetMetaOk() (*PaginationMeta, bool)`

GetMetaOk returns a tuple with the Meta field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMeta

`func (o *CityListResponse) SetMeta(v PaginationMeta)`

SetMeta sets Meta field to given value.

### HasMeta

`func (o *CityListResponse) HasMeta() bool`

HasMeta returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


