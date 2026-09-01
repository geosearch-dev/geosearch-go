# PostalCodeListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | Pointer to [**[]PostalCode**](PostalCode.md) |  | [optional] 
**Meta** | Pointer to [**PaginationMeta**](PaginationMeta.md) |  | [optional] 

## Methods

### NewPostalCodeListResponse

`func NewPostalCodeListResponse() *PostalCodeListResponse`

NewPostalCodeListResponse instantiates a new PostalCodeListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPostalCodeListResponseWithDefaults

`func NewPostalCodeListResponseWithDefaults() *PostalCodeListResponse`

NewPostalCodeListResponseWithDefaults instantiates a new PostalCodeListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *PostalCodeListResponse) GetData() []PostalCode`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *PostalCodeListResponse) GetDataOk() (*[]PostalCode, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *PostalCodeListResponse) SetData(v []PostalCode)`

SetData sets Data field to given value.

### HasData

`func (o *PostalCodeListResponse) HasData() bool`

HasData returns a boolean if a field has been set.

### GetMeta

`func (o *PostalCodeListResponse) GetMeta() PaginationMeta`

GetMeta returns the Meta field if non-nil, zero value otherwise.

### GetMetaOk

`func (o *PostalCodeListResponse) GetMetaOk() (*PaginationMeta, bool)`

GetMetaOk returns a tuple with the Meta field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMeta

`func (o *PostalCodeListResponse) SetMeta(v PaginationMeta)`

SetMeta sets Meta field to given value.

### HasMeta

`func (o *PostalCodeListResponse) HasMeta() bool`

HasMeta returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


