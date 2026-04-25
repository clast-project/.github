# clast-project

A collection of high-performance C# libraries focused on data processing, storage, and analytics.

## Libraries

| Library | Description | Status |
|---------|-------------|--------|
| **Parquet** | Read and write Apache Parquet files | Planned |
| **FSST** | Fast Static Symbol Table string compression | Planned |
| **ALP** | Adaptive Lossless floating-Point compression | Planned |
| **FastLanes** | SIMD-friendly lightweight integer compression | Planned |
| **DataSketches** | Probabilistic data structures (HLL, quantiles, theta sketches) | Planned |
| **Tables** | In-memory columnar table support | Planned |

## Goals

- **Performance**: Leverage modern .NET features (SIMD, `Span<T>`, `Memory<T>`) for maximum throughput.
- **Correctness**: Fully tested against reference implementations and real-world datasets.
- **Interoperability**: Compatible with the broader Apache Arrow / Parquet ecosystem.
- **Simplicity**: Clean, idiomatic C# APIs that are easy to use and compose.

## Getting Started

Each library lives in its own repository under the [clast-project](https://github.com/clast-project) organization. Refer to each library's own README for installation and usage instructions.

## Contributing

We welcome contributions! Please read our [Contributing Guidelines](CONTRIBUTING.md) and [Code of Conduct](CODE_OF_CONDUCT.md) before opening issues or pull requests.

## License

All libraries in this organization are released under the [MIT License](https://opensource.org/licenses/MIT) unless otherwise noted.
