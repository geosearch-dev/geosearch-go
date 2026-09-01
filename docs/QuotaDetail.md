# QuotaDetail

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Limit** | **int64** | Monthly request allowance for the account&#39;s current plan. | 
**Used** | **int64** | Requests consumed in the current quota period. | 
**ResetsAt** | **time.Time** | Start of the next quota period, when &#x60;used&#x60; returns to zero. Matches the &#x60;X-RateLimit-Reset&#x60; header on the same response, expressed as RFC 3339 rather than an epoch second. | 
**UpgradeUrl** | **string** | Absolute URL of the billing page where the plan can be raised. Derived server-side from configuration and never reflected from a request header or parameter. | 

## Methods

### NewQuotaDetail

`func NewQuotaDetail(limit int64, used int64, resetsAt time.Time, upgradeUrl string, ) *QuotaDetail`

NewQuotaDetail instantiates a new QuotaDetail object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewQuotaDetailWithDefaults

`func NewQuotaDetailWithDefaults() *QuotaDetail`

NewQuotaDetailWithDefaults instantiates a new QuotaDetail object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLimit

`func (o *QuotaDetail) GetLimit() int64`

GetLimit returns the Limit field if non-nil, zero value otherwise.

### GetLimitOk

`func (o *QuotaDetail) GetLimitOk() (*int64, bool)`

GetLimitOk returns a tuple with the Limit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimit

`func (o *QuotaDetail) SetLimit(v int64)`

SetLimit sets Limit field to given value.


### GetUsed

`func (o *QuotaDetail) GetUsed() int64`

GetUsed returns the Used field if non-nil, zero value otherwise.

### GetUsedOk

`func (o *QuotaDetail) GetUsedOk() (*int64, bool)`

GetUsedOk returns a tuple with the Used field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsed

`func (o *QuotaDetail) SetUsed(v int64)`

SetUsed sets Used field to given value.


### GetResetsAt

`func (o *QuotaDetail) GetResetsAt() time.Time`

GetResetsAt returns the ResetsAt field if non-nil, zero value otherwise.

### GetResetsAtOk

`func (o *QuotaDetail) GetResetsAtOk() (*time.Time, bool)`

GetResetsAtOk returns a tuple with the ResetsAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResetsAt

`func (o *QuotaDetail) SetResetsAt(v time.Time)`

SetResetsAt sets ResetsAt field to given value.


### GetUpgradeUrl

`func (o *QuotaDetail) GetUpgradeUrl() string`

GetUpgradeUrl returns the UpgradeUrl field if non-nil, zero value otherwise.

### GetUpgradeUrlOk

`func (o *QuotaDetail) GetUpgradeUrlOk() (*string, bool)`

GetUpgradeUrlOk returns a tuple with the UpgradeUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpgradeUrl

`func (o *QuotaDetail) SetUpgradeUrl(v string)`

SetUpgradeUrl sets UpgradeUrl field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


