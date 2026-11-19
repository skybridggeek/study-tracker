# Study Tracker

<div align="center">

**A React and TypeScript foundation for a modern study-tracking application**

[![React](https://img.shields.io/badge/React-19-61DAFB?logo=react&logoColor=white)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-6-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-8-646CFF?logo=vite&logoColor=white)](https://vite.dev/)
[![License](https://img.shields.io/badge/license-not%20specified-lightgrey)](#license)

</div>

## Overview

Study Tracker is a front-end project built with React, TypeScript, and Vite. It currently provides a polished starter interface with responsive layouts, dark-mode-aware styling, and a small interactive counter. The application is ready to be expanded into a full study-tracking tool.

> **Project status:** The repository is in the initial UI/starter stage. Features such as subjects, study sessions, progress metrics, persistence, and authentication have not been implemented yet.

## Current Features

- React 19 application using functional components and hooks
- Strict TypeScript configuration
- Vite development server with Hot Module Replacement (HMR)
- Responsive desktop and mobile layout
- Automatic light and dark theme styling via `prefers-color-scheme`
- Accessible SVG icons and semantic page sections
- Interactive counter demonstrating React state
- ESLint rules for JavaScript, TypeScript, React Hooks, and React Refresh
- Optimized production build with Vite

## Tech Stack

| Area | Technology |
| --- | --- |
| UI | React 19 |
| Language | TypeScript 6 |
| Build tool | Vite 8 |
| Styling | CSS / CSS nesting |
| Development rules | ESLint 10 |
| Package manager | npm |

## Project Structure

```text
study-tracker/
├── public/
│   ├── favicon.svg          # Browser tab icon
│   └── icons.svg            # Reusable SVG icon definitions
├── src/
│   ├── assets/
│   │   ├── hero.png         # Main illustration
│   │   ├── react.svg        # React logo
│   │   └── vite.svg         # Vite logo
│   ├── App.tsx              # Root application component
│   ├── App.css              # Component and layout styles
│   ├── index.css            # Global theme and base styles
│   └── main.tsx             # React entry point
├── eslint.config.js         # ESLint configuration
├── index.html               # HTML entry document
├── package.json             # Dependencies and npm scripts
├── tsconfig.app.json        # Application TypeScript settings
├── tsconfig.node.json       # Node/config TypeScript settings
└── vite.config.ts           # Vite configuration
```

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) 20.19+ or 22.12+
- npm, included with Node.js
- A modern browser

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/skybridggeek/study-tracker.git
   cd study-tracker
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the development server:

   ```bash
   npm run dev
   ```

4. Open the local address shown by Vite, usually:

   ```text
   http://localhost:5173
   ```

The browser refreshes automatically as source files are edited.

## Available Scripts

| Command | Description |
| --- | --- |
| `npm run dev` | Start the Vite development server with HMR |
| `npm run build` | Type-check the application and create a production build in `dist/` |
| `npm run lint` | Run ESLint across the project |
| `npm run preview` | Serve the production build locally for testing |

## Development

Application code is located in `src/`. The entry point renders `App` from [src/main.tsx](src/main.tsx), while the current UI and state are implemented in [src/App.tsx](src/App.tsx).

- Add application components below `src/` and import them from `App.tsx`.
- Use [src/App.css](src/App.css) for component and layout-specific styles.
- Use [src/index.css](src/index.css) for global styles and theme variables.
- Place static images or fonts in `src/assets/` or `public/`, as appropriate.
- Keep reusable SVG symbols in [public/icons.svg](public/icons.svg).

Before submitting a change, run:

```bash
npm run lint
npm run build
```

## Deployment

Build the application for production:

```bash
npm run build
```

The generated `dist/` directory can be deployed to any static-hosting provider, including GitHub Pages, Netlify, Vercel, or Cloudflare Pages. Configure the host to publish the `dist/` directory and, for a subdirectory deployment, set the appropriate Vite `base` option in [vite.config.ts](vite.config.ts).

## Planned Improvements

The following features are natural next steps but are not implemented in the current codebase:

- Subject and course management
- Study-session timer
- Daily, weekly, and monthly progress views
- Study goals and streak tracking
- Session history and notes
- Local browser persistence
- Optional cloud synchronization and authentication
- Tests and automated CI workflows

## Contributing

Contributions are welcome. When contributing:

1. Fork the repository.
2. Create a focused feature branch.
3. Follow the existing React and TypeScript structure.
4. Run `npm run lint` and `npm run build`.
5. Open a pull request with a clear description of the change.

## License

No license has been specified for this repository. Add a license file before distributing or accepting contributions if you intend to publish the project.
