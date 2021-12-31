# Starter NPM Package

An empty starter for publishing to NPM, with Babel for Transpiling code.

Requirements:
- You need `npx` installed globally. 
  - `npm install -g npx`
  - Used by npm script for calling babel

## How to Use

1
```
git clone <this-repo>
```

2
Update in `package.json` the `name` field with

```json
"name" : "<package-name>",                 // UNSCOPED PACKAGE 
"name" : "@<npm-username>/<package-name>", // USER SCOPED PACKAGE 
"name" : "@<npm-organizationname>/<package-name>", // ORGANIZATION SCOPED PACKAGE 
```

3
When developing

```
npm start
```

4
When ready to publish - first time published

```
npm run build
npm publish --access public
```

4
When ready to publish - update published package 
Increment version in `package.json` if you are updating the package.

```
npm run build
npm publish
```