# Hello WASM

This project is used as an example of how to get started working with WASM as part of a [larger tutorial](https://freemasen.github.io/wasm_tutorial). You can find a live demo of it [here]().

To build this project you can execute the following commands.

```bash
git clone https://github.com/freemasen/wasm_hw
cd wasm_hw
cargo +nightly build --target wasm32-unknown-unknown
wasm-bindgen ./target/wasm32-unknown-unknown/debug/hello_world.wasm --out-dir .
yarn
#or npm install
./node_modules/.bin/webpack-dev-server
```
> If you don't have `rust`, `nightly`, the `wasm32-unknown-unknown`, or target `wasm-bindgen`; [follow along here](https://freemasen.github.io/wasm_tutorial/setps/02-getting-started.html) to get started

At this point you can open firefox and navigate to `localhost:8080` to see it working.