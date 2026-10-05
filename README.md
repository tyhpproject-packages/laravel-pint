<!-- tyhp-readme:start -->
# tyhpdef/laravel-pint

Tyhp type definitions for `laravel/pint` `1.32.1`.

```bash
composer require --dev tyhpdef/laravel-pint:1.32.1
```

This is a metapackage. Composer also installs `tyhpdef/laravel-pint-impl` (type files).
Require **this** name, not `tyhpdef/laravel-pint-impl`.

See https://tyhplang.com.

## Maintain `laravel/pint`? Ship the types yourself

If you are a Packagist maintainer of `laravel/pint`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/laravel-pint-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `laravel/pint` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/laravel-pint": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `laravel/pint` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `laravel/pint` with a real constraint,
   `"replace": { "tyhpdef/laravel-pint": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `laravel/pint` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/laravel-pint` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
