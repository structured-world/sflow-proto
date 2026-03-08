# sflow-proto

Protobuf definitions for SFLOW workflow engine.

## Structure

- `sflow/v1/` — CE API definitions (mirrored to GitHub under Apache 2.0)
- `sflow/ee/v1/` — EE API definitions (private, never public)

## Code Generation

```bash
buf generate
```

Generates:
- Rust (tonic) → `gen/rust/`
- TypeScript (protobuf-ts) → `gen/ts/`
