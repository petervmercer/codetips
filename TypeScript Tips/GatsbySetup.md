# TypeScript in GatsbyJs

## Setup

### Install

```shell script
yarn add gatsby-plugin-typescript
yarn add typescript --dev
```

Once the dependencies are installed, we can add gatsby-plugin-typescript to the gatsby-config.js

```shell script
gatsby-plugin-offline,
gatsby-plugin-react-helmet,
gatsby-plugin-typescript,
```

### tslint.json

Add tslint.json to the root directory

```json
{
  "extends": ["tslint-react"],
  "rules": {
    "prettier": true,
    "jsx-no-multiline-js": false,
    "jsx-no-lambda": false,
    "import-name": false,
    "no-boolean-literal-compare": false
  }
}
```

### tsconfig.json

Add tsconfig.json to the root directory

```json
{
  "compilerOptions": {
    "module": "commonjs",
    "target": "esnext",
    "jsx": "preserve",
    "lib": ["dom", "esnext"],
    "strict": true,
    "noEmit": true,
    "isolatedModules": true,
    "esModuleInterop": true,
    "noUnusedLocals": false,
    "allowJs": true
  },
  "exclude": ["node_modules", "public", ".cache"]
}
```

