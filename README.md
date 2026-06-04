# FSD Template

🚀 A modern and scalable boilerplate built on top of the **Feature-Sliced Design** architectural methodology.

---

## 🛠 Tech Stack

- **Core:** [React 19](https://reactjs.org)
- **Type System:** [TypeScript](https://typescriptlang.org)
- **State Management:** [Redux Toolkit](https://redux-toolkit.js.org)
- **Build Tool:** [Vite](https://vite.dev)
- **Linter:** [ESLint](https://eslint.org) (pre-configured for FSD)

---

## 🏗 Architecture & Codebase Structure

The project strictly follows the **Feature-Sliced Design** layers:

- `app/` — Global initializers, providers, styles, and the application entry point.
- `pages/` — Composition layer assembling application screens from widgets.
- `widgets/` — High-level structural components combining features and entities.
- `features/` — User actions and interactions that bring distinct business value.
- `entities/` — Business logic, domain models, and state handling (e.g., Counter).
- `shared/` — Reusable UI components, API clients, utilities, and helper functions.

---

## 🚀 Quick Start

### Clone the repository
```bash
git clone https://github.com/mattuzik/vite-react-redux-fsd-template
```

### Install dependencies
```bash
npm install
```

### Run the development server
```bash
npm run dev
```

### Production build
```bash
npm run build
```

---

## 📏 Architecture & Coding Rules

1.  **Respect Layer Hierarchy:** A module can only import code from layers located strictly below it.
2.  **Public API:** Always use `index.ts` at the root of each module to export only the required functionality.
3.  **Strict Typing:** Explicit interfaces and types are mandatory for all application states, hooks, and component props.
