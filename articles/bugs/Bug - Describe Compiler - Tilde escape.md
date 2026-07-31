Article type: 						`Bug`<br>
Article name:						`Bug - Describe Compiler - Tilde escape`<br>
Affected Software/module:			`Describe Compiler`<br>
Author:								`Framez`<br>
<br>

## Description:
Escaping left angle bracket produces a right angle bracket in the final text
<br><br>
```
      adb shell pm uninstall --user 0 \<PACKAGE_NAME\> {color|blue}, 
      uninstall a package {comment},
      gap {empty},
```

This produces a text "adb shell pm uninstall --user 0 >PACKAGE_NAME>"