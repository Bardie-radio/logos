# Bardie.Logos.Contracts

Versioned **gRPC contract package** for Bardie module authors. Single source of truth for Module Registry join, Auth Adapter / Source Module work RPCs, and Kithara-hosted BlobStorage / Library services.

**Package id:** `Bardie.Logos.Contracts` · **Version:** `0.1.0` · **TFM:** `net10.0`

| Proto | Namespace | Docs |
|-------|-----------|------|
| `Protos/module_registry.proto` | `Bardie.Modules.V1` | [grpc-module-registry](https://github.com/Bardie-radio/kithara/blob/main/docs/architecture/interfaces/grpc-module-registry.md) |
| `Protos/auth_adapter.proto` | `Bardie.Auth.V1` | [grpc-auth-adapter](https://github.com/Bardie-radio/kithara/blob/main/docs/architecture/interfaces/grpc-auth-adapter.md) |
| `Protos/source_module.proto` | `Bardie.Source.V1` | [grpc-source-module](https://github.com/Bardie-radio/kithara/blob/main/docs/architecture/interfaces/grpc-source-module.md) |
| `Protos/blob_storage.proto` | `Bardie.Storage.V1` | [grpc-blob-storage](https://github.com/Bardie-radio/kithara/blob/main/docs/architecture/interfaces/grpc-blob-storage.md) |
| `Protos/library.proto` | `Bardie.Library.V1` | [grpc-library](https://github.com/Bardie-radio/kithara/blob/main/docs/architecture/interfaces/grpc-library.md) |

C# stubs are generated with `GrpcServices=Both` (client + server). `.proto` files are also packed under `protos/` for non-C# generators.

**Blob key layout:** `tunes/<source_slug>/…` under the storage driver root (see blob-storage docs).

## Consume

`PackageReference` to nuget.org `Bardie.Logos.Contracts` (pin version in `Directory.Packages.props`).

```xml
<PackageReference Include="Bardie.Logos.Contracts" />
```

`.proto` files are packed under `protos/` for non-C# generators. Do not copy protos into consumer repos.
