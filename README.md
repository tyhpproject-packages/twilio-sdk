<!-- tyhp-readme:start -->
# tyhpdef/twilio-sdk

Tyhp type definitions for `twilio/sdk` `8.12.1`.

```bash
composer require --dev tyhpdef/twilio-sdk:8.12.1
```

This is a metapackage. Composer also installs `tyhpdef/twilio-sdk-impl` (type files).
Require **this** name, not `tyhpdef/twilio-sdk-impl`.

See https://tyhplang.com.

## Maintain `twilio/sdk`? Ship the types yourself

If you are a Packagist maintainer of `twilio/sdk`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/twilio-sdk-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `twilio/sdk` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/twilio-sdk": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `twilio/sdk` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `twilio/sdk` with a real constraint,
   `"replace": { "tyhpdef/twilio-sdk": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `twilio/sdk` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/twilio-sdk` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
