# PartnerMerchantControllerApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getMerchantStatus**](PartnerMerchantControllerApi.md#getMerchantStatus) | **GET** /partners/merchants/{merchantId}/status |  |
| [**listMerchants**](PartnerMerchantControllerApi.md#listMerchants) | **GET** /partners/merchants |  |
| [**onboardMerchant**](PartnerMerchantControllerApi.md#onboardMerchant) | **POST** /partners/merchants |  |


<a id="getMerchantStatus"></a>
# **getMerchantStatus**
> MerchantOnboardingStatus getMerchantStatus(merchantId, acceptLanguage)



### Example
```java
// Import classes:
import com.zipper.auth.sdk.ApiClient;
import com.zipper.auth.sdk.ApiException;
import com.zipper.auth.sdk.Configuration;
import com.zipper.auth.sdk.auth.*;
import com.zipper.auth.sdk.models.*;
import com.zipper.auth.sdk.api.PartnerMerchantControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");
    
    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    PartnerMerchantControllerApi apiInstance = new PartnerMerchantControllerApi(defaultClient);
    UUID merchantId = UUID.randomUUID(); // UUID | 
    String acceptLanguage = "en"; // String | Language preference for response content. Supported: en, he
    try {
      MerchantOnboardingStatus result = apiInstance.getMerchantStatus(merchantId, acceptLanguage);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling PartnerMerchantControllerApi#getMerchantStatus");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **merchantId** | **UUID**|  | |
| **acceptLanguage** | **String**| Language preference for response content. Supported: en, he | [optional] [default to en] [enum: en, he] |

### Return type

[**MerchantOnboardingStatus**](MerchantOnboardingStatus.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a id="listMerchants"></a>
# **listMerchants**
> PageMerchantSummary listMerchants(pageable, acceptLanguage)



### Example
```java
// Import classes:
import com.zipper.auth.sdk.ApiClient;
import com.zipper.auth.sdk.ApiException;
import com.zipper.auth.sdk.Configuration;
import com.zipper.auth.sdk.auth.*;
import com.zipper.auth.sdk.models.*;
import com.zipper.auth.sdk.api.PartnerMerchantControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");
    
    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    PartnerMerchantControllerApi apiInstance = new PartnerMerchantControllerApi(defaultClient);
    Pageable pageable = new Pageable(); // Pageable | 
    String acceptLanguage = "en"; // String | Language preference for response content. Supported: en, he
    try {
      PageMerchantSummary result = apiInstance.listMerchants(pageable, acceptLanguage);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling PartnerMerchantControllerApi#listMerchants");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **pageable** | [**Pageable**](.md)|  | |
| **acceptLanguage** | **String**| Language preference for response content. Supported: en, he | [optional] [default to en] [enum: en, he] |

### Return type

[**PageMerchantSummary**](PageMerchantSummary.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a id="onboardMerchant"></a>
# **onboardMerchant**
> PartnerOnboardingResult onboardMerchant(merchantOnboardingRequest, acceptLanguage)



### Example
```java
// Import classes:
import com.zipper.auth.sdk.ApiClient;
import com.zipper.auth.sdk.ApiException;
import com.zipper.auth.sdk.Configuration;
import com.zipper.auth.sdk.auth.*;
import com.zipper.auth.sdk.models.*;
import com.zipper.auth.sdk.api.PartnerMerchantControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");
    
    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    PartnerMerchantControllerApi apiInstance = new PartnerMerchantControllerApi(defaultClient);
    MerchantOnboardingRequest merchantOnboardingRequest = new MerchantOnboardingRequest(); // MerchantOnboardingRequest | 
    String acceptLanguage = "en"; // String | Language preference for response content. Supported: en, he
    try {
      PartnerOnboardingResult result = apiInstance.onboardMerchant(merchantOnboardingRequest, acceptLanguage);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling PartnerMerchantControllerApi#onboardMerchant");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **merchantOnboardingRequest** | [**MerchantOnboardingRequest**](MerchantOnboardingRequest.md)|  | |
| **acceptLanguage** | **String**| Language preference for response content. Supported: en, he | [optional] [default to en] [enum: en, he] |

### Return type

[**PartnerOnboardingResult**](PartnerOnboardingResult.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

