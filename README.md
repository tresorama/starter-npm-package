# Starter NPM Package

An empty starter for publishing to NPM, with Babel for Transpiling code.

Requirements:
- You need `npx` installed globally. 
  - `npm install -g npx`
  - Used by npm script for calling babel

## How to Use

**1**
```
git clone <this-repo> <directory-name>
cd <directory-name>
npm i
```

**2 - Add a package name**

Update in `package.json` the `name` field with

```json
"name" : "<package-name>",                 // UNSCOPED PACKAGE 
"name" : "@<npm-username>/<package-name>", // USER SCOPED PACKAGE 
"name" : "@<npm-organizationname>/<package-name>", // ORGANIZATION SCOPED PACKAGE 
```

**3 - When developing**

```
npm start
```

For test your package you can use one of these:
- `npm link` - search on google ()
- run `npm install absolute/path/to/package` from other project directory

**4 - When ready to publish, if first time publish**

```
npm run build
npm publish --access public
```

**4 - When ready to publish, if updating published package.**

Increment version in `package.json` if you are updating the package.

```
npm run build
npm publish
```