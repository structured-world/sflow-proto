# sflow-proto

Protobuf definitions of the public SFLOW gRPC API: the workflow, admin, block
and inspection services and their shared types. The SFLOW server
([structured-world/sflow](https://github.com/structured-world/sflow)) and its
clients are generated from these files.

## Structure

- `sflow/v1/`: API definitions, package `sflow.v1`

## Checks

```bash
buf lint
buf format --diff --exit-code
buf breaking --against '.git#branch=origin/main'
```

## Code generation

```bash
buf generate
```

Generates Rust (prost + tonic) into `gen/rust/` and TypeScript (protobuf-ts)
into `gen/ts/`; the plugins are expected on `PATH`.

## License

Apache-2.0, see [LICENSE](LICENSE).

Contributions are accepted under the [Structured World Contributor License Agreement](https://sw.foundation/cla); see [CONTRIBUTING.md](CONTRIBUTING.md).
