Article type: 						`Feature Suggestion`<br>
Article name:						`SuggestFeature - Log function parameter`<br>
Affected Software/module:			`SparkLib`, `SparkCli`<br>
Author:								`Framez`<br>
<br>

## Description:
In SparkLib, most functions log to a variable, which is returned afterwards in the output associative array.
However, this is rigid - allowing the log to be outputted only after the execution has finished.
A better, more interactive way is to pass a logger function to each function, and pass it to an internal logging function,
so that the consumer of SparkCli can pass something like for example - a console logging function, and receive the output immediately.
<br><br>
This is done in few functions in the library, but I am suggesting that this should be the norm in the next release or SparkLib

```
public static function Database_Curate_Ids(mysqli $link, ?callable $logger = null)
```