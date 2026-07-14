Quick build instructions to produce a Windows executable for this project.

Prerequisites
- Node.js and npm installed
- Git (optional)

Commands

1. Install dependencies:

```bash
npm install
```

2. Run the app (for testing):

```bash
npm run start
```

3. Build a Windows installer/exe (requires build toolchain on Windows):

```bash
npm run dist
```

Notes
- The build uses `electron-builder` and targets NSIS for Windows x64. If you need a portable exe only, adjust `package.json` `build.win.target`.
- If packaging fails due to missing native toolchain, follow electron-builder docs for Windows prerequisites.
