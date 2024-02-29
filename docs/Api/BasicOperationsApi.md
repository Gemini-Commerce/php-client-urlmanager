# GeminiCommerce\Urlmanager\BasicOperationsApi

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



$apiInstance = new GeminiCommerce\Urlmanager\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \GeminiCommerce\Urlmanager\Model\UrlmanagerChangeUrlRewriteRequestPathRequest(); // \GeminiCommerce\Urlmanager\Model\UrlmanagerChangeUrlRewriteRequestPathRequest

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
| **body** | [**\GeminiCommerce\Urlmanager\Model\UrlmanagerChangeUrlRewriteRequestPathRequest**](../Model/UrlmanagerChangeUrlRewriteRequestPathRequest.md)|  | |

### Return type

**object**

### Authorization

No authorization required

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



$apiInstance = new GeminiCommerce\Urlmanager\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \GeminiCommerce\Urlmanager\Model\UrlmanagerChangeUrlRewriteRequestPathRequest(); // \GeminiCommerce\Urlmanager\Model\UrlmanagerChangeUrlRewriteRequestPathRequest

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
| **body** | [**\GeminiCommerce\Urlmanager\Model\UrlmanagerChangeUrlRewriteRequestPathRequest**](../Model/UrlmanagerChangeUrlRewriteRequestPathRequest.md)|  | |

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerCreateUrlRewrite()`

```php
urlManagerCreateUrlRewrite($body): \GeminiCommerce\Urlmanager\Model\UrlmanagerUrlRewrite
```

Create Url Rewrite

Create a new URL rewrite configuration with customizable rules.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new GeminiCommerce\Urlmanager\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \GeminiCommerce\Urlmanager\Model\UrlmanagerCreateUrlRewriteRequest(); // \GeminiCommerce\Urlmanager\Model\UrlmanagerCreateUrlRewriteRequest

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
| **body** | [**\GeminiCommerce\Urlmanager\Model\UrlmanagerCreateUrlRewriteRequest**](../Model/UrlmanagerCreateUrlRewriteRequest.md)|  | |

### Return type

[**\GeminiCommerce\Urlmanager\Model\UrlmanagerUrlRewrite**](../Model/UrlmanagerUrlRewrite.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerCreateUrlRewrite2()`

```php
urlManagerCreateUrlRewrite2($body): \GeminiCommerce\Urlmanager\Model\UrlmanagerUrlRewrite
```

Create Url Rewrite

Create a new URL rewrite configuration with customizable rules.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new GeminiCommerce\Urlmanager\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \GeminiCommerce\Urlmanager\Model\UrlmanagerCreateUrlRewriteRequest(); // \GeminiCommerce\Urlmanager\Model\UrlmanagerCreateUrlRewriteRequest

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
| **body** | [**\GeminiCommerce\Urlmanager\Model\UrlmanagerCreateUrlRewriteRequest**](../Model/UrlmanagerCreateUrlRewriteRequest.md)|  | |

### Return type

[**\GeminiCommerce\Urlmanager\Model\UrlmanagerUrlRewrite**](../Model/UrlmanagerUrlRewrite.md)

### Authorization

No authorization required

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



$apiInstance = new GeminiCommerce\Urlmanager\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \GeminiCommerce\Urlmanager\Model\UrlmanagerDeleteUrlRewriteRequest(); // \GeminiCommerce\Urlmanager\Model\UrlmanagerDeleteUrlRewriteRequest

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
| **body** | [**\GeminiCommerce\Urlmanager\Model\UrlmanagerDeleteUrlRewriteRequest**](../Model/UrlmanagerDeleteUrlRewriteRequest.md)|  | |

### Return type

**object**

### Authorization

No authorization required

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



$apiInstance = new GeminiCommerce\Urlmanager\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \GeminiCommerce\Urlmanager\Model\UrlmanagerDeleteUrlRewriteRequest(); // \GeminiCommerce\Urlmanager\Model\UrlmanagerDeleteUrlRewriteRequest

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
| **body** | [**\GeminiCommerce\Urlmanager\Model\UrlmanagerDeleteUrlRewriteRequest**](../Model/UrlmanagerDeleteUrlRewriteRequest.md)|  | |

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerGetUrlRewrite()`

```php
urlManagerGetUrlRewrite($body): \GeminiCommerce\Urlmanager\Model\UrlmanagerUrlRewrite
```

Get Url Rewrite

Retrieve the details of a specific URL rewrite configuration.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new GeminiCommerce\Urlmanager\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \GeminiCommerce\Urlmanager\Model\UrlmanagerGetUrlRewriteRequest(); // \GeminiCommerce\Urlmanager\Model\UrlmanagerGetUrlRewriteRequest

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
| **body** | [**\GeminiCommerce\Urlmanager\Model\UrlmanagerGetUrlRewriteRequest**](../Model/UrlmanagerGetUrlRewriteRequest.md)|  | |

### Return type

[**\GeminiCommerce\Urlmanager\Model\UrlmanagerUrlRewrite**](../Model/UrlmanagerUrlRewrite.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerGetUrlRewrite2()`

