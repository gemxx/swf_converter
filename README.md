# swfpack
Swfpack is a tool that convert swf format between uncompressed/zlib/lzma.

# Installation
    $ npm install swfpack

# Usage
````
var swfpack = require('swfpack');

var converter = new swfpack(file); //  file <String>|<Buffer>
var buffer_fws = converter.pack('fws'); // fws (uncompressed)
var buffer_cws = converter.pack('cws'); // cws (compressed by using the ZLIB open standard)
var buffer_zws = converter.pack('zws', 7); // zws (compressed by using the LZMA open standard), lzma level 1-9
````

#License
MIT
