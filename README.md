# codingame-utils
## Jox.MergeCSharpFiles
With this NuGet package installed, building a C# project will also generate a single file containing all project's source code.

This can be used to write programs for [CodinGame](https://www.codingame.com/) consisting of multiple source files, and syncing the generated file to the CodinGame IDE using [codingame-sync](https://www.codingame.com/forum/t/codingame-sync-beta).

By default, the merged file will be written to `obj\Merged.cs`. As of version 0.6, this can be customized by setting the MSBuild property `MergedCSharpFile` in your `.csproj` file, for example:

```
<PropertyGroup>
  <MergedCSharpFile>C:\Temp\CodinGame-sync.cs</MergedCSharpFile>
</PropertyGroup>
```
