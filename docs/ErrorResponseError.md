# ErrorResponseError

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Code** | **string** |  | 
**Message** | **string** |  | 
**Details** | Pointer to [**[]ErrorResponseErrorDetailsInner**](ErrorResponseErrorDetailsInner.md) |  | [optional] 
**RequestId** | **string** | Correlation identifier present on every error response. Quote this when contacting support. | 
**TraceId** | Pointer to **string** | W3C trace ID of the distributed trace for this request, when tracing is enabled. Omitted entirely when no span was recording, so clients must treat it as optional. It complements rather than replaces &#x60;request_id&#x60;. | [optional] 
**Quota** | Pointer to [**QuotaDetail**](QuotaDetail.md) |  | [optional] 
**Upgrade** | Pointer to [**UpgradeDetail**](UpgradeDetail.md) |  | [optional] 

## Methods

### NewErrorResponseError

`func NewErrorResponseError(code string, message string, requestId string, ) *ErrorResponseError`

NewErrorResponseError instantiates a new ErrorResponseError object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewErrorResponseErrorWithDefaults

`func NewErrorResponseErrorWithDefaults() *ErrorResponseError`

NewErrorResponseErrorWithDefaults instantiates a new ErrorResponseError object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCode

`func (o *ErrorResponseError) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *ErrorResponseError) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *ErrorResponseError) SetCode(v string)`

SetCode sets Code field to given value.


### GetMessage

`func (o *ErrorResponseError) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *ErrorResponseError) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *ErrorResponseError) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetDetails

`func (o *ErrorResponseError) GetDetails() []ErrorResponseErrorDetailsInner`

GetDetails returns the Details field if non-nil, zero value otherwise.

### GetDetailsOk

`func (o *ErrorResponseError) GetDetailsOk() (*[]ErrorResponseErrorDetailsInner, bool)`

GetDetailsOk returns a tuple with the Details field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDetails

`func (o *ErrorResponseError) SetDetails(v []ErrorResponseErrorDetailsInner)`

SetDetails sets Details field to given value.

### HasDetails

`func (o *ErrorResponseError) HasDetails() bool`

HasDetails returns a boolean if a field has been set.

### GetRequestId

`func (o *ErrorResponseError) GetRequestId() string`

GetRequestId returns the RequestId field if non-nil, zero value otherwise.

### GetRequestIdOk

`func (o *ErrorResponseError) GetRequestIdOk() (*string, bool)`

GetRequestIdOk returns a tuple with the RequestId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequestId

`func (o *ErrorResponseError) SetRequestId(v string)`

SetRequestId sets RequestId field to given value.


### GetTraceId

`func (o *ErrorResponseError) GetTraceId() string`

GetTraceId returns the TraceId field if non-nil, zero value otherwise.

### GetTraceIdOk

`func (o *ErrorResponseError) GetTraceIdOk() (*string, bool)`

GetTraceIdOk returns a tuple with the TraceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTraceId

`func (o *ErrorResponseError) SetTraceId(v string)`

SetTraceId sets TraceId field to given value.

### HasTraceId

`func (o *ErrorResponseError) HasTraceId() bool`

HasTraceId returns a boolean if a field has been set.

### GetQuota

`func (o *ErrorResponseError) GetQuota() QuotaDetail`

GetQuota returns the Quota field if non-nil, zero value otherwise.

### GetQuotaOk

`func (o *ErrorResponseError) GetQuotaOk() (*QuotaDetail, bool)`

GetQuotaOk returns a tuple with the Quota field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuota

`func (o *ErrorResponseError) SetQuota(v QuotaDetail)`

SetQuota sets Quota field to given value.

### HasQuota

`func (o *ErrorResponseError) HasQuota() bool`

HasQuota returns a boolean if a field has been set.

### GetUpgrade

`func (o *ErrorResponseError) GetUpgrade() UpgradeDetail`

GetUpgrade returns the Upgrade field if non-nil, zero value otherwise.

### GetUpgradeOk

`func (o *ErrorResponseError) GetUpgradeOk() (*UpgradeDetail, bool)`

GetUpgradeOk returns a tuple with the Upgrade field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpgrade

`func (o *ErrorResponseError) SetUpgrade(v UpgradeDetail)`

SetUpgrade sets Upgrade field to given value.

### HasUpgrade

`func (o *ErrorResponseError) HasUpgrade() bool`

HasUpgrade returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


