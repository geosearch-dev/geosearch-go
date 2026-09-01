# Country

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int64** |  | [optional] 
**GeonameId** | Pointer to **int64** |  | [optional] 
**IsoCode** | Pointer to **string** |  | [optional] 
**Iso3Code** | Pointer to **string** |  | [optional] 
**IsoNumeric** | Pointer to **int32** |  | [optional] 
**FipsCode** | Pointer to **string** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**Capital** | Pointer to **string** |  | [optional] 
**AreaSqKm** | Pointer to **float64** |  | [optional] 
**Population** | Pointer to **int64** |  | [optional] 
**ContinentCode** | Pointer to **string** |  | [optional] 
**Tld** | Pointer to **string** |  | [optional] 
**CurrencyCode** | Pointer to **string** |  | [optional] 
**CurrencyName** | Pointer to **string** |  | [optional] 
**Phone** | Pointer to **string** |  | [optional] 
**PostalCodeFormat** | Pointer to **string** |  | [optional] 
**PostalCodeRegex** | Pointer to **string** |  | [optional] 
**Languages** | Pointer to **[]string** |  | [optional] 
**Neighbours** | Pointer to **[]string** |  | [optional] 
**Latitude** | Pointer to **float64** |  | [optional] 
**Longitude** | Pointer to **float64** |  | [optional] 
**FlagEmoji** | Pointer to **string** |  | [optional] 
**Geometry** | Pointer to [**GeoJSONMultiPolygon**](GeoJSONMultiPolygon.md) | Country boundary. Returned by default on &#x60;GET /v1/countries/{code}&#x60; and on request via &#x60;?fields&#x3D;geometry&#x60; on &#x60;GET /v1/countries&#x60;.  NOT TIER-GATED. Country geometry is served on every plan, including Free. Region geometry is gated — see the &#x60;Region&#x60; schema. | [optional] 

## Methods

### NewCountry

`func NewCountry() *Country`

NewCountry instantiates a new Country object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCountryWithDefaults

`func NewCountryWithDefaults() *Country`

NewCountryWithDefaults instantiates a new Country object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Country) GetId() int64`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Country) GetIdOk() (*int64, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Country) SetId(v int64)`

SetId sets Id field to given value.

### HasId

`func (o *Country) HasId() bool`

HasId returns a boolean if a field has been set.

### GetGeonameId

`func (o *Country) GetGeonameId() int64`

GetGeonameId returns the GeonameId field if non-nil, zero value otherwise.

### GetGeonameIdOk

`func (o *Country) GetGeonameIdOk() (*int64, bool)`

GetGeonameIdOk returns a tuple with the GeonameId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGeonameId

`func (o *Country) SetGeonameId(v int64)`

SetGeonameId sets GeonameId field to given value.

### HasGeonameId

`func (o *Country) HasGeonameId() bool`

HasGeonameId returns a boolean if a field has been set.

### GetIsoCode

`func (o *Country) GetIsoCode() string`

GetIsoCode returns the IsoCode field if non-nil, zero value otherwise.

### GetIsoCodeOk

`func (o *Country) GetIsoCodeOk() (*string, bool)`

GetIsoCodeOk returns a tuple with the IsoCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsoCode

`func (o *Country) SetIsoCode(v string)`

SetIsoCode sets IsoCode field to given value.

### HasIsoCode

`func (o *Country) HasIsoCode() bool`

HasIsoCode returns a boolean if a field has been set.

### GetIso3Code

`func (o *Country) GetIso3Code() string`

GetIso3Code returns the Iso3Code field if non-nil, zero value otherwise.

### GetIso3CodeOk

`func (o *Country) GetIso3CodeOk() (*string, bool)`

GetIso3CodeOk returns a tuple with the Iso3Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIso3Code

`func (o *Country) SetIso3Code(v string)`

SetIso3Code sets Iso3Code field to given value.

### HasIso3Code

`func (o *Country) HasIso3Code() bool`

HasIso3Code returns a boolean if a field has been set.

### GetIsoNumeric

`func (o *Country) GetIsoNumeric() int32`

GetIsoNumeric returns the IsoNumeric field if non-nil, zero value otherwise.

### GetIsoNumericOk

`func (o *Country) GetIsoNumericOk() (*int32, bool)`

GetIsoNumericOk returns a tuple with the IsoNumeric field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsoNumeric

`func (o *Country) SetIsoNumeric(v int32)`

SetIsoNumeric sets IsoNumeric field to given value.

### HasIsoNumeric

`func (o *Country) HasIsoNumeric() bool`

HasIsoNumeric returns a boolean if a field has been set.

### GetFipsCode

`func (o *Country) GetFipsCode() string`

GetFipsCode returns the FipsCode field if non-nil, zero value otherwise.

### GetFipsCodeOk

