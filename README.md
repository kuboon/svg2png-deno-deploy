# svg2png-deno-deploy

[svg2png-wasm](https://github.com/ssssota/svg2png-wasm) demo with Deno Deploy.

Convert online svg to png.

## Usage

`https://svg2png.deno.dev/[svg url]`

e.g.

`https://svg2png.deno.dev/https://github.com/ssssota/svg2png-wasm/raw/main/logo.svg`

![](https://svg2png.deno.dev/https://github.com/ssssota/svg2png-wasm/raw/main/logo.svg)

### options

#### `svg2png-scale=N`

e.g.

`https://svg2png-worker.ssssota.workers.dev/https://github.com/ssssota/svg2png-wasm/raw/main/logo.svg?svg2png-scale=10`

![](https://svg2png-worker.ssssota.workers.dev/https://github.com/ssssota/svg2png-wasm/raw/main/logo.svg?svg2png-scale=10)

#### `svg2png-background=COLOR`

e.g.

`https://svg2png-worker.ssssota.workers.dev/https://github.com/ssssota/svg2png-wasm/raw/main/logo.svg?svg2png-background=black`

![](https://svg2png-worker.ssssota.workers.dev/https://github.com/ssssota/svg2png-wasm/raw/main/logo.svg?svg2png-background=black)

`https://svg2png-worker.ssssota.workers.dev/https://github.com/ssssota/svg2png-wasm/raw/main/logo.svg?svg2png-background=rgba(127,127,127,0.5)`

![](<https://svg2png-worker.ssssota.workers.dev/https://github.com/ssssota/svg2png-wasm/raw/main/logo.svg?svg2png-background=rgba(127,127,127,0.5)>)

## License

MIT

This project use [resvg](https://github.com/RazrFalcon/resvg) that project is
licensed under the MPLv2.0. You can see resvg source from
[here](https://github.com/RazrFalcon/resvg).
