# Boundary

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**GeonameId** | **int64** | The area the polygon belongs to, read back from the source row rather than echoed from the request. | 
**Name** | **string** | The area&#39;s name, resolved through &#x60;?lang&#x3D;&#x60; when supplied. | 
**Type** | **string** | Which kind of area this is. | 
**Geometry** | [**GeoJSONGeometry**](GeoJSONGeometry.md) |  | 
**Simplify** | **float64** | The tolerance that was ACTUALLY APPLIED, or &#x60;null&#x60; for full precision.  THIS IS NOT YOUR &#x60;?simplify&#x3D;&#x60; ECHOED BACK. A requested tolerance of &#x60;0&#x60; is dropped rather than executed, so &#x60;?simplify&#x3D;0&#x60; returns &#x60;null&#x60; here — that is the truthful answer, because no simplification was performed. Read this field rather than assuming the request was honoured verbatim. | 

## Methods

### NewBoundary

`func NewBoundary(geonameId int64, name string, type_ string, geometry GeoJSONGeometry, simplify float64, ) *Boundary`

NewBoundary instantiates a new Boundary object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBoundaryWithDefaults

`func NewBoundaryWithDefaults() *Boundary`

NewBoundaryWithDefaults instantiates a new Boundary object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetGeonameId

`func (o *Boundary) GetGeonameId() int64`

GetGeonameId returns the GeonameId field if non-nil, zero value otherwise.

### GetGeonameIdOk

`func (o *Boundary) GetGeonameIdOk() (*int64, bool)`

GetGeonameIdOk returns a tuple with the GeonameId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGeonameId

`func (o *Boundary) SetGeonameId(v int64)`

SetGeonameId sets GeonameId field to given value.


### GetName

`func (o *Boundary) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Boundary) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Boundary) SetName(v string)`

SetName sets Name field to given value.


### GetType

`func (o *Boundary) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *Boundary) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *Boundary) SetType(v string)`

SetType sets Type field to given value.


### GetGeometry

`func (o *Boundary) GetGeometry() GeoJSONGeometry`

GetGeometry returns the Geometry field if non-nil, zero value otherwise.

### GetGeometryOk

`func (o *Boundary) GetGeometryOk() (*GeoJSONGeometry, bool)`

GetGeometryOk returns a tuple with the Geometry field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGeometry

`func (o *Boundary) SetGeometry(v GeoJSONGeometry)`

SetGeometry sets Geometry field to given value.


### GetSimplify

`func (o *Boundary) GetSimplify() float64`

GetSimplify returns the Simplify field if non-nil, zero value otherwise.

### GetSimplifyOk

`func (o *Boundary) GetSimplifyOk() (*float64, bool)`

GetSimplifyOk returns a tuple with the Simplify field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSimplify

`func (o *Boundary) SetSimplify(v float64)`

SetSimplify sets Simplify field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


