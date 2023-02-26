
# API documentation
Short links can be generated in a programmable way by calling the API interface

### API ccll address

Self-deployed CloudFlare Worker address, for example: https://url.dem0.workers.dev or a self-bound domain name

### Calling method: HTTP POST Request format: JSON
Example:
````
{
	"url": "https://example.com"
}
````

### Example response (JSON):

````
{
    "status": 200,
    "key": "/demo"
}
````

Note: The interface will only return the key value corresponding to the short link. In actual use, the corresponding domain name prefix needs to be added. For example, if the key parameter returned in the example is "/demo", we need to add "https://url.dem0.workers.dev" as a prefix, it can be used by completing it as a complete url, namely: https://url.dem0.workers.dev/demo

