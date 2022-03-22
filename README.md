# ForEvolve.Conventions

![Pack and Deploy master to NuGet.org](https://github.com/ForEvolve/ForEvolve.Conventions/workflows/Pack%20and%20Deploy%20master%20to%20NuGet.org/badge.svg)
[![Nuget](https://img.shields.io/nuget/v/ForEvolve.Conventions.Templates)](https://www.nuget.org/packages/ForEvolve.Conventions.Templates)

This repo contains coding conventions that I use in multiple projects. To simplify my life, I packed them as `dotnet new` templates. The templates can be installed from the command-line, using NuGet.

Out of now I created:

-   `.editorconfig`
-   `.prettierrc`

## Usage

To install the templates, you must execute the following command, once (templates are installed globally).

```xml
dotnet new -i ForEvolve.Conventions.Templates
```

Then you can `dotnet new [templates name]` to generate the files. The available templates are:

```bash
dotnet new cheditorconfig
dotnet new chprettierrc
```

_Files are generated in the current directory._

# How to contribute?

If you would like to contribute to the project, first, thank you for your interest, and please read [Contributing to ForEvolve open source projects](https://github.com/ForEvolve/ForEvolve.Conventions/tree/master/CONTRIBUTING.md) for more information.

## Contributor Covenant Code of Conduct

Also, please read the [Contributor Covenant Code of Conduct](https://github.com/ForEvolve/ForEvolve.Conventions/tree/master/CODE_OF_CONDUCT.md) that applies to all ForEvolve repositories.
