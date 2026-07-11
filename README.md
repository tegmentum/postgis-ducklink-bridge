# postgis-duckdb-bridge-dynlink

Phase A dynlink-mode duckdb bridge for `postgis` (target `postgis`).

The bridge imports only `compose:dynlink/linker` and dispatches SQL
scalar arms as CBOR envelopes through the resident provider
`postgis-composed`. Aggregate / cast / table / pragma / column paths
return `duckerror::unsupported` at Phase A scope.
