# PRAXO-CORE for C# / .NET

Dedicated repository for the C# implementation of PRAXO-CORE: an embeddable,
MIT-licensed agent execution kernel with policy controls, human-in-the-loop
approval, checkpoints, events, and tool calling.

- Package: `Praxo.Core` on NuGet
- Documentation: https://axisvela.github.io/praxo-core/languages/csharp/
- Canonical source: https://github.com/axisvela/praxo-core/tree/main/language/csharp
- Release index: https://axisvela.github.io/praxo-core/languages/registry-status/

This repository is a discovery mirror of the canonical C# source. The monorepo
remains the source of truth and the release workflow source. Shared conformance
vectors are included under `spec/`.

## Install

```sh
dotnet add package Praxo.Core --version 0.3.0
```

## Verify

From `language/csharp`:

```sh
dotnet build Praxo.Core/Praxo.Core.csproj
dotnet run --project Praxo.Conformance
dotnet run --project Praxo.Tests
```

PRAXO-CORE is not a hosted model, workflow engine, identity provider, or safety
controller. Do not infer exactly-once execution, complete sandbox isolation,
production security certification, live-provider behavior, or physical safety
from this package.

MIT licensed.
