# github-packages-demo

GitHub packages demo

## Usage

Create `.npmrc` file in your project

```
registry=https://npm.pkg.github.com/
```

Install the package:

```
npm install @taroalan/github-packages-demo@0.0.1 --save
```

## How to publish a package

Step 1: Use `publishConfig` option in your package.json

```json
{
  "publishConfig": {
    "registry": "https://npm.pkg.github.com/"
  }
}
```

Step 2: Authenticate

```shell
npm login --registry=https://npm.pkg.github.com/
```

Step 3: Publish

```
npm publish
```

[Read More](https://help.github.com/en/packages/using-github-packages-with-your-projects-ecosystem/configuring-npm-for-use-with-github-packages)
