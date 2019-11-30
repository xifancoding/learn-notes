# Jest Summary

## getting started

Start `ts-jest` in your project:

Steps | commonds
--- | --- |
   `installing` | *npm install --save-dev jest typescript ts-jest @types/jest*
   `create jest.config.js` | *npx ts-jest config:init*

Add the following section to your `jest.config.js`:

```javascript
module.exports = {
    transform: {
        "^.+\\.(ts|tsx)$": "ts-jest"
    },
    testRegex: "(/__tests__/.*| (\\.| /)(test|spec))\\.(jsx?|tsx?)$",
    moduleFileExtensions: ["ts", "tsx", "js", "jsx", "json", "node"],
};
```

Add the following section to your `pakage.json`:

```json
{
    ...
    "scripts": {
         ...
        "test": "jest"
         ...
    }
    ...
}
```

Using Jest in your project teminal

```javascript
jest
//OR
nmp test
```

Building your test files:

1. all the files in the folder `"${workspaceFolder}/__tests__/*"`.
2. all the files names `"${name}.test|spec.js|ts"`.

[...more](https://jestjs.io/docs/en/getting-started)
