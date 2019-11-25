# MWS SV Secondary target selection notebooks and raw data

Each directory corresponds to one SV target class.

### Avoid duplicating raw input catalogs

Some target classes use the same raw catalog, for example to select in
different magnitude ranges. For example, `MWS_CALIB_APOGEE` and
`MWS_CALIB_APOGEE_VERYBRIGHT`. In these cases, the catalog under `/raw` for all but
one of these classes should be a symlink. For example,
`MWS_CALIB_APOGEE_VERYBRIGHT/1/raw/...fits` is a symlink to
`MWS_CALIB_APOGEE/1/raw/..fits`.
