# Copilot Instructions for HelloWorld C# Project

## Project Overview

This is a simple .NET 7.0 console application using the minimal hosting model and top-level statements. The project follows modern C# conventions with implicit usings and nullable reference types enabled.

## Architecture & Structure

- **Entry Point**: `Program.cs` - Uses top-level statements (no Main method required)
- **Project Type**: Console application targeting .NET 7.0
- **Solution Structure**: Single project solution (`helloworld.sln` + `helloworld.csproj`)
- **Build Outputs**: Compiled to `bin/Debug/net7.0/` with executable and dependencies

## Key Configuration Settings

### Project File (`helloworld.csproj`)
```xml
<ImplicitUsings>enable</ImplicitUsings>  <!-- Auto-imports common System namespaces -->
<Nullable>enable</Nullable>              <!-- Enables nullable reference types -->
```

### Global Usings (Auto-Generated)
The following namespaces are globally available without explicit `using` statements:
- `System`
- `System.Collections.Generic`
- `System.IO`
- `System.Linq`
- `System.Net.Http`
- `System.Threading`
- `System.Threading.Tasks`

## Development Workflows

### Building & Running
- **Build**: `dotnet build` or use VS Code build task
- **Run**: `dotnet run` from project root
- **Clean**: `dotnet clean` to remove build artifacts

### File Organization
- Source code directly in project root (simple single-file project)
- Build outputs in `bin/` and `obj/` directories (auto-generated)
- No separate source directories for this simple project

## Coding Conventions

### Modern C# Features in Use
- **Top-level statements**: No need for Program class or Main method in `Program.cs`
- **Implicit usings**: Common System namespaces imported automatically
- **Nullable reference types**: Enabled project-wide for better null safety
- **File-scoped namespaces**: Not used (simple console app doesn't need namespaces)

### Code Style
- Simple, direct console output using `Console.WriteLine()`
- No complex error handling needed for this basic application
- Follow standard C# naming conventions (PascalCase for public members)

## Dependencies & Integration

- **Target Framework**: .NET 7.0 (cross-platform: Windows, Linux, macOS)
- **No external NuGet packages**: Pure .NET BCL usage
- **No database or external services**: Self-contained console application

## Common Tasks

When modifying this project:
1. Keep `Program.cs` simple with top-level statements
2. Add any new files at project root level
3. Use global usings - avoid explicit `using` statements for common System namespaces
4. Enable nullable reference types for any new code
5. Test changes with `dotnet run` for immediate feedback