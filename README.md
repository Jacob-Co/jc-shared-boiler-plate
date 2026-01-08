## To use shared
- create `tsconfig.base.json` in base folder, with content:
```
{
  "compilerOptions": {
    "baseUrl": ".",
    "paths": {
      "@shared/*": ["shared/src/*"]
    }
  }
}
```
- in each project that will use the `shared`:
```
{
  "extends": "../tsconfig.base.json"
}
```

