# typescript-scaffold
scaffolding nodejs app with typescript

## tsc
npm init -y
npm i -D typescript
npm i -D @types/node

npx tsc --init
touch src/index.ts
## tsconfig.json

* "target": "esnext",
* "sourceMap": true,
* "outDir": "./dist", 
* "rootDir": "./src",
* "removeComments": true,

## ts-node-dev
npm i -D ts-node-dev

pacjage.json
"scripts": {
    "prebuild": "rm -rf dist",
    "build": "tsc",
    "dev": "ts-node-dev --transpile-only --no-notify src"
},
