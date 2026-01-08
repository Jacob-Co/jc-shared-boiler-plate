## To use shared
- create a monorepo, with `package.json`:
```
{
  "private": true,
  "workspaces": [
    "receipts-reader-app", // sample frontend
    "receipts-server", // sample backend
    "receipts-shared" // this is the shared boiler plate
  ]
}
```
- to use shared in a given subfolder:
```
"dependencies": {
    "receipts-shared": "*" // name in shared package.json
},
```
- then in root use the `-w` command to build then run:
```
$ npm i
$ npm run build -w receipts-shared
$ npm run dev -w receipts-server

```
