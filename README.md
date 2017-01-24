# piiom-tool library
Pixel Image Input, Output &amp; Memory tool library.

!!! Warning !!! At this time this repository is just a placeholder and contains no useful code or at most some testcases. !!! warning !!!

This tool library is specifically for pixel based file and memory formats and contains methods for reading from files, writing to files, structured memory dumping, structured memory manipulation, conversion to and from an extended raw format and analysis tools.  It is not intended as a graphics library in the sense of various filters, rotations and manipulations.  The purpose is to enable basic reading and writing of image files so that a target software can focus on its own target features.  It is our hope that piiom-tool library can be easily dropin / plugin for other projects.

# features

There are basically 5 parts to the tool library, namely:
+ supporting class interfaces
+ image file / buffer / stream reader / writer interfaces
+ image buffer interface
+ analyzer interface
+ minimal manipulation interface

Assuming:
`const piiom = require( './piiom' );`

## piiom object methods



## supporting class interfaces

piiom.createReader( source:{path-string|buffer|readable-file-handler|readable-stream}, options?:{object} ):{piiomReader|false}:{piiomReader|false}
piiom.createWriter( source:{path-string|buffer|writable-file-handler|writable-stream}, options?:{object} ):{piiomReader|false}:{piiomReader|false}

piiomReader#addListener( type:{string|event|array}, callback, options?:{object|integer} )
piiomReader#appendListener( type:{string|event|array}, callback, options?:{object|integer} ):{piiomEvent#|false}
piiomReader#prependListener( type:{string|event|array}, callback, options?:{object|integer} )
piiomReader#on( type:{string|event|array}, callback, options?:{object|integer} )
piiomReader#once( type:{string|event|array}, callback, options?:{object} )
piiomReader#remove( type:{string|event|array}, callback )
piiomReader#emit( type:{string|event|array} )

## Image file / stream reading interface

piiom.createReader( source:{path-string|buffer|file-handler|read-stream}, options?:{object} ):{piiomReader|false}:{piiomReader|false}

piiomReader#addListener( type:{string|event|array}, callback, options?:{object|integer} )
piiomReader#appendListener( type:{string|event|array}, callback, options?:{object|integer} ):{piiomEvent#|false}
piiomReader#prependListener( type:{string|event|array}, callback, options?:{object|integer} )
piiomReader#on( type:{string|event|array}, callback, options?:{object|integer} )
piiomReader#once( type:{string|event|array}, callback, options?:{object} )
piiomReader#remove( type:{string|event|array}, callback )
piiomReader#emit( type:{string|event|array} )

## Image file / stream / buffer writing interface

@TODO: give details


## Image buffer interface

@TODO: give details

## Image analyzer interface

@TODO: give details

## Image minimal manipulation interface

@TODO: give details

# target image types

+ extended raw
+ bmp (and it's many variations)
+ png
+ jpg
+ gif
+ WebP



