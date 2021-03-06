# Avalonia Templates for `dotnet new`

For more information about `dotnet new` templates see [here](https://blogs.msdn.microsoft.com/dotnet/2017/04/02/how-to-create-your-own-templates-for-dotnet-new/).

## Installing the templates

Clone this repository and run:

```
dotnet new --install [path-to-repository]
```

The templates should now be available in `dotnet`:

```
Templates                   Short Name         Language        Tags
--------------------------------------------------------------------------
Console Application         console              [C#], F#      Common/Console
Class library               classlib             [C#], F#      Common/Library
Unit Test Project           mstest               [C#], F#      Test/MSTest
xUnit Test Project          xunit                [C#], F#      Test/xUnit
ASP.NET Core Empty          web                  [C#]          Web/Empty
ASP.NET Core Web App        mvc                  [C#], F#      Web/MVC
ASP.NET Core Web API        webapi               [C#]          Web/WebAPI
Avalonia .NET Core App      avalonia.app         [C#], F#      ui/xaml
Avalonia .NET Core MVVM App avalonia.mvvm        [C#], F#      ui/xaml
Avalonia UserControl        avalonia.usercontrol [C#], F#      ui/xaml
Avalonia Window             avalonia.window      [C#], F#      ui/xaml
Solution File               sln                                Solution
```

# Creating a new MVVM Application

MVVM is the recommended pattern for creating Avalonia C# applications, however you can use it in F# too. The MVVM application template
uses [ReactiveUI](https://reactiveui.net/) to ease building applications with complex interactions.

To create a new C# MVVM application called `MyApp` in its own subdirectory, run:

```
dotnet new avalonia.mvvm -o MyApp
```
And for F# run:
```
dotnet new avalonia.mvvm -o MyApp -lang F#
```

# Creating a new Application
To create a new barebones C# application called `MyApp` in its own subdirectory, run:

```
dotnet new avalonia.app -o MyApp
```

And for F# run:

```
dotnet new avalonia.app -o MyApp -lang F#
```

# Creating a new Window

To create a new application called `MyNewWindow`, in the namespace `MyApp` run:

C#:
```
dotnet new avalonia.window -na MyApp -n MyNewWindow
```

F#:
```
dotnet new avalonia.window -na MyApp -n MyNewWindow -lang F#
```

# Creating a new UserControl

To create a new `UserControl` called `MyNewView`, in the namespace `MyApp` run:

C#:
```
dotnet new avalonia.window -na MyApp -n MyNewView
```

F#:
```
dotnet new avalonia.window -na MyApp -n MyNewView -lang F#
```
