# Setup

## Install

```shell script
npm install -g typescript
```

Check install 

```shell script
tsc --help
```

## Using tsc

### Creating a tsconfig

```shell script
tsc --init
```

#### Json example

```json
{
  "compilerOptions": {
    "target": "es5",
    "module": "esnext",
    "lib": ["dom", "esnext"],
    "importHelpers": true,
    "declaration": true,
    "sourceMap": true,
    "rootDir": "./",
    "strict": true,
    "pretty": true,
    "removeComments": true,
    "noImplicitAny": true,
    "strictNullChecks": true,
    "strictFunctionTypes": true,
    "strictPropertyInitialization": true,
    "noImplicitThis": true,
    "alwaysStrict": true,
    "stripInternal": true,
    "noUnusedLocals": true,
    "noUnusedParameters": true,
    "noImplicitReturns": true,
    "noFallthroughCasesInSwitch": true,
    "emitDecoratorMetadata": false,
    "experimentalDecorators": false,
    "moduleResolution": "node",
    "jsx": "react",
    "esModuleInterop": true,
    "allowSyntheticDefaultImports": true
  },
  "include": ["src", "types"],
  "exclude": ["node_modules", "dist"]
}
```

#### Can import for abstraction

```json
{
  "extends": "./tsconfig.base.json",
  "include": ["src", "types"],
  "compilerOptions": {
    "baseUrl": "./",
    "paths": {
      "scorm2aws": ["src/"]
    }
  }
}
```

### Watching for changes

```shell script
tsc -w
```


