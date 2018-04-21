## Library Life Cycle in Angular

1. Plan
2. Develop
3. Unit Test
4. Integration Setup
5. Env Test
6. Publish
7. Enhance
8. Growth Hack


## Essentials of a Angular Component Library
Library should be reusable module, so the user can npm install it like other angular components.
```bash
npm install my-some-library --save
```
1. package.json 
```bash
npm init
```

```js
{
.....
"main": "magic-mask.umd.js"
"module":"index.es5.js",
"es2015":"index.js",
"typings":"index.d.ts",
"peerdependencies":{
"@angular/core":"^2.4.0 || ^4.0.0",
"rxjs": "^5.0.1"}
}
```

2. module
3. intellisense enabled
4. platform independent
5. form enabled
6. AOT enabled
7. packaging
8. versioning






Creating & Publishing Angular (2+) Component Libraries ft. Anas Firdousi
