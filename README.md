`@delphi/common` is the SvelteKit project producing the package we want to import. `@delphi/common/package` is the package directory (after running `npm run package` from `@delphi/common`).

In the root package, we can run `npm install --save-dev ./@delphi/common/package`, and the package `my-test-package` (the name given in `@delphi/common/package.json`) will be available to us in the root package as `import MyComponent from 'my-test-package/MyComponent.svelte'`.
