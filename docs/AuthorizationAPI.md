# \AuthorizationAPI

All URIs are relative to *https://sellingpartnerapi-na.amazon.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetAuthorizationCode**](AuthorizationAPI.md#GetAuthorizationCode) | **Get** /authorization/v1/authorizationCode | Returns the Login with Amazon (LWA) authorization code for an existing Amazon MWS authorization.



## GetAuthorizationCode

> GetAuthorizationCodeResponse GetAuthorizationCode(ctx).SellingPartnerId(sellingPartnerId).DeveloperId(developerId).MwsAuthToken(mwsAuthToken).Execute()

Returns the Login with Amazon (LWA) authorization code for an existing Amazon MWS authorization.



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "github.com//phoenis-maha/sp-authorization"
)

func main() {
    sellingPartnerId := "sellingPartnerId_example" // string | The seller ID of the seller for whom you are requesting Selling Partner API authorization. This must be the seller ID of the seller who authorized your application on the Marketplace Appstore.
    developerId := "developerId_example" // string | Your developer ID. This must be one of the developer ID values that you provided when you registered your application in Developer Central.
    mwsAuthToken := "mwsAuthToken_example" // string | The MWS Auth Token that was generated when the seller authorized your application on the Marketplace Appstore.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.AuthorizationAPI.GetAuthorizationCode(context.Background()).SellingPartnerId(sellingPartnerId).DeveloperId(developerId).MwsAuthToken(mwsAuthToken).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `AuthorizationAPI.GetAuthorizationCode``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetAuthorizationCode`: GetAuthorizationCodeResponse
    fmt.Fprintf(os.Stdout, "Response from `AuthorizationAPI.GetAuthorizationCode`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetAuthorizationCodeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sellingPartnerId** | **string** | The seller ID of the seller for whom you are requesting Selling Partner API authorization. This must be the seller ID of the seller who authorized your application on the Marketplace Appstore. | 
 **developerId** | **string** | Your developer ID. This must be one of the developer ID values that you provided when you registered your application in Developer Central. | 
 **mwsAuthToken** | **string** | The MWS Auth Token that was generated when the seller authorized your application on the Marketplace Appstore. | 

### Return type

[**GetAuthorizationCodeResponse**](GetAuthorizationCodeResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, payload, errors

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

