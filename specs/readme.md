# Protocol Specifications

The files in this folder are derived from source files in other repos as follows:

## Park Observer 1.x
* `Protocol_Guide_v1.html` -- https://github.com/regan-sarwas/Observer/blob/master/Observer/Protocols/Protocol%20Guide.md
* `Protocol_Specification_V2.html`  -- https://github.com/regan-sarwas/Observer/blob/master/Observer/Protocol%20Specification%20V2.md

## Park Observer 2.x
* `Protocol_Guide_v2.html` -- https://github.com/regan-sarwas/Park-Observer/blob/master/Park%20Observer/Documentation/Protocol%20Guide.md
* `Protocol_Specification_V2.2.html` -- https://github.com/regan-sarwas/Park-Observer/blob/master/Park%20Observer/Documentation/Protocol%20Specification.md

## Protocol Schema Validation

* `protocol.v1.schema.json` -- https://github.com/regan-sarwas/Park-Observer/blob/master/Park%20Observer/Documentation/protocol.v1.schema.json
* `protocol.v2.schema.json` -- https://github.com/regan-sarwas/Park-Observer/blob/master/Park%20Observer/Documentation/protocol.v2.schema.json
* `csv.json` -- https://github.com/regan-sarwas/poz2fgdb/blob/master/csv.json


The `json` files are copied exactly.  The `html` files are basically
wrappers with minimal formatting (css) and header around the html
representation of the source markdown file.  I've used https://markdowntohtml.com
for the conversion but [pandoc](https://pandoc.org), [dillinger](https://dillinger.io),
[atom](https://atom.io) or any other similar tool will probably work fine.
