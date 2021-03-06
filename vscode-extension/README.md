# ilspy-vscode (powered by ICSharpCode.Decompiler)

Welcome to the ILSpy extension for Visual Studio Code! This extension provides two commands inside Visual Studio Code:

* `ilspy.decompileAssemblyPromptForFilePath` - Decompile an MSIL assembly from a user-input full path.
* `ilspy.decompileAssemblyInWorkspace` - Decompile a MSIL assembly inside of current Visual Studio Code workspace.

Open the Visual Studio Code Command Palette (<kbd>Ctrl+Shift+P</kbd>) then type `ilspy` to show the two commands.

The `Decompile IL Assembly in Current Workspace` will put all potential .NET assemblies
(files with extension `.dll`, `.exe`, `.winrt`, or `.netmodule`) in your
workspace in a list for selection.

For the `Decompile IL Assembly from a Given Path` command, when prompted, type the full path to a .NET assembly,
For example, `c:/temp/a.dll` or `/home/user/b.dll`.

If the file is a valid .NET assebmly, a tree view named `DECOMPILED MEMBERS` is added into the Explorer view.
It allows expanding and selecting various nodes, whose decompiled C# code is shown in the editor.

## Requirements

* Windows - no other pre-requisites
* Linux/MacOS - requires Mono version >= 4.6.0.

## What's New

First release of ILSpy .NET Decompiler extension for Visual Studio Code!

See our [change log](CHANGELOG.md) for all of the updates.

### Found a Bug?
Please file any issues at https://github.com/icsharpcode/ilspy-vscode/issues

## Development

First install:
* Node.js (newer than 4.3.1)
* Npm (newer than 2.14.12)

* Run `npm i`
* Run `npm run compile`
* Open in Visual Studio Code (`code .`)
* *Optional:* run `npm run watch`, make code changes
* Press <kbd>F5</kbd> to debug

To **test** do the following: `npm test` or <kbd>F5</kbd> in VS Code with the "Launch Tests" debug configuration.

## License

[MIT license](LICENSE.TXT).
