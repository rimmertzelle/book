# Working example

This project is also available on [github](https://github.com/rimmertzelle/ajax-proxy).

On the server, for example in PHP, create an API call to a different domain. In this following code [cUrl](https://www.php.net/manual/en/book.curl.php) is used to setup and execute the call.

```php
<?php
/**
 * Class to handle an AJAX call as a proxy
 */
class Proxy
{
    private $url;

    public function __construct($url)
    {
        $this->url = $url;
    }

    public function getData($collection)
    {
        $request_url = $this->url . "/" . $collection . "/";
        $curl = curl_init($request_url);

        curl_setopt($curl, CURLOPT_RETURNTRANSFER, true);
        curl_setopt($curl, CURLOPT_HTTPHEADER, [
            'Content-Type: application/json',
        ]);
        
        //API call with Authorization
        //Change the key with your credentials
        // curl_setopt($curl, CURLOPT_HTTPHEADER, [
        //     'Content-Type: application/json',
        //     'Authorization: Bearer key'
        // ]);

        $response = curl_exec($curl);
        curl_close($curl);

        return $response;
    }
}
```

A controller to handle the call from the browser and setup the proxy.

```php
<?php
include("./proxy.php");

//setup the Proxy with the right credentials
$mySwapiProxy = new Proxy('https://swapi.dev/api');

//get the data
$result = $mySwapiProxy->getData('people/1');

//print the data to the frontend.
echo $result;
```

The call from the browser to the proxy.

```jsx
window.addEventListener("load", init);

function init() {
  displayData();
}

function displayData(){
  fetch("../controller.php").then(function(response){
    return response.json();
  }).then(function(data){
    console.log(data);
  }).catch(function(error){
    console.log(error);
  })
}
```