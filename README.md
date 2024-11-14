# urlmanager

The URL Manager service provides a set of APIs for managing URL rewrites within your application. URL rewriting is a technique used to modify the appearance or structure of URLs while maintaining the functionality and accessibility of the underlying resources.

The URL Manager service offers various operations to create, retrieve, update, and delete URL rewrite configurations. These configurations allow you to define rules that map incoming URLs to different paths or destinations based on specific criteria. By using URL rewriting, you can enhance the user experience, improve SEO (Search Engine Optimization), and manage complex URL structures effectively.

To get started with the URL Manager service, you need to integrate the provided Proto API into your application. The API supports various programming languages and frameworks, making it easy to incorporate URL rewriting functionality into your existing codebase.

Once integrated, you can utilize the different API methods to create, manage, and query URL rewrite configurations based on your application's requirements.

Refer to the API documentation for detailed information on the request and response formats, authentication requirements, and example usage of each API method.


## Installation & Usage

### Requirements

PHP 7.4 and later.
Should also work with PHP 8.0.

### Composer

To install the bindings via [Composer](https://getcomposer.org/), add the following to `composer.json`:

```json
{
  "repositories": [
    {
      "type": "vcs",
      "url": "https://github.com/Gemini-Commerce/php-client-urlmanager.git"
    }
  ],
  "require": {
    "Gemini-Commerce/php-client-urlmanager": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
<?php
require_once('/path/to/urlmanager/vendor/autoload.php');
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

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

## API Endpoints

All URIs are relative to *https://urlmanager.api.gogemini.io*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*BasicOperationsApi* | [**urlManagerChangeUrlRewriteRequestPath**](docs/Api/BasicOperationsApi.md#urlmanagerchangeurlrewriterequestpath) | **POST** /urlmanager/change_url_rewrite_request_path | Change Url Rewrite Request Path
*BasicOperationsApi* | [**urlManagerChangeUrlRewriteRequestPath2**](docs/Api/BasicOperationsApi.md#urlmanagerchangeurlrewriterequestpath2) | **POST** /urlmanager.UrlManager/ChangeUrlRewriteRequestPath | Change Url Rewrite Request Path
*BasicOperationsApi* | [**urlManagerCreateUrlRewrite**](docs/Api/BasicOperationsApi.md#urlmanagercreateurlrewrite) | **POST** /urlmanager/create_url_rewrite | Create Url Rewrite
*BasicOperationsApi* | [**urlManagerCreateUrlRewrite2**](docs/Api/BasicOperationsApi.md#urlmanagercreateurlrewrite2) | **POST** /urlmanager.UrlManager/CreateUrlRewrite | Create Url Rewrite
*BasicOperationsApi* | [**urlManagerDeleteUrlRewrite**](docs/Api/BasicOperationsApi.md#urlmanagerdeleteurlrewrite) | **POST** /urlmanager/delete_url_rewrite | Delete Url Rewrite
*BasicOperationsApi* | [**urlManagerDeleteUrlRewrite2**](docs/Api/BasicOperationsApi.md#urlmanagerdeleteurlrewrite2) | **POST** /urlmanager.UrlManager/DeleteUrlRewrite | Delete Url Rewrite
*BasicOperationsApi* | [**urlManagerGetUrlRewrite**](docs/Api/BasicOperationsApi.md#urlmanagergeturlrewrite) | **POST** /urlmanager/get_url_rewrite | Get Url Rewrite
*BasicOperationsApi* | [**urlManagerGetUrlRewrite2**](docs/Api/BasicOperationsApi.md#urlmanagergeturlrewrite2) | **POST** /urlmanager.UrlManager/GetUrlRewrite | Get Url Rewrite
*BasicOperationsApi* | [**urlManagerListUrlRewrites**](docs/Api/BasicOperationsApi.md#urlmanagerlisturlrewrites) | **POST** /urlmanager/list_url_rewrites | List Url Rewrites
*BasicOperationsApi* | [**urlManagerListUrlRewrites2**](docs/Api/BasicOperationsApi.md#urlmanagerlisturlrewrites2) | **POST** /urlmanager.UrlManager/ListUrlRewrites | List Url Rewrites
*BasicOperationsApi* | [**urlManagerListUrlRewritesByTargetPaths**](docs/Api/BasicOperationsApi.md#urlmanagerlisturlrewritesbytargetpaths) | **POST** /urlmanager/list_url_rewrites_by_target_paths | List Url Rewrites By Target Paths
*BasicOperationsApi* | [**urlManagerListUrlRewritesByTargetPaths2**](docs/Api/BasicOperationsApi.md#urlmanagerlisturlrewritesbytargetpaths2) | **POST** /urlmanager.UrlManager/ListUrlRewritesByTargetPaths | List Url Rewrites By Target Paths
*BasicOperationsApi* | [**urlManagerResolveUrlRewrite**](docs/Api/BasicOperationsApi.md#urlmanagerresolveurlrewrite) | **POST** /urlmanager/resolve_url_rewrite | Resolve Url Rewrite
*BasicOperationsApi* | [**urlManagerResolveUrlRewrite2**](docs/Api/BasicOperationsApi.md#urlmanagerresolveurlrewrite2) | **POST** /urlmanager.UrlManager/ResolveUrlRewrite | Resolve Url Rewrite

## Models

- [GetUrlRewriteRequestCompoundIdentifier](docs/Model/GetUrlRewriteRequestCompoundIdentifier.md)
- [ListUrlRewritesRequestFilter](docs/Model/ListUrlRewritesRequestFilter.md)
- [ProtobufAny](docs/Model/ProtobufAny.md)
- [RpcStatus](docs/Model/RpcStatus.md)
- [UrlRewriteLinkRel](docs/Model/UrlRewriteLinkRel.md)
- [UrlRewriteRedirectType](docs/Model/UrlRewriteRedirectType.md)
- [UrlmanagerChangeUrlRewriteRequestPathRequest](docs/Model/UrlmanagerChangeUrlRewriteRequestPathRequest.md)
- [UrlmanagerCreateUrlRewriteRequest](docs/Model/UrlmanagerCreateUrlRewriteRequest.md)
- [UrlmanagerDeleteUrlRewriteRequest](docs/Model/UrlmanagerDeleteUrlRewriteRequest.md)
- [UrlmanagerGetUrlRewriteRequest](docs/Model/UrlmanagerGetUrlRewriteRequest.md)
- [UrlmanagerListUrlRewritesByTargetPathsRequest](docs/Model/UrlmanagerListUrlRewritesByTargetPathsRequest.md)
- [UrlmanagerListUrlRewritesByTargetPathsResponse](docs/Model/UrlmanagerListUrlRewritesByTargetPathsResponse.md)
- [UrlmanagerListUrlRewritesRequest](docs/Model/UrlmanagerListUrlRewritesRequest.md)
- [UrlmanagerListUrlRewritesResponse](docs/Model/UrlmanagerListUrlRewritesResponse.md)
- [UrlmanagerResolveUrlRewriteRequest](docs/Model/UrlmanagerResolveUrlRewriteRequest.md)
- [UrlmanagerUrlRewrite](docs/Model/UrlmanagerUrlRewrite.md)

## Authorization

Authentication schemes defined for the API:
### Authorization

- **Type**: API key
- **API key parameter name**: Authorization
- **Location**: HTTP header


### standardAuthorization

- **Type**: `OAuth`
- **Flow**: `implicit`
- **Authorization URL**: ``
- **Scopes**: N/A

## Tests

To run the tests, use:

```bash
composer install
vendor/bin/phpunit
```

## Author

info@gemini-commerce.com

## About this package

This PHP package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: `1.0.0`
    - Generator version: `7.9.0`
- Build package: `org.openapitools.codegen.languages.PhpClientCodegen`
