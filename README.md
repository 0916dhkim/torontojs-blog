# Toronto JS blog

## Pre-requisites

- [Node.js](https://nodejs.org/en/download/)
- [npm](https://www.npmjs.com/get-npm)
- [mkcert](https://github.com/FiloSottile/mkcert)

## Running the project

Check detailed documentation on the project setup and how to get it running in [`src/content/docs/setup.md`](./src/content/docs/setup.md).

## Commands

All commands are run from the root of the project, from a terminal:

| Command | Action |
| :--- | :--- |
| `npm install` | Installs all dependencies |
| `npm start` | Starts local dev server at [`https://localhost:3000/`](https://localhost:3000/) |
| `npm run build` | Build your production site to `./dist/` |
| `npm run preview` | Preview your build locally, before deploying |
| `npm run astro ...` | Run CLI commands like `astro add`, `astro check` |
| `npm run lint` | Checks the project for errors and fix most of them |


## Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── .astro/
|-- .github/
|-- .husky/
|-- .vscode/
|-- certs/
├── dist/
├── node_modules/
├── public/
├── src/
│   └── components/
|   └── js/
│   └── layouts/
│   └── pages/
│   └── styles/
|   └── env.d.ts
|   └── manifest.json
|   └── sw-caching.ts
├── .eslintrc
├── .stylelintrc
├── .markuplintrc
├── .gitignore
├── astro.config.ts
├── package.json
├── package-lock.json
├── tsconfig.json
└── README.md
```

- `.astro/`: Astro's internal files, this is auto generated and should not be modified.
- `.github/`: GitHub configuration files, including the actions to run when code is pushed and alerts about dependencies.
- `.husky/`: Husky is a tool that hooks into git and run commands before actions are made, such as commits and pushes.
- `.vscode/`: Visual Studio Code configuration files, including settings, extensions, and tasks.
- `certs/`: SSL certificates for local development.
- `dist/`: The output of `npm run build`, this is the production site.
- `node_modules/`: The dependencies of the project. This is generated by `npm install`.
- `public/`: Static files for the project, those are copied without any processing to the `dist/` folder and are available at the root of the site.
- `src/`: The source code of the project.
  - `components/`: Reusable components that are used across multiple pages.
  - `js/`: JavaScript files that are not components, like scripts that run on the client side.
  - `layouts/`: Resuable layouts that are used across multiple pages.
  - `pages/`: Pages are the main content of the site, they are the entry points of the site.
  - `styles/`: Styles are the CSS files of the project.
  - `env.d.ts`: Global typescript type file, used to declare global variables and other things that should be made available throughout the project.
  - `manifest.json`: Web App Manifest file, used to configure the PWA part of the project.
  - `sw-caching.ts`: Service Worker caching strategies to be used. This is what instructs the service worker on how to cache the site.
- `.eslintrc`: ESLint configuration file, used to configure the linter for JavaScript and TypeScript files.
- `.stylelintrc`: Stylelint configuration file, used to configure the linter for CSS files.
- `.markuplintrc`: Markuplint configuration file, used to configure the linter for HTML and Astro files.
- `.gitignore`: Git configuration file, used to tell git which files to ignore.
- `astro.config.ts`: Astro configuration file, used to configure Astro's behavior.
- `package.json`: NPM configuration file, lists out the project's dependencies and some configuration.
- `package-lock.json`: NPM lock file, used to lock the versions of the dependencies.
- `tsconfig.json`: TypeScript configuration file, used to configure the TypeScript compiler.
- `README.md`: This file.

## Contributing

If you want to contribute to the project, please read the [contributing guide](./src/content/docs/contributing.md).
