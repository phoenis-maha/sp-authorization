# GetAuthorizationCodeResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Payload** | Pointer to [**AuthorizationCode**](AuthorizationCode.md) |  | [optional] 
**Errors** | Pointer to [**[]Error**](Error.md) | A list of error responses returned when a request is unsuccessful. | [optional] 

## Methods

### NewGetAuthorizationCodeResponse

`func NewGetAuthorizationCodeResponse() *GetAuthorizationCodeResponse`

NewGetAuthorizationCodeResponse instantiates a new GetAuthorizationCodeResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetAuthorizationCodeResponseWithDefaults

`func NewGetAuthorizationCodeResponseWithDefaults() *GetAuthorizationCodeResponse`

NewGetAuthorizationCodeResponseWithDefaults instantiates a new GetAuthorizationCodeResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPayload

`func (o *GetAuthorizationCodeResponse) GetPayload() AuthorizationCode`

GetPayload returns the Payload field if non-nil, zero value otherwise.

### GetPayloadOk

`func (o *GetAuthorizationCodeResponse) GetPayloadOk() (*AuthorizationCode, bool)`

GetPayloadOk returns a tuple with the Payload field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPayload

`func (o *GetAuthorizationCodeResponse) SetPayload(v AuthorizationCode)`

SetPayload sets Payload field to given value.

### HasPayload

`func (o *GetAuthorizationCodeResponse) HasPayload() bool`

HasPayload returns a boolean if a field has been set.

### GetErrors

`func (o *GetAuthorizationCodeResponse) GetErrors() []Error`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *GetAuthorizationCodeResponse) GetErrorsOk() (*[]Error, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *GetAuthorizationCodeResponse) SetErrors(v []Error)`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *GetAuthorizationCodeResponse) HasErrors() bool`

HasErrors returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


