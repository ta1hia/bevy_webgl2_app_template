# Template of multi-target (WASM / Native) Bevy's application

## Prerequisites

```
nix-shell default.nix
cargo install cargo-make 
cargo install wasm-bindgen-cli
```

## Build and serve WASM version
```
cargo build --target wasm32-unknown-unknown --features web
cargo make serve
```
then point your browser to http://127.0.0.1:4000/


## Build and run native version
```
cargo make run
```

![Screenshot](https://mrk.sed.pl/bevy-showcase/assets/bevy_webgl2_app_template.png?v=3)
