# sflow-proto

CE Protobuf definitions for SFLOW workflow engine (Apache 2.0).

Mirrored to GitHub on release tags. EE protos are in a separate repo (`sflow-proto-ee`).

## Structure

- `sflow/v1/` — CE API definitions

## Code Generation

```bash
buf generate
```

Generates:
- Rust (tonic) → `gen/rust/`
- TypeScript (protobuf-ts) → `gen/ts/`