`func (o *Country) GetFipsCodeOk() (*string, bool)`

GetFipsCodeOk returns a tuple with the FipsCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFipsCode

`func (o *Country) SetFipsCode(v string)`

SetFipsCode sets FipsCode field to given value.

### HasFipsCode

`func (o *Country) HasFipsCode() bool`

HasFipsCode returns a boolean if a field has been set.

### GetName

`func (o *Country) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Country) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Country) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *Country) HasName() bool`

HasName returns a boolean if a field has been set.

### GetCapital

`func (o *Country) GetCapital() string`

GetCapital returns the Capital field if non-nil, zero value otherwise.

### GetCapitalOk

`func (o *Country) GetCapitalOk() (*string, bool)`

GetCapitalOk returns a tuple with the Capital field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCapital

`func (o *Country) SetCapital(v string)`

SetCapital sets Capital field to given value.

### HasCapital

`func (o *Country) HasCapital() bool`

HasCapital returns a boolean if a field has been set.

### GetAreaSqKm

`func (o *Country) GetAreaSqKm() float64`

GetAreaSqKm returns the AreaSqKm field if non-nil, zero value otherwise.

### GetAreaSqKmOk

`func (o *Country) GetAreaSqKmOk() (*float64, bool)`

GetAreaSqKmOk returns a tuple with the AreaSqKm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAreaSqKm

`func (o *Country) SetAreaSqKm(v float64)`

SetAreaSqKm sets AreaSqKm field to given value.

### HasAreaSqKm

`func (o *Country) HasAreaSqKm() bool`

HasAreaSqKm returns a boolean if a field has been set.

### GetPopulation

`func (o *Country) GetPopulation() int64`

GetPopulation returns the Population field if non-nil, zero value otherwise.

### GetPopulationOk

`func (o *Country) GetPopulationOk() (*int64, bool)`

GetPopulationOk returns a tuple with the Population field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPopulation

`func (o *Country) SetPopulation(v int64)`

SetPopulation sets Population field to given value.

### HasPopulation

`func (o *Country) HasPopulation() bool`

HasPopulation returns a boolean if a field has been set.

### GetContinentCode

`func (o *Country) GetContinentCode() string`

GetContinentCode returns the ContinentCode field if non-nil, zero value otherwise.

### GetContinentCodeOk

`func (o *Country) GetContinentCodeOk() (*string, bool)`

GetContinentCodeOk returns a tuple with the ContinentCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContinentCode

`func (o *Country) SetContinentCode(v string)`

SetContinentCode sets ContinentCode field to given value.

### HasContinentCode

`func (o *Country) HasContinentCode() bool`

HasContinentCode returns a boolean if a field has been set.

### GetTld

`func (o *Country) GetTld() string`

GetTld returns the Tld field if non-nil, zero value otherwise.

### GetTldOk

`func (o *Country) GetTldOk() (*string, bool)`

GetTldOk returns a tuple with the Tld field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTld

`func (o *Country) SetTld(v string)`

SetTld sets Tld field to given value.

### HasTld

`func (o *Country) HasTld() bool`

HasTld returns a boolean if a field has been set.

### GetCurrencyCode

`func (o *Country) GetCurrencyCode() string`

GetCurrencyCode returns the CurrencyCode field if non-nil, zero value otherwise.

### GetCurrencyCodeOk

`func (o *Country) GetCurrencyCodeOk() (*string, bool)`

GetCurrencyCodeOk returns a tuple with the CurrencyCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrencyCode

`func (o *Country) SetCurrencyCode(v string)`

SetCurrencyCode sets CurrencyCode field to given value.

### HasCurrencyCode

`func (o *Country) HasCurrencyCode() bool`

HasCurrencyCode returns a boolean if a field has been set.

### GetCurrencyName

`func (o *Country) GetCurrencyName() string`

GetCurrencyName returns the CurrencyName field if non-nil, zero value otherwise.

### GetCurrencyNameOk

`func (o *Country) GetCurrencyNameOk() (*string, bool)`

GetCurrencyNameOk returns a tuple with the CurrencyName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrencyName

`func (o *Country) SetCurrencyName(v string)`

SetCurrencyName sets CurrencyName field to given value.

### HasCurrencyName

`func (o *Country) HasCurrencyName() bool`

HasCurrencyName returns a boolean if a field has been set.

### GetPhone

`func (o *Country) GetPhone() string`

GetPhone returns the Phone field if non-nil, zero value otherwise.

### GetPhoneOk

`func (o *Country) GetPhoneOk() (*string, bool)`

GetPhoneOk returns a tuple with the Phone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhone

`func (o *Country) SetPhone(v string)`

SetPhone sets Phone field to given value.

### HasPhone

`func (o *Country) HasPhone() bool`

