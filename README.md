# LightBWS for LazyCat

This repository packages [LightBWS](https://github.com/ca-x/lightbws) as the
LazyCat application `community.lazycat.app.lightbws`.

The scheduled GitHub Actions workflow watches stable tags from
`docker.io/czyt/lightbws`, copies the selected `linux/amd64` image to the
LazyCat registry, builds a versioned LPK Release asset, and reconciles both the
official LazyCat store and the configured private store.

## Required GitHub Actions secrets

- `LAZYCAT_TOKEN`
- `APPSTORE_URL`
- `APPSTORE_TOKEN`

Optional private-store secrets are `APP_ID` and
`PRIVATE_STORE_GROUP_CODES`.
