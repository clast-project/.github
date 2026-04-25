# Contributing to clast-project

Thank you for your interest in contributing! This document describes how to contribute to any library in the **clast-project** organization.

## Code of Conduct

By participating in this project, you agree to abide by our [Code of Conduct](CODE_OF_CONDUCT.md).

## How to Contribute

### Reporting Bugs

Before opening a bug report, please search the existing issues to avoid duplicates. When filing a new bug, use the **Bug Report** issue template and include:

- A clear, descriptive title.
- Steps to reproduce the problem.
- The expected behavior and what actually happened.
- Your .NET SDK version and operating system.
- A minimal code sample or test case that demonstrates the issue.

### Suggesting Features

Feature requests are welcome! Use the **Feature Request** issue template and describe:

- The problem you are trying to solve.
- The proposed solution and any alternatives you considered.
- Whether you are willing to implement it yourself.

### Submitting Pull Requests

1. **Fork** the repository and create a branch from `main` with a descriptive name (e.g. `feature/alp-encoding`, `fix/parquet-null-handling`).
2. **Write tests** for all new functionality. We require tests to pass before merging.
3. **Follow the coding style** of the existing codebase (see [Coding Style](#coding-style) below).
4. **Run the tests** locally before opening a pull request:
   ```bash
   dotnet test
   ```
5. **Fill out the pull request template** completely.
6. **Link any related issues** using [closing keywords](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue) (e.g. `Closes #42`).

A maintainer will review your pull request as soon as possible. We may request changes before merging.

## Coding Style

- Follow the [Microsoft C# Coding Conventions](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions).
- Use `var` where the type is obvious; prefer explicit types for clarity in complex expressions.
- Prefer `Span<T>` and `Memory<T>` over arrays in performance-critical paths.
- Use XML doc comments (`///`) on all public APIs.
- Keep lines under 120 characters.
- Use [nullable reference types](https://learn.microsoft.com/en-us/dotnet/csharp/nullable-references) (`<Nullable>enable</Nullable>`).

## Project Setup

Requirements:

- [.NET 8 SDK](https://dotnet.microsoft.com/download) or later
- A C# IDE such as [Visual Studio](https://visualstudio.microsoft.com/), [Rider](https://www.jetbrains.com/rider/), or [VS Code](https://code.visualstudio.com/) with the C# extension

Build a project:

```bash
dotnet build
```

Run tests:

```bash
dotnet test
```

Run benchmarks (where available):

```bash
dotnet run -c Release --project benchmarks/<ProjectName>.Benchmarks
```

## Versioning

This project follows [Semantic Versioning](https://semver.org/). Breaking changes are only introduced in major version bumps.

## Licensing

By contributing, you agree that your contributions will be licensed under the same [MIT License](https://opensource.org/licenses/MIT) that covers the project.
