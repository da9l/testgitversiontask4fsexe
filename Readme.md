# Test gitversiontask for F# exe projects

To test you need to set the `.../GitVersion/artifact/<exactversion>/nuget` as a source in your local nuget setup.
To do this you'll need

```powershell
choco install nuget.commandline
nuget source add -Name gvtrepo -Source <absolutePathToNugetFolderAbove>

```

Then you can modify the .fsproj and .csproj to include the right version.
