# portfolio-web

henryheffernan.com の3Dポートフォリオサイトのソースを、学習用に取り込んだリポジトリです。

A study copy of the source for Henry Heffernan's 3D portfolio website, [henryheffernan.com](https://henryheffernan.com/). The page renders a desk and a retro computer in Three.js; the screen of the computer shows a separate 2D "OS" site ([portfolio-inner-site](https://github.com/henryjeff/portfolio-inner-site)).

This repository is kept to read and learn from the code. The original design and code are by Henry Heffernan.

## Features

- Three.js scene with a custom camera controller, GLSL shaders and spatial audio
- Tween.js camera animations when you move to the screen
- Loading screen and overlay UI built with React and Framer Motion
- Express server that serves the production build and a contact form endpoint

## Usage

Node.js and npm are required.

```sh
git clone https://github.com/Sol-momma/portfolio-web.git
cd portfolio-web
npm install
npm run dev        # webpack dev server
```

Production build:

```sh
npm run build      # outputs to public/
npm start          # serves public/ with Express on port 8080
```

The contact form needs SMTP settings from environment variables; the rest of the site works without them.

## Project structure

```text
bundler/            # webpack configs (dev / prod)
server/             # Express server
src/Application/    # Three.js app: Camera, Renderer, World, Shaders, Audio, UI
static/             # models, textures, images and audio
```

## Tech stack

- TypeScript, Three.js, GLSL
- React, Framer Motion, Tween.js
- webpack, Express

## License

[MIT](LICENSE.md), copyright Henry Heffernan.
