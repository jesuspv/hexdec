NAME
   hexdec - decode masked hexadecimal data

SYNOPSIS
   hexdec options metadata

VERSION
   0.0.0

DESCRIPTION
   The hexdec utility decodes hexadecimal data via custom dictionaries.

   The dictionary is defined via the environment variables prefixed by HEXDEC_. For each
   variable HEXDEC_ENTRY=VALUE, ENTRY is the decoded representation and VALUE the hex
   bitmask. For instance:

      HEXDEC_SERVICE=0x000000ff
      HEXDEC_ROUTER=0x0003ff00
      HEXDEC_PORT_STATUS=0x80000000

   In case bitmasks overlap, all the matchings are printed.

OPTIONS:
   -h, --help                 display this help
   -v, --version              display program version
