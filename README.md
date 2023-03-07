# Leptos App

A Single Page Application (SPA) in Rust using Leptos framework, Tailwind CSS and Trunk build tools.

## Overview

Template includes:
- Routing
- Global state
- Components, Models and Pages module structure
- Tailwind CSS

## Dev dependencies

Web Assembly build target
```bash
rustup target add wasm32-unknown-unknown
```

Leptos docs (optional)
```bash
cargo install mdbook

mkdir -p $HOME/repo
pushd $HOME/repo

git clone --depth 1 https://github.com/leptos-rs/leptos.git && cd leptos/docs/book && mdbook serve

popd

```

VS Code extensions
- rust-analyzer (The Rust Programming Language)
- Tailwind CSS IntelliSense (Tailwind Labs)
- Code Spell Checker (Street Side Software)
- GitLens (GitKraken)
- Bicep (Microsoft)
- Azure Functions (Microsoft)

## Setup

Tailwind dev service
```bash
npm install
npx tailwindcss -i ./styles/input.css -o ./styles/tailwind.css --watch
```

Trunk dev service
```bash
cargo install trunk
trunk serve
```

## Build
```bash
npx tailwindcss -i ./styles/input.css -o ./styles/tailwind.css --minify

trunk build

ls -la dist
```