```php
urlManagerGetUrlRewrite2($body): \GeminiCommerce\Urlmanager\Model\UrlmanagerUrlRewrite
```

Get Url Rewrite

Retrieve the details of a specific URL rewrite configuration.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new GeminiCommerce\Urlmanager\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \GeminiCommerce\Urlmanager\Model\UrlmanagerGetUrlRewriteRequest(); // \GeminiCommerce\Urlmanager\Model\UrlmanagerGetUrlRewriteRequest

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
| **body** | [**\GeminiCommerce\Urlmanager\Model\UrlmanagerGetUrlRewriteRequest**](../Model/UrlmanagerGetUrlRewriteRequest.md)|  | |

### Return type

[**\GeminiCommerce\Urlmanager\Model\UrlmanagerUrlRewrite**](../Model/UrlmanagerUrlRewrite.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerListUrlRewrites()`

```php
urlManagerListUrlRewrites($body): \GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesResponse
```

List Url Rewrites

Retrieve a list of all URL rewrite configurations in your application.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new GeminiCommerce\Urlmanager\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesRequest(); // \GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesRequest

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
| **body** | [**\GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesRequest**](../Model/UrlmanagerListUrlRewritesRequest.md)|  | |

### Return type

[**\GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesResponse**](../Model/UrlmanagerListUrlRewritesResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerListUrlRewrites2()`

```php
urlManagerListUrlRewrites2($body): \GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesResponse
```

List Url Rewrites

Retrieve a list of all URL rewrite configurations in your application.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new GeminiCommerce\Urlmanager\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesRequest(); // \GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesRequest

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
| **body** | [**\GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesRequest**](../Model/UrlmanagerListUrlRewritesRequest.md)|  | |

### Return type

[**\GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesResponse**](../Model/UrlmanagerListUrlRewritesResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerListUrlRewritesByTargetPaths()`

```php
urlManagerListUrlRewritesByTargetPaths($body): \GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesByTargetPathsRequest
```

List Url Rewrites By Target Paths

Retrieve URL rewrite configurations based on target paths.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new GeminiCommerce\Urlmanager\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesByTargetPathsRequest(); // \GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesByTargetPathsRequest

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
| **body** | [**\GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesByTargetPathsRequest**](../Model/UrlmanagerListUrlRewritesByTargetPathsRequest.md)|  | |

### Return type

[**\GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesByTargetPathsRequest**](../Model/UrlmanagerListUrlRewritesByTargetPathsRequest.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerListUrlRewritesByTargetPaths2()`

```php
urlManagerListUrlRewritesByTargetPaths2($body): \GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesByTargetPathsRequest
```

List Url Rewrites By Target Paths

Retrieve URL rewrite configurations based on target paths.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new GeminiCommerce\Urlmanager\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesByTargetPathsRequest(); // \GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesByTargetPathsRequest

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
| **body** | [**\GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesByTargetPathsRequest**](../Model/UrlmanagerListUrlRewritesByTargetPathsRequest.md)|  | |

### Return type

[**\GeminiCommerce\Urlmanager\Model\UrlmanagerListUrlRewritesByTargetPathsRequest**](../Model/UrlmanagerListUrlRewritesByTargetPathsRequest.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerResolveUrlRewrite()`

```php
urlManagerResolveUrlRewrite($body): \GeminiCommerce\Urlmanager\Model\UrlmanagerUrlRewrite
```

Resolve Url Rewrite

Resolve and retrieve the rewritten URL for a given input URL.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new GeminiCommerce\Urlmanager\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \GeminiCommerce\Urlmanager\Model\UrlmanagerResolveUrlRewriteRequest(); // \GeminiCommerce\Urlmanager\Model\UrlmanagerResolveUrlRewriteRequest

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
| **body** | [**\GeminiCommerce\Urlmanager\Model\UrlmanagerResolveUrlRewriteRequest**](../Model/UrlmanagerResolveUrlRewriteRequest.md)|  | |

### Return type

[**\GeminiCommerce\Urlmanager\Model\UrlmanagerUrlRewrite**](../Model/UrlmanagerUrlRewrite.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `urlManagerResolveUrlRewrite2()`

```php
urlManagerResolveUrlRewrite2($body): \GeminiCommerce\Urlmanager\Model\UrlmanagerUrlRewrite
```

Resolve Url Rewrite

Resolve and retrieve the rewritten URL for a given input URL.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new GeminiCommerce\Urlmanager\Api\BasicOperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \GeminiCommerce\Urlmanager\Model\UrlmanagerResolveUrlRewriteRequest(); // \GeminiCommerce\Urlmanager\Model\UrlmanagerResolveUrlRewriteRequest

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
| **body** | [**\GeminiCommerce\Urlmanager\Model\UrlmanagerResolveUrlRewriteRequest**](../Model/UrlmanagerResolveUrlRewriteRequest.md)|  | |

### Return type

[**\GeminiCommerce\Urlmanager\Model\UrlmanagerUrlRewrite**](../Model/UrlmanagerUrlRewrite.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
