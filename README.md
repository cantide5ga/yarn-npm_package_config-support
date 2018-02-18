# Demo of yarn support for $npm_package_config

Tested with yarn 1.3.2.

npm correctly replaces the config value for key `foo` with `baz`.  yarn **does not** replace default `bar`; also doesn't seem to know what to do with the config directive switch and just echos it.

`npm run demo --yarn-npm_package_config-support:foo=baz`

vs.

`yarn run demo --yarn-npm_package_config-support:foo=baz`