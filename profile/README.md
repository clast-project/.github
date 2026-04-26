# clast-project

The goal of the project is to create a collection of high-performance C# libraries focused on data processing, storage, and analytics.

## Libraries

| Library | Description | Status |
|---------|-------------|--------|
| **[fsst](https://github.com/clast-project/fsst)** | Fast Static Symbol Table string compression | [Version 0.1.0](https://www.nuget.org/packages/Clast.Fsst) |
| **[alp](https://github.com/clast-project/alp)** | Adaptive Lossless floating-Point compression | [Version 0.1.0](https://www.nuget.org/packages/Clast.Alp) |
| **[fastlanes](https://github.com/clast-project/fastlanes)** | SIMD-friendly lightweight integer compression | [Version 0.1.0](https://www.nuget.org/packages/Clast.FastLanes) |
| **database-decimal** | Decimal libraries compatible with the traditional "database" approach | Preliminary implementation |

## Goals

- **Performance**: Leverage modern .NET features (SIMD, `Span<T>`, `Memory<T>`) for maximum throughput.
- **Correctness**: Fully tested against reference implementations and real-world datasets.
- **Interoperability**: Compatible with the broader data ecosystem where appropriate.
- **Simplicity**: Clean, idiomatic C# APIs that are easy to use and compose.

## Getting Started

Each library lives in its own repository under the [clast-project](https://github.com/clast-project) organization. Refer to each library's own README for installation and usage instructions.

## Contributing

This is a bit of an experiment and I'm not currently accepting contributions.

## License

All libraries in this organization are released under the [Apache License, Version 2.0](LICENSE) unless otherwise noted.
