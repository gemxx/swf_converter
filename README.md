# swfpack
The tool to convert swf format between uncompressed/zlib/lzma.

# Usage
var converter = new swfpack(targetPath); // targetPath: buffer|absolute_path
var buffer_fws = converter.pack('fws'); // fws (uncompressed)
var buffer_cws = converter.pack('cws'); // cws (compressed by using the ZLIB open standard)
var buffer_zws = converter.pack('zws', 7); // zws, lzma level 1-9 (compressed by using the LZMA open standard)

