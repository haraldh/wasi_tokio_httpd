# wasihttp

Be sure to update your rust stable toolchain to at least 1.60.0.

## wasmtime

```console
❯ CARGO_TARGET_WASM32_WASI_RUNNER="wasmtime run --tcplisten 127.0.0.1:8080" cargo run --target wasm32-wasi  
```

Server is running on [`http://127.0.0.1:8080`](http://127.0.0.1:8080).

## enarx

after installing [enarx](https://github.com/enarx/enarx/) in `$PATH` with `cargo install`

```console
❯ CARGO_TARGET_WASM32_WASI_RUNNER="enarx run --wasmcfgfile Enarx.toml" cargo run --target wasm32-wasi 
```

Server is running on [`https://127.0.0.1:8080`](https://127.0.0.1:8080).
