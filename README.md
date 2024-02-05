# electron-app-from-dist

An Electron application that loads a local web page from the 'dist' directory.

## Features

- Loads a local web page.
- Development and build scripts for multiple platforms.

## Prerequisites

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)

## Getting Started

1. Clone the repository:

```sh
git clone git@github.com:quecot/electron-app-from-dist.git
```

2. Populate the `dist/` dist directory with your web application files.

3. Install the dependencies:

```sh
npm install
```

4. Run the application in development mode:

```sh
npm run dev
```

## Building for production

To build the application for production, use the provided npm scripts:

- For macOS (ARM64):

```sh
npm run build:macos-arm64
```

- For Windows (64-bit):

```sh
npm run build:windows
```

- For Windows (32-bit):

```sh
npm run build:windows-32
```

**Note**: Remember to replace `**YOUR_APP_NAME**` in the build scripts with your desired application name in the `package.json`.

## Note for Vite Users

If you're building your web application with Vite, ensure you set "base": "./", in your vite.config.js or vite.config.ts to ensure correct asset paths in the built Electron app.

## Note for Astro Users

Astro does not allow for non-url paths as base, which can be seen discussed in [this issue](https://github.com/withastro/astro/issues/2163#issuecomment-994145837). For a quick fix, you can check out [astro-relative-links](https://www.npmjs.com/package/astro-relative-links).

## License

This project is licensed under the MIT License.

## Contributions

Contributions are always welcome. Feel free to open issues, suggest improvements, or submit pull requests.
