# electron-app-from-dist

An Electron application that loads a local web page from the 'dist' directory.

## Features

- Loads a local web page.
- Development and build scripts for multiple platforms.

## Prerequisites

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)

## Getting Started

1. Install the dependencies:

```sh
npm install
```

2. Run the application in development mode:

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

## License

This project is licensed under the MIT License.

## Contributions

Contributions are always welcome. Feel free to open issues, suggest improvements, or submit pull requests.