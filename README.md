# Brunch Task Runner extension
Adds support for the [Brunch](http://brunch.io/)
build tool in Visual Studio 2015's Task Runner Explorer.

[![Build status](https://ci.appveyor.com/api/projects/status/3x24c3gbyv2g34l8?svg=true)](https://ci.appveyor.com/project/madskristensen/brunchtaskrunner)

Download the extension at the
[VS Gallery](https://visualstudiogallery.msdn.microsoft.com/de706ad0-8a73-4df3-bef5-867bb9a70d51)
or get the
[nightly build](http://vsixgallery.com/extension/b4a4ad37-5a4b-4dfd-85fd-595cab6a26a9/)

## Install Brunch
In order to use this extension, you must have
[Brunch](http://brunch.io/) installed globally or locally
in your project.

Use [npm](http://npmjs.org/) to install it globally by
typing the following in a command line:

>npm install brunch -g

## Config files
The Brunch Task Runner automatically triggers when it finds
Brunch configuration files. These file names are supported:

1. config.coffee
2. brunch-config.coffee
3. brunch-config.js

Any config file will have a Brunch logo watermark at
the bottom right corner of the editor window.

![Watermark](art/watermark.png)

You can toggle the visibility of the watermark by clicking
on it.

## Task Runner Explorer
Open Task Runner Explorer by right-clicking the Brunch
configuration file and select **Task Runner Explorer** from
the context menu:

![Open Task Runner Explorer](art/open-trx.png)

Task Runner Explorer will show both _build_ and _watch_
tasks as well as any _override files_ present in the working
directory.

In this case, there are two *override files*:

1. config.overrides.**staging**
1. config.overrides.**test**

![Task List](art/task-list.png)

Each task can be executed by double-clicking the task.

![Console output](art/console.png)

### Debugging
By clicking the _Debug_ icon on the left menu bar, the
**--debug** switch is being enabled for all Brunch tasks.

![Debug](art/debug.png)

The _Debug_ menu icon is a toggle button that can be left
on or off for as long as needed.

### Bindings
Task bindings make it possible to associate individual tasks
with Visual Studio events such as _Project Open_ etc.

![Bindings](art/bindings.png)

## Item Template
You can easily add a new **brunch-config.coffee** file to
your project from the _Add New Item_ dialog.

Just search for "brunch".

![Item template](art/item-template.png)

## Contribute
Check out the [contribution guidelines](.github/CONTRIBUTING.md)
if you want to contribute to this project.

For cloning and building this project yourself, make sure 
to install the
[Extensibility Tools 2015](https://visualstudiogallery.msdn.microsoft.com/ab39a092-1343-46e2-b0f1-6a3f91155aa6)
extension for Visual Studio which enables some features
used by this project.

## License
[Apache 2.0](LICENSE) 