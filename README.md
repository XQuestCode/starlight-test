# SplashKit SDK - Starlight Framework

## Introduction
Welcome to the official documentation for the SplashKit SDK on the Starlight framework! This readme markdown script will guide you through the installation process and provide an overview of the features and functionalities of the SDK.

## Installation
1. Clone/Fork this repository.
1. Install the necessary dependencies. Make sure you have the following installed:
    ```
    npm install
    ```
## 🚀 Project Structure

Inside of your Astro + Starlight project, you'll see the following folders and files:

```
.
├── public/
└── src/
    ├── assets/
    ├── content/
    │   ├── docs/
    │   ├── components/
    │   ├── guides/
    │   ├── installation/
    │   └── troubleshoot/
    ├── styles/
    ├── config.ts
    └── env.d.ts
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

Starlight looks for `.md` or `.mdx` files in the `src/content/docs/` directory. Each file is exposed as a route based on its file name.

Images can be added to `src/assets/` and embedded in Markdown with a relative link.

Static assets, like favicons, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:3000`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |
| `npm run generate-mdx`             | Generate MDX file *(for functions)* from JSON data in `test` folder                   |

## Contributing
We welcome contributions from the community to enhance the SplashKit SDK on the Starlight framework. If you would like to contribute, please follow the guidelines outlined in the CONTRIBUTING.md file.

