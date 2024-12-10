# armv7-prisma-engine

Building Prisma Engine for ARMv7

# Usage

1. Require `prisma >= 6.0.1`
1. Download engine files from the [release](https://github.com/boostchicken/armv7-prisma-engine) page
1. Update the environment variables for your projects

```shell
PRISMA_QUERY_ENGINE_BINARY=path/to/query-engine
PRISMA_QUERY_ENGINE_LIBRARY=path/to/libquery_engine.so.node
PRISMA_SCHEMA_ENGINE_BINARY=path/to/schema-engine
```

Test your environment variable: `npx prisma -v`

```log
prisma                  : 6.0.1
Architecture            : arm
Query Engine (Node-API) : libquery-engine e9771e62de70f79a5e1c604a2d7c8e2a0a874b48 (at libquery_engine.so.node, resolved by PRISMA_QUERY_ENGINE_LIBRARY)
Schema Engine           : schema-engine-cli e9771e62de70f79a5e1c604a2d7c8e2a0a874b48 (at schema-engine, resolved by PRISMA_SCHEMA_ENGINE_BINARY)
```

Learn more: https://www.prisma.io/docs/orm/more/under-the-hood/engines

# Reference

- https://github.com/prisma/prisma-engines
- https://github.com/ImBIOS/prisma-armv7-builds
