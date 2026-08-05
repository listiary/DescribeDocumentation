Article type: 						`Feature Suggestion`<br>
Article name:						`SuggestFeature - SparkLib - Internet Access Check on some exceptions`<br>
Affected Software/module:			`SparkLib`, `SparkCli`<br>
Author:								`Framez`<br>
<br>

## Description:
I didn't have internet, because my laptop was in airplane mode, and the script I was running failed,
saying that:

```
Values are NOT correct - we were not able to establish a connection to the server with the values you provided!
Connection failed: php_network_getaddresses: getaddrinfo for web.jumphosting03.com failed: No such host is known
SCRIPT FAILED
```

Which is kind of fine, yet, it will be better, if we can, in such occasions, look at if we can provide a more specific error to the user.


## Relevant commands:
```
php spark.php config-test
```