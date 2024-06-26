# cloudirector's Proxy
> A web proxy for my own light personal use; also forked.

> ## Running in the cloud
>> [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/cloudirector/cloudirectors-proxy/tree/master)

> ## Running locally
>> ```sh
>> git clone https://github.com/cloudirector/cloudirectors-proxy.git
>> cd cloudirectors-proxy
>> node server.js
>> ```


> ## Options in config.json
>> ```json
>> {
>>     "port": "8080",
>>     "ssl": false,
>>     "prefix": "/web/",
>>     "localAddresses": [],
>>     "blockedHostnames": []
>> }
>> ```
>>> 
>>> `"port": "8080"` = Sets HTTP server port of web proxy.
>>> 
>>> `"ssl": "false"` = Sets HTTP server SSL.
>>> 
>>> `"prefix": "/web/"` = Sets the overall prefix of the web proxy.
>>> 
>>> `"localAddresses": [ "0.0.0.0" ]` = Allows you to choose which IP to make the request from. If there are multiple IP's then the IP chosen will be randomized.
>>> 
>>> `"blockedHostnames": [ "example.org", "example.com" ]` = If the hostname of the proxy URL matches any of the URL hostnames listed in the array, the request to the server will be cancelled.
