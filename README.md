# Http class CURL wrapper
CURL Wrapper

VERSION = 0.0.1

## Requirement
PHP >= 5.2

For return response body as XML need SimpleXMLElement

## Usage
### Include required files in the application

Include `Http` class to .php file

```php
require_once('Http.php');
```

### How to use
Initialize new Class, and use methods like

```php
$http = Http::get($url);
$http->json();
```

`$http->url` - current URL

`$http->method` - current method

`$http->request` - requested data

`$http->response` - server response

`$http->info` - connection information

`$http->json()`- return response body as json

 `$http->xml()`- return response body as xml

## Methods

```php
$http = Http::get($url);
```

```php
$http = Http::post($url, $data);
```

`$data` - request data

```php
$http = Http::put($url, $data);
```

```php
$http = Http::patch($url, $data);
```

```php
$http = Http::delete($url, $data);
```

## Contributing
1. Fork it ( https://github.com/stepanovit/http_curl_wrapper/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request