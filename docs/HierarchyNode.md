# HierarchyNode

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**GeonameId** | Pointer to **int64** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**Type** | Pointer to **string** |  | [optional] 
**Depth** | Pointer to **int32** | THE DIRECTION DEPENDS ON THE ENDPOINT, because this schema is shared by two operations that number their nodes from opposite ends.  On &#x60;GET /v1/cities/{id}/hierarchy&#x60; depth counts UP from the entity asked about: &#x60;depth: 0&#x60; is the city and the country carries the HIGHEST depth. On &#x60;GET /v1/resolve&#x60; depth is POSITIONAL, counting outward-in: &#x60;depth: 0&#x60; is the COUNTRY. Code that sorts or indexes on this field across both endpoints without accounting for the inversion silently REVERSES the hierarchy rather than failing — &#x60;max(by: depth)&#x60; returns the country on one and the innermost region on the other.  On &#x60;/v1/resolve&#x60; depth is the ARRAY INDEX and NOT an administrative level. A chain may skip a level: a measured 3.8% of coordinates resolve to a country plus a level-2 region with no level-1 region, and in those &#x60;depth: 1&#x60; is a level-2 area. &#x60;HierarchyNode&#x60; carries no &#x60;level&#x60; field, so there is no second signal to disambiguate with — treat depth as position only. | [optional] 

## Methods

### NewHierarchyNode

`func NewHierarchyNode() *HierarchyNode`

NewHierarchyNode instantiates a new HierarchyNode object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewHierarchyNodeWithDefaults

`func NewHierarchyNodeWithDefaults() *HierarchyNode`

NewHierarchyNodeWithDefaults instantiates a new HierarchyNode object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetGeonameId

`func (o *HierarchyNode) GetGeonameId() int64`

GetGeonameId returns the GeonameId field if non-nil, zero value otherwise.

### GetGeonameIdOk

`func (o *HierarchyNode) GetGeonameIdOk() (*int64, bool)`

GetGeonameIdOk returns a tuple with the GeonameId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGeonameId

`func (o *HierarchyNode) SetGeonameId(v int64)`

SetGeonameId sets GeonameId field to given value.

### HasGeonameId

`func (o *HierarchyNode) HasGeonameId() bool`

HasGeonameId returns a boolean if a field has been set.

### GetName

`func (o *HierarchyNode) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *HierarchyNode) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *HierarchyNode) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *HierarchyNode) HasName() bool`

HasName returns a boolean if a field has been set.

### GetType

`func (o *HierarchyNode) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *HierarchyNode) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *HierarchyNode) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *HierarchyNode) HasType() bool`

HasType returns a boolean if a field has been set.

### GetDepth

`func (o *HierarchyNode) GetDepth() int32`

GetDepth returns the Depth field if non-nil, zero value otherwise.

### GetDepthOk

`func (o *HierarchyNode) GetDepthOk() (*int32, bool)`

GetDepthOk returns a tuple with the Depth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDepth

`func (o *HierarchyNode) SetDepth(v int32)`

SetDepth sets Depth field to given value.

### HasDepth

`func (o *HierarchyNode) HasDepth() bool`

HasDepth returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


