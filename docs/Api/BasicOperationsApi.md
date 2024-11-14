# OpenAPI\Client\BasicOperationsApi

All URIs are relative to https://urlmanager.api.gogemini.io, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**urlManagerChangeUrlRewriteRequestPath()**](BasicOperationsApi.md#urlManagerChangeUrlRewriteRequestPath) | **POST** /urlmanager/change_url_rewrite_request_path | Change Url Rewrite Request Path |
| [**urlManagerChangeUrlRewriteRequestPath2()**](BasicOperationsApi.md#urlManagerChangeUrlRewriteRequestPath2) | **POST** /urlmanager.UrlManager/ChangeUrlRewriteRequestPath | Change Url Rewrite Request Path |
| [**urlManagerCreateUrlRewrite()**](BasicOperationsApi.md#urlManagerCreateUrlRewrite) | **POST** /urlmanager/create_url_rewrite | Create Url Rewrite |
| [**urlManagerCreateUrlRewrite2()**](BasicOperationsApi.md#urlManagerCreateUrlRewrite2) | **POST** /urlmanager.UrlManager/CreateUrlRewrite | Create Url Rewrite |
| [**urlManagerDeleteUrlRewrite()**](BasicOperationsApi.md#urlManagerDeleteUrlRewrite) | **POST** /urlmanager/delete_url_rewrite | Delete Url Rewrite |
| [**urlManagerDeleteUrlRewrite2()**](BasicOperationsApi.md#urlManagerDeleteUrlRewrite2) | **POST** /urlmanager.UrlManager/DeleteUrlRewrite | Delete Url Rewrite |
| [**urlManagerGetUrlRewrite()**](BasicOperationsApi.md#urlManagerGetUrlRewrite) | **POST** /urlmanager/get_url_rewrite | Get Url Rewrite |
| [**urlManagerGetUrlRewrite2()**](BasicOperationsApi.md#urlManagerGetUrlRewrite2) | **POST** /urlmanager.UrlManager/GetUrlRewrite | Get Url Rewrite |
| [**urlManagerListUrlRewrites()**](BasicOperationsApi.md#urlManagerListUrlRewrites) | **POST** /urlmanager/list_url_rewrites | List Url Rewrites |
| [**urlManagerListUrlRewrites2()**](BasicOperationsApi.md#urlManagerListUrlRewrites2) | **POST** /urlmanager.UrlManager/ListUrlRewrites | List Url Rewrites |
| [**urlManagerListUrlRewritesByTargetPaths()**](BasicOperationsApi.md#urlManagerListUrlRewritesByTargetPaths) | **POST** /urlmanager/list_url_rewrites_by_target_paths | List Url Rewrites By Target Paths |
| [**urlManagerListUrlRewritesByTargetPaths2()**](BasicOperationsApi.md#urlManagerListUrlRewritesByTargetPaths2) | **POST** /urlmanager.UrlManager/ListUrlRewritesByTargetPaths | List Url Rewrites By Target Paths |
| [**urlManagerResolveUrlRewrite()**](BasicOperationsApi.md#urlManagerResolveUrlRewrite) | **POST** /urlmanager/resolve_url_rewrite | Resolve Url Rewrite |
| [**urlManagerResolveUrlRewrite2()**](BasicOperationsApi.md#urlManagerResolveUrlRewrite2) | **POST** /urlmanager.UrlManager/ResolveUrlRewrite | Resolve Url Rewrite |


## `urlManagerChangeUrlRewriteRequestPath()`

```php
urlManagerChangeUrlRewriteRequestPath($body): object
```

Change Url Rewrite Request Path

Modify the request path of a specific URL rewrite configuration.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: Authorization
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new OpenAPI\Client\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\UrlmanagerChangeUrlRewriteRequestPathRequest(); // \OpenAPI\Client\Model\UrlmanagerChangeUrlRewriteRequestPathRequest

try {
    $result = $apiInstance->urlManagerChangeUrlRewriteRequestPath($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BasicOperationsApi->urlManagerChangeUrlRewriteRequestPath: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | [**\OpenAPI\Client\Model\UrlmanagerChangeUrlRewriteRequestPathRequest**](../Model/UrlmanagerChangeUrlRewriteRequestPathRequest.md)|  | |

### Return type

**object**

### Authorization

[Authorization](../../README.md#Authorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerChangeUrlRewriteRequestPath2()`

```php
urlManagerChangeUrlRewriteRequestPath2($body): object
```

Change Url Rewrite Request Path

Modify the request path of a specific URL rewrite configuration.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: Authorization
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new OpenAPI\Client\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\UrlmanagerChangeUrlRewriteRequestPathRequest(); // \OpenAPI\Client\Model\UrlmanagerChangeUrlRewriteRequestPathRequest

try {
    $result = $apiInstance->urlManagerChangeUrlRewriteRequestPath2($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BasicOperationsApi->urlManagerChangeUrlRewriteRequestPath2: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | [**\OpenAPI\Client\Model\UrlmanagerChangeUrlRewriteRequestPathRequest**](../Model/UrlmanagerChangeUrlRewriteRequestPathRequest.md)|  | |

### Return type

**object**

### Authorization

[Authorization](../../README.md#Authorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerCreateUrlRewrite()`

```php
urlManagerCreateUrlRewrite($body): \OpenAPI\Client\Model\UrlmanagerUrlRewrite
```

Create Url Rewrite

Create a new URL rewrite configuration with customizable rules.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: Authorization
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new OpenAPI\Client\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\UrlmanagerCreateUrlRewriteRequest(); // \OpenAPI\Client\Model\UrlmanagerCreateUrlRewriteRequest

try {
    $result = $apiInstance->urlManagerCreateUrlRewrite($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BasicOperationsApi->urlManagerCreateUrlRewrite: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | [**\OpenAPI\Client\Model\UrlmanagerCreateUrlRewriteRequest**](../Model/UrlmanagerCreateUrlRewriteRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\UrlmanagerUrlRewrite**](../Model/UrlmanagerUrlRewrite.md)

### Authorization

[Authorization](../../README.md#Authorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerCreateUrlRewrite2()`

```php
urlManagerCreateUrlRewrite2($body): \OpenAPI\Client\Model\UrlmanagerUrlRewrite
```

Create Url Rewrite

Create a new URL rewrite configuration with customizable rules.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: Authorization
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new OpenAPI\Client\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\UrlmanagerCreateUrlRewriteRequest(); // \OpenAPI\Client\Model\UrlmanagerCreateUrlRewriteRequest

try {
    $result = $apiInstance->urlManagerCreateUrlRewrite2($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BasicOperationsApi->urlManagerCreateUrlRewrite2: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | [**\OpenAPI\Client\Model\UrlmanagerCreateUrlRewriteRequest**](../Model/UrlmanagerCreateUrlRewriteRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\UrlmanagerUrlRewrite**](../Model/UrlmanagerUrlRewrite.md)

### Authorization

[Authorization](../../README.md#Authorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerDeleteUrlRewrite()`

```php
urlManagerDeleteUrlRewrite($body): object
```

Delete Url Rewrite

Delete an existing URL rewrite configuration.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: Authorization
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new OpenAPI\Client\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\UrlmanagerDeleteUrlRewriteRequest(); // \OpenAPI\Client\Model\UrlmanagerDeleteUrlRewriteRequest

try {
    $result = $apiInstance->urlManagerDeleteUrlRewrite($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BasicOperationsApi->urlManagerDeleteUrlRewrite: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | [**\OpenAPI\Client\Model\UrlmanagerDeleteUrlRewriteRequest**](../Model/UrlmanagerDeleteUrlRewriteRequest.md)|  | |

### Return type

**object**

### Authorization

[Authorization](../../README.md#Authorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerDeleteUrlRewrite2()`

```php
urlManagerDeleteUrlRewrite2($body): object
```

Delete Url Rewrite

Delete an existing URL rewrite configuration.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: Authorization
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new OpenAPI\Client\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\UrlmanagerDeleteUrlRewriteRequest(); // \OpenAPI\Client\Model\UrlmanagerDeleteUrlRewriteRequest

try {
    $result = $apiInstance->urlManagerDeleteUrlRewrite2($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BasicOperationsApi->urlManagerDeleteUrlRewrite2: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | [**\OpenAPI\Client\Model\UrlmanagerDeleteUrlRewriteRequest**](../Model/UrlmanagerDeleteUrlRewriteRequest.md)|  | |

### Return type

**object**

### Authorization

[Authorization](../../README.md#Authorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerGetUrlRewrite()`

```php
urlManagerGetUrlRewrite($body): \OpenAPI\Client\Model\UrlmanagerUrlRewrite
```

Get Url Rewrite

Retrieve the details of a specific URL rewrite configuration.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: Authorization
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new OpenAPI\Client\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\UrlmanagerGetUrlRewriteRequest(); // \OpenAPI\Client\Model\UrlmanagerGetUrlRewriteRequest

try {
    $result = $apiInstance->urlManagerGetUrlRewrite($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BasicOperationsApi->urlManagerGetUrlRewrite: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | [**\OpenAPI\Client\Model\UrlmanagerGetUrlRewriteRequest**](../Model/UrlmanagerGetUrlRewriteRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\UrlmanagerUrlRewrite**](../Model/UrlmanagerUrlRewrite.md)

### Authorization

[Authorization](../../README.md#Authorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerGetUrlRewrite2()`

```php
urlManagerGetUrlRewrite2($body): \OpenAPI\Client\Model\UrlmanagerUrlRewrite
```

Get Url Rewrite

Retrieve the details of a specific URL rewrite configuration.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: Authorization
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new OpenAPI\Client\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\UrlmanagerGetUrlRewriteRequest(); // \OpenAPI\Client\Model\UrlmanagerGetUrlRewriteRequest

try {
    $result = $apiInstance->urlManagerGetUrlRewrite2($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BasicOperationsApi->urlManagerGetUrlRewrite2: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | [**\OpenAPI\Client\Model\UrlmanagerGetUrlRewriteRequest**](../Model/UrlmanagerGetUrlRewriteRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\UrlmanagerUrlRewrite**](../Model/UrlmanagerUrlRewrite.md)

### Authorization

[Authorization](../../README.md#Authorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerListUrlRewrites()`

```php
urlManagerListUrlRewrites($body): \OpenAPI\Client\Model\UrlmanagerListUrlRewritesResponse
```

List Url Rewrites

Retrieve a list of all URL rewrite configurations in your application.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: Authorization
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new OpenAPI\Client\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\UrlmanagerListUrlRewritesRequest(); // \OpenAPI\Client\Model\UrlmanagerListUrlRewritesRequest

try {
    $result = $apiInstance->urlManagerListUrlRewrites($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BasicOperationsApi->urlManagerListUrlRewrites: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | [**\OpenAPI\Client\Model\UrlmanagerListUrlRewritesRequest**](../Model/UrlmanagerListUrlRewritesRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\UrlmanagerListUrlRewritesResponse**](../Model/UrlmanagerListUrlRewritesResponse.md)

### Authorization

[Authorization](../../README.md#Authorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerListUrlRewrites2()`

```php
urlManagerListUrlRewrites2($body): \OpenAPI\Client\Model\UrlmanagerListUrlRewritesResponse
```

List Url Rewrites

Retrieve a list of all URL rewrite configurations in your application.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: Authorization
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new OpenAPI\Client\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\UrlmanagerListUrlRewritesRequest(); // \OpenAPI\Client\Model\UrlmanagerListUrlRewritesRequest

try {
    $result = $apiInstance->urlManagerListUrlRewrites2($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BasicOperationsApi->urlManagerListUrlRewrites2: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | [**\OpenAPI\Client\Model\UrlmanagerListUrlRewritesRequest**](../Model/UrlmanagerListUrlRewritesRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\UrlmanagerListUrlRewritesResponse**](../Model/UrlmanagerListUrlRewritesResponse.md)

### Authorization

[Authorization](../../README.md#Authorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerListUrlRewritesByTargetPaths()`

```php
urlManagerListUrlRewritesByTargetPaths($body): \OpenAPI\Client\Model\UrlmanagerListUrlRewritesByTargetPathsRequest
```

List Url Rewrites By Target Paths

Retrieve URL rewrite configurations based on target paths.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: Authorization
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new OpenAPI\Client\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\UrlmanagerListUrlRewritesByTargetPathsRequest(); // \OpenAPI\Client\Model\UrlmanagerListUrlRewritesByTargetPathsRequest

try {
    $result = $apiInstance->urlManagerListUrlRewritesByTargetPaths($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BasicOperationsApi->urlManagerListUrlRewritesByTargetPaths: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | [**\OpenAPI\Client\Model\UrlmanagerListUrlRewritesByTargetPathsRequest**](../Model/UrlmanagerListUrlRewritesByTargetPathsRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\UrlmanagerListUrlRewritesByTargetPathsRequest**](../Model/UrlmanagerListUrlRewritesByTargetPathsRequest.md)

### Authorization

[Authorization](../../README.md#Authorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerListUrlRewritesByTargetPaths2()`

```php
urlManagerListUrlRewritesByTargetPaths2($body): \OpenAPI\Client\Model\UrlmanagerListUrlRewritesByTargetPathsRequest
```

List Url Rewrites By Target Paths

Retrieve URL rewrite configurations based on target paths.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: Authorization
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new OpenAPI\Client\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\UrlmanagerListUrlRewritesByTargetPathsRequest(); // \OpenAPI\Client\Model\UrlmanagerListUrlRewritesByTargetPathsRequest

try {
    $result = $apiInstance->urlManagerListUrlRewritesByTargetPaths2($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BasicOperationsApi->urlManagerListUrlRewritesByTargetPaths2: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | [**\OpenAPI\Client\Model\UrlmanagerListUrlRewritesByTargetPathsRequest**](../Model/UrlmanagerListUrlRewritesByTargetPathsRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\UrlmanagerListUrlRewritesByTargetPathsRequest**](../Model/UrlmanagerListUrlRewritesByTargetPathsRequest.md)

### Authorization

[Authorization](../../README.md#Authorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerResolveUrlRewrite()`

```php
urlManagerResolveUrlRewrite($body): \OpenAPI\Client\Model\UrlmanagerUrlRewrite
```

Resolve Url Rewrite

Resolve and retrieve the rewritten URL for a given input URL.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: Authorization
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new OpenAPI\Client\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\UrlmanagerResolveUrlRewriteRequest(); // \OpenAPI\Client\Model\UrlmanagerResolveUrlRewriteRequest

try {
    $result = $apiInstance->urlManagerResolveUrlRewrite($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BasicOperationsApi->urlManagerResolveUrlRewrite: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | [**\OpenAPI\Client\Model\UrlmanagerResolveUrlRewriteRequest**](../Model/UrlmanagerResolveUrlRewriteRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\UrlmanagerUrlRewrite**](../Model/UrlmanagerUrlRewrite.md)

### Authorization

[Authorization](../../README.md#Authorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerResolveUrlRewrite2()`

```php
urlManagerResolveUrlRewrite2($body): \OpenAPI\Client\Model\UrlmanagerUrlRewrite
```

Resolve Url Rewrite

Resolve and retrieve the rewritten URL for a given input URL.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: Authorization
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new OpenAPI\Client\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\UrlmanagerResolveUrlRewriteRequest(); // \OpenAPI\Client\Model\UrlmanagerResolveUrlRewriteRequest

try {
    $result = $apiInstance->urlManagerResolveUrlRewrite2($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BasicOperationsApi->urlManagerResolveUrlRewrite2: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | [**\OpenAPI\Client\Model\UrlmanagerResolveUrlRewriteRequest**](../Model/UrlmanagerResolveUrlRewriteRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\UrlmanagerUrlRewrite**](../Model/UrlmanagerUrlRewrite.md)

### Authorization

[Authorization](../../README.md#Authorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
