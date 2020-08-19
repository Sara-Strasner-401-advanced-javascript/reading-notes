# Local Storage
Before HTML5, application data had to be stored in cookies, included in every server request. HTML5 set out to provide a standardized API, implemented natively and consistently in multiple browsers, without having to rely on third-party plugins.

## HTML5 Storage
HTML5 storage is a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, etc. Unlike cookies, this data is never transmitted to the remote web server. Certain browser vendors also refer to it as “Local Storage” or “DOM Storage.” HTML5 data can be any type supported by JavaScript, including strings, Booleans, integers, or floats.

Within JavaScript code, you can access HTML5 Storage through the `localStorage` object on the global `window` object.

If you want to keep track programmatically of when the storage area changes, you can trap the `storage` event, which is fired on the `window` object whenever `setItem()`, `removeItem()`, or `clear()` is called and actually changes something.

**Data is stored as strings. If you are storing and retrieving anything other than strings, you will need to use functions like `parseInt()` or `parseFloat()` to coerce your retrieved data into the expected JavaScript datatype.** 

## Limitations in Current Browsers
- 5 megabytes is how much storage space each origin gets by default. “QUOTA_EXCEEDED_ERR” is the exception that will get thrown if you exceed your storage quota of 5 megabytes.
- You cannot ask the user for more storage space. 
