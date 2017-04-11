Assemble `geoserver.war` with modules using nightly files


## Requirements

* `bash`
* `coreutils` (or equivalent)
* `curl`
* `zip` and `unzip`


## Quickstart

1. Copy `settings.conf.example` to `settings.conf`
2. Edit `settings.conf` as needed
   * `DATE`
   * `VERSION` and `BRANCH`
   * `EXTENSION_NAMES` and `COMMUNITY_NAMES`
3. Run `./gsawn settings.conf`
   * Nightly files are saved under `nightly/${BRANCH}/`
   * `geoserver.war` is saved under `build/${BRANCH}/${DATE}/`


## Caveats

This merely assembles a `geoserver.war` file that contains the desired plugins.
It does not handle external dependencies (eg, native libraries).
It does not handle any custom configuration for a plugin.
