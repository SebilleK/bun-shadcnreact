# Template Info

## bun-shadcnreact

Vite + React template (Typescript) using Bun and TailwindCSS + shadcn/ui for styling. Simply start off with [shadcn/ui](https://ui.shadcn.com/) directly and install the components you need.

Example:

```bash
bunx --bun shadcn-ui@latest add switch
```

This was made for personal use but feel free to clone this template as well.

## Quickstart

To use this template:

```bash
git clone https://github.com/SebilleK/bun-shadcnreact # clone this repo
cd bun-shadcnreact
bun i # install dependencies
bun run dev # start the server
```

To build app for production:

```bash
bunx --bun vite build
```

References:

- https://bun.sh/guides/ecosystem/vite
- https://tailwindcss.com/docs/installation
- https://ui.shadcn.com/docs/installation/vite

# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default {
	// other rules...
	parserOptions: {
		ecmaVersion: 'latest',
		sourceType: 'module',
		project: ['./tsconfig.json', './tsconfig.node.json'],
		tsconfigRootDir: __dirname,
	},
};
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list
