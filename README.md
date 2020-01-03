# ForEvolve.Conventions

This repo contains conventions like `.editorconfig` and `.prettierrc`, that can be installed as a NuGet Package.

## Install

In an `<ItemGroup>`, add the following `PackageReference` to your `.csproj`:

```xml
<PackageReference Include="ForEvolve.Conventions.CodeFormat" Version="[insert the version here]" GeneratePathProperty="true" />
```

## Known issues/limitation

- The `GeneratePathProperty="true"` is very important to copy the files, otherwise some variables are missing.
- If you install the package using standard tooling (`dotnet add package ForEvolve.Conventions.CodeFormat` or VS Package Manager), you may need to delete your `obj` directory after adding the `GeneratePathProperty` attribute. Otherwise the `.targets` gets stuck in a loop trying to copy the files from the older `PackageReference`.
- If you install the package from VS, you might need to reopen it so it takes the `.editorconfig` into account; sounds like a bug in VS.
- From VS Code, the files are copied twice, once at the project-level and once at the solution-level. I guess that `$(SolutionDir)` is not available at some point, leading to multiple execution context.
- The package must be installed in a project,

# How to contribute?

If you would like to contribute to the project, first, thank you for your interest, and please read [Contributing to ForEvolve open source projects](https://github.com/ForEvolve/ForEvolve.DependencyInjection/tree/master/CONTRIBUTING.md) for more information.

## Contributor Covenant Code of Conduct

Also, please read the [Contributor Covenant Code of Conduct](https://github.com/ForEvolve/ForEvolve.DependencyInjection/tree/master/CODE_OF_CONDUCT.md) that applies to all ForEvolve repositories.
