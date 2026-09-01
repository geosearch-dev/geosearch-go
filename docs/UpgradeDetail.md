# UpgradeDetail

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**UpgradeUrl** | **string** | Absolute URL of the billing page where the plan can be raised. Derived server-side from configuration and never reflected from a request header or parameter. | 

## Methods

### NewUpgradeDetail

`func NewUpgradeDetail(upgradeUrl string, ) *UpgradeDetail`

NewUpgradeDetail instantiates a new UpgradeDetail object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpgradeDetailWithDefaults

`func NewUpgradeDetailWithDefaults() *UpgradeDetail`

NewUpgradeDetailWithDefaults instantiates a new UpgradeDetail object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUpgradeUrl

`func (o *UpgradeDetail) GetUpgradeUrl() string`

GetUpgradeUrl returns the UpgradeUrl field if non-nil, zero value otherwise.

### GetUpgradeUrlOk

`func (o *UpgradeDetail) GetUpgradeUrlOk() (*string, bool)`

GetUpgradeUrlOk returns a tuple with the UpgradeUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpgradeUrl

`func (o *UpgradeDetail) SetUpgradeUrl(v string)`

SetUpgradeUrl sets UpgradeUrl field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


