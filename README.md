# workers-sdk-require-debug-repro

`vendor/ext-dep` is a CommonJS dependency.

`ext-dep/index.js` requires `debug`, which doesn't work in `@cloudflare/vitest-pool-workers`.

```
pnpm i
pnpm test
```

```
TypeError: Cannot use require() to import an ES Module.
```
