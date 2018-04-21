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
1. package file: package.json 
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

2. module file
3. intellisense enabled
4. platform independent
5. form enabled - control value accessor interface
6. AOT enabled
```bach
npm install @angular/compilter-cli
npm install @angular/platform-server

ngc
tsconfig.json -> tsconfig.aot.json
```

Don't use the JIT compilter
NgModule should be statically analyzable 
- convert your lamba to simple export functions
- conver default export to named export
- mark membets accessed from template as public
- convert dynamic component template to static templates
- export components explicitly
- use static selectors
- be more explicit about what you are using
include *.metadata.json in your package
tsc - ngc - .js compiled
tsc - ngc - .metadata.json
tsc - ngc - .d.ts

7. packaging
produce FESM but with caution

8. versioning
major.minor.patch
```bash
npm version [<newversion>] | major | minor | patch | premajor | preminor | prepatch | prerelease | from-git]
```
https://docs.npmjs.com/cli/version


9.Theme Enabled



Creating & Publishing Angular (2+) Component Libraries ft. Anas Firdousi
https://www.youtube.com/watch?v=tZZ8EQnX2cE

