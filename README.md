<!-- tyhp-readme:start -->
# tyhpdef/psr-container

Tyhp type definitions for `psr/container` `2.0.2`.

```bash
composer require --dev tyhpdef/psr-container:2.0.2
```

This is a metapackage. Composer also installs `tyhpdef/psr-container-impl` (type files).
Require **this** name, not `tyhpdef/psr-container-impl`.

See https://tyhplang.com.

## Maintain `psr/container`? Ship the types yourself

If you are a Packagist maintainer of `psr/container`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/psr-container-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `psr/container` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/psr-container": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `psr/container` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `psr/container` with a real constraint,
   `"replace": { "tyhpdef/psr-container": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `psr/container` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/psr-container` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
