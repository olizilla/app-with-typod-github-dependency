# Test for typos in git url dependencies in `package.json`

See: https://github.com/npm/npm/issues/10401

This repo contains an example `package.json` that declares a dependency on a github url.
The name it gives for the dep doesn't match the name property of the deps package.json.

`npm install` with `npm@3.4.0` completes with no error, but the dep is not installed.