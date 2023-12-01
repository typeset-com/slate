This package contains the React-specific logic for Slate, which has been patched for use in Typeset/Dropdeck. It's separated further into a series of directories:

- [**Components**](./src/components) — containing the React components for rendering Slate editors.
- [**Hooks**](./src/hooks) — containing a few React hooks for Slate editors.
- [**Plugins**](./src/plugin) — containing the React-specific plugins for Slate editors.
- [**Utils**](./src/utils) — containing a few private convenience modules.

Feel free to poke around in each of them to learn more!

# Build and deployment
You build the package by running `yarn build` in the root of the `slate` repo. Once built, navigate into this repository and do the following:

```
npm login # if you haven't already; you need to login as an account with access to the dropdeck-slate-react project on NPM.js
npm publish --dry-run # to test that everything is working
npm publish # to publish the package; note this requires a one-time password from your authenticator app
```

**Note**: Make sure to update the version number in `package.json` before publishing.
