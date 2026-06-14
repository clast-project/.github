# clast-project

The goal of the project is to create a collection of high-performance C# libraries focused on data processing, storage, and analytics.

## Libraries

| Library | Description | Status |
|---------|-------------|--------|
| **[alp](https://github.com/clast-project/alp)** | Adaptive Lossless floating-Point compression | [Version 0.1.0](https://www.nuget.org/packages/Clast.Alp) |
| **[bloom-filter](https://github.com/clast-project/bloom-filter)** | Parquet-format Split Block Bloom Filter (SBBF) with a generic-key facade | [Version 0.1.0](https://www.nuget.org/packages/Clast.BloomFilter/) |
| **[database-decimal](https://github.com/clast-project/database-decimal)** | Decimal libraries compatible with the traditional "database" approach | [Version 0.1.1](https://www.nuget.org/packages/Clast.DatabaseDecimal) |
| **[fastlanes](https://github.com/clast-project/fastlanes)** | SIMD-friendly lightweight integer compression | [Version 0.1.1](https://www.nuget.org/packages/Clast.FastLanes) |
| **[fsst](https://github.com/clast-project/fsst)** | Fast Static Symbol Table string compression | [Version 0.1.3](https://www.nuget.org/packages/Clast.Fsst) |
| **[pcodec](https://github.com/clast-project/pcodec)** | Pco numeric compression format | [Version 0.1.1](https://www.nuget.org/packages/Clast.Pcodec) |

## Goals

- **Performance**: Leverage modern .NET features (SIMD, `Span<T>`, `Memory<T>`) for maximum throughput.
- **Correctness**: Fully tested against reference implementations and real-world datasets.
- **Interoperability**: Compatible with the broader data ecosystem where appropriate.
- **Simplicity**: Clean, idiomatic C# APIs that are easy to use and compose.

## Getting Started

Each library lives in its own repository under the [clast-project](https://github.com/clast-project) organization. Refer to each library's own README for installation and usage instructions.

## Forked Google Libraries

These are forks of existing Google .NET libraries, with Newtonsoft.Json replaced by source-generated System.Text.Json, made trimming/AOT-compatible, and a net10.0 target added (alongside netstandard2.0 and net8.0).

Why: to provide a Newtonsoft-free, AOT-ready build of the Google.Cloud.Storage.V1 dependency closure. Namespaces and public type names are unchanged — only the package id, assembly name, and strong-name key differ — so consumers recompile against the Clast.* packages rather than using them as binary drop-in replacements.

| Library | Replaces |
|---------|----------|
│ **[Clast.Google.Apis.Core](https://www.nuget.org/packages/Clast.Google.Apis.Core)** │ Google.Apis.Core │
│ **[Clast.Google.Apis](https://www.nuget.org/packages/Clast.Google.Apis)** │ Google.Apis │
│ **[Clast.Google.Apis.Auth](https://www.nuget.org/packages/Clast.Google.Apis.Auth)** │ Google.Apis.Auth │
│ **[Clast.Google.Apis.Storage.v1](https://www.nuget.org/packages/Clast.Google.Apis.Storage.v1)** │ Google.Apis.Storage.v1 │
│ **[Clast.Google.Apis.Bigquery.v2](https://www.nuget.org/packages/Clast.Google.Apis.Bigquery.v2)** │ Google.Apis.Bigquery.v2 │
│ **[Clast.Grpc.Auth](https://www.nuget.org/packages/Clast.Grpc.Auth)** │ Grpc.Auth │
│ **[Clast.Google.Api.Gax](https://www.nuget.org/packages/Clast.Google.Api.Gax)** │ Google.Api.Gax │
│ **[Clast.Google.Api.Gax.Rest](https://www.nuget.org/packages/Clast.Google.Api.Gax.Rest)** │ Google.Api.Gax.Rest │
│ **[Clast.Google.Api.Gax.Grpc](https://www.nuget.org/packages/Clast.Google.Api.Gax.Gprc)** │ Google.Api.Gax.Grpc │
│ **[Clast.Google.Cloud.Storage.V1](https://www.nuget.org/packages/Clast.Google.Cloud.Storage.V1)** │ Google.Cloud.Storage.V1 │
│ **[Clast.Google.Cloud.BigQuery.V2](https://www.nuget.org/packages/Clast.Google.Cloud.BigQuery.V2)** │ Google.Cloud.BigQuery.V2 │
│ **[Clast.Google.Cloud.BigQuery.Storage.V1](https://www.nuget.org/packages/Clast.Google.Cloud.BigQuery.Storage.V1)** │ Google.Cloud.BigQuery.Storage.V1 │

## Contributing

This is a bit of an experiment and I'm not currently accepting contributions.

## License

All libraries in this organization are released under the [Apache License, Version 2.0](LICENSE) unless otherwise noted.
