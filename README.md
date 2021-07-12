# Flyyer x Docusaurus

To create dynamic image previews please refer to [docs.flyyer.io](http://docs.flyyer.io/).

**This plugin required [Docusaurus v2](https://v2.docusaurus.io/).** There is no support for v1.

## Install

```bash
yarn add @flyyer/docusaurus-preset

# or with npm
npm install --save @flyyer/docusaurus-preset
```

On your `docusaurus.config.js` add `@flyyer/docusaurus-preset` at the end of your `presets` array:

```js
{
  // ...
  presets: [
    // ...
    [
      "@flyyer/docusaurus-preset",
      {
        /**
         * Get your project's identifier at https://flyyer.io/dashboard/_/projects/_/integrate
         */
        project: "",
      },
    ],
  ],
}
```

## Development

Clone this repository with:

```bash
git clone https://github.com/useflyyer/docusaurus-preset.git
cd docusaurus-preset
```

Install dependencies and bootstrap [Lerna](https://github.com/lerna/lerna/):

```bash
yarn install
yarn run bootstrap
```

Build packages:

```bash
yarn run build
```

## Publishing

Create a new [Lerna version](https://github.com/lerna/lerna/tree/main/commands/version#readme):

```bash
yarn run lerna version
```

Publish packages:

```bash
yarn run lerna publish from-git --yes
```