HasPhone returns a boolean if a field has been set.

### GetPostalCodeFormat

`func (o *Country) GetPostalCodeFormat() string`

GetPostalCodeFormat returns the PostalCodeFormat field if non-nil, zero value otherwise.

### GetPostalCodeFormatOk

`func (o *Country) GetPostalCodeFormatOk() (*string, bool)`

GetPostalCodeFormatOk returns a tuple with the PostalCodeFormat field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostalCodeFormat

`func (o *Country) SetPostalCodeFormat(v string)`

SetPostalCodeFormat sets PostalCodeFormat field to given value.

### HasPostalCodeFormat

`func (o *Country) HasPostalCodeFormat() bool`

HasPostalCodeFormat returns a boolean if a field has been set.

### GetPostalCodeRegex

`func (o *Country) GetPostalCodeRegex() string`

GetPostalCodeRegex returns the PostalCodeRegex field if non-nil, zero value otherwise.

### GetPostalCodeRegexOk

`func (o *Country) GetPostalCodeRegexOk() (*string, bool)`

GetPostalCodeRegexOk returns a tuple with the PostalCodeRegex field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostalCodeRegex

`func (o *Country) SetPostalCodeRegex(v string)`

SetPostalCodeRegex sets PostalCodeRegex field to given value.

### HasPostalCodeRegex

`func (o *Country) HasPostalCodeRegex() bool`

HasPostalCodeRegex returns a boolean if a field has been set.

### GetLanguages

`func (o *Country) GetLanguages() []string`

GetLanguages returns the Languages field if non-nil, zero value otherwise.

### GetLanguagesOk

`func (o *Country) GetLanguagesOk() (*[]string, bool)`

GetLanguagesOk returns a tuple with the Languages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLanguages

`func (o *Country) SetLanguages(v []string)`

SetLanguages sets Languages field to given value.

### HasLanguages

`func (o *Country) HasLanguages() bool`

HasLanguages returns a boolean if a field has been set.

### GetNeighbours

`func (o *Country) GetNeighbours() []string`

GetNeighbours returns the Neighbours field if non-nil, zero value otherwise.

### GetNeighboursOk

`func (o *Country) GetNeighboursOk() (*[]string, bool)`

GetNeighboursOk returns a tuple with the Neighbours field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNeighbours

`func (o *Country) SetNeighbours(v []string)`

SetNeighbours sets Neighbours field to given value.

### HasNeighbours

`func (o *Country) HasNeighbours() bool`

HasNeighbours returns a boolean if a field has been set.

### GetLatitude

`func (o *Country) GetLatitude() float64`

GetLatitude returns the Latitude field if non-nil, zero value otherwise.

### GetLatitudeOk

`func (o *Country) GetLatitudeOk() (*float64, bool)`

GetLatitudeOk returns a tuple with the Latitude field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatitude

`func (o *Country) SetLatitude(v float64)`

SetLatitude sets Latitude field to given value.

### HasLatitude

`func (o *Country) HasLatitude() bool`

HasLatitude returns a boolean if a field has been set.

### GetLongitude

`func (o *Country) GetLongitude() float64`

GetLongitude returns the Longitude field if non-nil, zero value otherwise.

### GetLongitudeOk

`func (o *Country) GetLongitudeOk() (*float64, bool)`

GetLongitudeOk returns a tuple with the Longitude field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLongitude

`func (o *Country) SetLongitude(v float64)`

SetLongitude sets Longitude field to given value.

### HasLongitude

`func (o *Country) HasLongitude() bool`

HasLongitude returns a boolean if a field has been set.

### GetFlagEmoji

`func (o *Country) GetFlagEmoji() string`

GetFlagEmoji returns the FlagEmoji field if non-nil, zero value otherwise.

### GetFlagEmojiOk

`func (o *Country) GetFlagEmojiOk() (*string, bool)`

GetFlagEmojiOk returns a tuple with the FlagEmoji field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFlagEmoji

`func (o *Country) SetFlagEmoji(v string)`

SetFlagEmoji sets FlagEmoji field to given value.

### HasFlagEmoji

`func (o *Country) HasFlagEmoji() bool`

HasFlagEmoji returns a boolean if a field has been set.

### GetGeometry

`func (o *Country) GetGeometry() GeoJSONMultiPolygon`

GetGeometry returns the Geometry field if non-nil, zero value otherwise.

### GetGeometryOk

`func (o *Country) GetGeometryOk() (*GeoJSONMultiPolygon, bool)`

GetGeometryOk returns a tuple with the Geometry field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGeometry

`func (o *Country) SetGeometry(v GeoJSONMultiPolygon)`

SetGeometry sets Geometry field to given value.

### HasGeometry

`func (o *Country) HasGeometry() bool`

HasGeometry returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


