# jquery-upload-1.0.2-jquery-3-4-1
## jQuery Upload 1.0.2 plugin updated to jQuery 3.4.1

After update the jQuery library on a project from 1.x to 3.4.1 version I got the "e.indexOf is not a function" error message. Trying to find an updated version of "jquery-upload-1.0.2" I haven't found... 
So, let's check what is broken and share a new updated version to the community.


Original File: **jquery.upload-1.0.2.js**

Updated File: **jquery.upload-1.0.2-jquery-3-4-1.js**

### Changes:
#### isFunction() was deprecated
1. Change **$.isFunction(data)** to **typeof data === "function"**
2. Change **$.isFunction(this)** to **typeof this === "function"**

#### .on() function to attach a event handler is deprecated
1. Change **.load(function() { ... })** to **.on("load", function (...)}**