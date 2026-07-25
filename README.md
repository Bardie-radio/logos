# Logos

Portable **module-mesh protocol** libraries for Bardie (`Bardie.Logos.*`).

| Package | Role |
|---------|------|
| `Bardie.Logos.Contracts` | Versioned gRPC contracts (ModuleRegistry, AuthAdapter, SourceModule, BlobStorage, Library) |
| `Bardie.Logos.Channel` | mTLS, module manifest, host/participant dial helpers |
| `Bardie.Logos.Hosting` | ASP.NET Core bootstrap for module participants (ports, health, OTel) |

Kithara **kind** SDKs: [`kithara-logos-auth`](https://github.com/Bardie-radio/kithara-logos-auth) (`Bardie.Module.Auth`), [`kithara-logos-source`](https://github.com/Bardie-radio/kithara-logos-source) (`Bardie.Module.Source`).

```bash
dotnet build Logos.sln
```
