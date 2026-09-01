# HierarchyListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | Pointer to [**[]HierarchyNode**](HierarchyNode.md) |  | [optional] 
**Meta** | Pointer to [**PaginationMeta**](PaginationMeta.md) |  | [optional] 

## Methods

### NewHierarchyListResponse

`func NewHierarchyListResponse() *HierarchyListResponse`

NewHierarchyListResponse instantiates a new HierarchyListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewHierarchyListResponseWithDefaults

`func NewHierarchyListResponseWithDefaults() *HierarchyListResponse`

NewHierarchyListResponseWithDefaults instantiates a new HierarchyListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *HierarchyListResponse) GetData() []HierarchyNode`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *HierarchyListResponse) GetDataOk() (*[]HierarchyNode, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *HierarchyListResponse) SetData(v []HierarchyNode)`

SetData sets Data field to given value.

### HasData

`func (o *HierarchyListResponse) HasData() bool`

HasData returns a boolean if a field has been set.

### GetMeta

`func (o *HierarchyListResponse) GetMeta() PaginationMeta`

GetMeta returns the Meta field if non-nil, zero value otherwise.

### GetMetaOk

`func (o *HierarchyListResponse) GetMetaOk() (*PaginationMeta, bool)`

GetMetaOk returns a tuple with the Meta field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMeta

`func (o *HierarchyListResponse) SetMeta(v PaginationMeta)`

SetMeta sets Meta field to given value.

### HasMeta

`func (o *HierarchyListResponse) HasMeta() bool`

HasMeta returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


