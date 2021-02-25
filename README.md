# Express TypeSript Native Example for MetaCall FaaS

This example shows how to deploy a TypeScript server into [MetaCall.io](https://dashboard.metacall.io).

This project does not require transpilation, instead, MetaCall loads directly the TypeScript files. The transpilation is done at load time.

The `package.json` points to the `src/index.ts`:
```json
{
  "language_id": "ts",
  "path": ".",
  "scripts": ["src/index.ts"]
}
```

This server is launched by TypeScript Loader. If you want an example to transpile TypeScript files in order to load them later on with Node Loader check out the [Express TypeScript Example](https://github.com/metacall/express-typescript-example.git).
