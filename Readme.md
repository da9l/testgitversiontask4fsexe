# Test gitversiontask for F# exe projects

To test you need to set the `.../GitVersion/artifact/<exactversion>/nuget` as a source in your local nuget setup.
To do this you'll need

```powershell
choco install nuget.commandline
nuget source add -Name gvtrepo -Source <absolutePathToNugetFolderAbove>

```

Then you can modify the .fsproj and .csproj to include the right version.

## Known problems

As of 2019-11-06 AssemblyInfo generation from fsproj does not work in dotnet core. It does work in VS2019 (with dotnetcore sdk 3.0).
