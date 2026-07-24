<img src="docs/assets/banner.svg" alt="Emscripten-forge Banner" style="width: 80%;">

#

[![CI](https://img.shields.io/badge/emscripten_forge-docs-yellow)](https://emscripten-forge.org)
[![CI](https://img.shields.io/badge/emscripten_forge-blog-pink)](https://emscripten-forge.org/blog/)


Visit [emscripten-forge.org](https://emscripten-forge.org) for more information and the documentation.

To build a package completely locally, run 
`curl -fsSL https://pixi.sh/install.sh | sh`
`pixi global install rattler-build=0.70.1`
`rattler-build build --recipe recipes/recipes/emscripten_emscripten-wasm32 --output-dir local-channel -c conda-forge`
`rattler-build build --recipe-dir recipes/recipes_emscripten --up-to <package name> --target-platform=emscripten-wasm32 --output-dir local-channel -c "file://$PWD/local-channel" -c conda-forge`

