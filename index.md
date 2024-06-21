# Chinese Takeout Name API

> **NOTE:** This API needs to be in a CORS Proxy to work due to autoenabled cors restrictions on the web page from vercel.

Recommended Endpoint:`https://calculator-eight-weld.vercel.app/?url=https://chineserandomtakeoutapi-v1.vercel.app/api/generate`

Normal(CORS Restricted): `https://chineserandomtakeoutapi-v1.vercel.app/api/generate`

The Chinese takeout name API is an API that generates a random chinese takeout restaurant name:

```json
{
  "restaurantName": "Great Wall Oriental Seafood"
}
```
This project was initiated using Node.js v18.19.0, Express.js and Vercel CLI.

The API is completely free to use with no API Key, no X-API Key, no call limits and no need to log into any external service.
 
Below are different methods you can run it Including our public Postman Workspace.

[![Run in Postman](https://run.pstmn.io/button.svg)](https://www.postman.com/spacecraft-engineer-38000999/workspace/takeout-api)


Shell (cURL):
```shell 
curl --location https://calculator-eight-weld.vercel.app/?url=https%3A%2F%2Fchineserandomtakeoutapi-v1.vercel.app%2Fapi%2Fgenerate
```
CS (HttpClient):
```cs
var client = new HttpClient();
var request = new HttpRequestMessage(HttpMethod.Get, "https://calculator-eight-weld.vercel.app/?url=https://chineserandomtakeoutapi-v1.vercel.app/api/generate");
var response = await client.SendAsync(request);
response.EnsureSuccessStatusCode();
Console.WriteLine(await response.Content.ReadAsStringAsync());
```
JS (jquery):
```javascript

var settings = {
  "url": "https://calculator-eight-weld.vercel.app/?url=https://chineserandomtakeoutapi-v1.vercel.app/api/generate",
  "method": "GET",
  "timeout": 0,
};

$.ajax(settings).done(function (response) {
  console.log(response);
});
```
Node.js (Axios):
```javascript
const axios = require('axios');

let config = {
  method: 'get',
  maxBodyLength: Infinity,
  url: 'https://calculator-eight-weld.vercel.app/?url=https://chineserandomtakeoutapi-v1.vercel.app/api/generate',
  headers: { }
};

axios.request(config)
.then((response) => {
  console.log(JSON.stringify(response.data));
})
.catch((error) => {
  console.log(error);
});
```
PHP (cURL):
```php
<?php

$curl = curl_init();

curl_setopt_array($curl, array(
  CURLOPT_URL => 'https://calculator-eight-weld.vercel.app/?url=https%3A%2F%2Fchineserandomtakeoutapi-v1.vercel.app%2Fapi%2Fgenerate',
  CURLOPT_RETURNTRANSFER => true,
  CURLOPT_ENCODING => '',
  CURLOPT_MAXREDIRS => 10,
  CURLOPT_TIMEOUT => 0,
  CURLOPT_FOLLOWLOCATION => true,
  CURLOPT_HTTP_VERSION => CURL_HTTP_VERSION_1_1,
  CURLOPT_CUSTOMREQUEST => 'GET',
));
```
C (libcurl):
```c
CURL *curl;
CURLcode res;
curl = curl_easy_init();
if(curl) {
  curl_easy_setopt(curl, CURLOPT_CUSTOMREQUEST, "GET");
  curl_easy_setopt(curl, CURLOPT_URL, "https://calculator-eight-weld.vercel.app/?url=https%3A%2F%2Fchineserandomtakeoutapi-v1.vercel.app%2Fapi%2Fgenerate");
  curl_easy_setopt(curl, CURLOPT_FOLLOWLOCATION, 1L);
  curl_easy_setopt(curl, CURLOPT_DEFAULT_PROTOCOL, "https");
  struct curl_slist *headers = NULL;
  curl_easy_setopt(curl, CURLOPT_HTTPHEADER, headers);
  res = curl_easy_perform(curl);
}
curl_easy_cleanup(curl);
```
Python (http.client):
```python
import http.client

conn = http.client.HTTPSConnection("calculator-eight-weld.vercel.app")
payload = ''
headers = {}
conn.request("GET", "/?url=https://chineserandomtakeoutapi-v1.vercel.app/api/generate", payload, headers)
res = conn.getresponse()
data = res.read()
print(data.decode("utf-8"))
```
R:
```r
library(RCurl)
res <- getURL("https://calculator-eight-weld.vercel.app/?url=https://chineserandomtakeoutapi-v1.vercel.app/api/generate", .opts=list(followlocation = TRUE))
cat(res)
```
