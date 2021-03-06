# Pip.WebUI Core Services http://github.com/pip-webui/pip-webui-core

Generic utilities and non-visual services to support client application development.

The module contains the following functionality:

* Functions (utilities, tags, dates, form errors)
* Translation
* Errors and transactions
* Routing
* Formatting
* Google analytics
* Timers
* Behaviors: Draggable, Focused, Selected, Infinite Scroll

In the version 1.0.0 the implementation was cleaned up and covered with unit tests.
Few functions were replaced with off-the-shelf libraries. Added support for sound play and google analytics. 

Quick Links:

* [Documentation](#documentation)
* [API Reference](http://htmlpreview.github.io/?https://github.com/pip-webui/pip-webui-core/blob/master/doc/api/index.html)
* [Contributing](#contributing)
* [Building](#building)
* [Installing](#installing)

## <a name="documentation"></a> Online Documentation

- Visit [documentation](doc/index.md) page
- Or build the project, launch and open samples; see [Building](#building) for details
   
## <a name="contributing"></a> Contributing

Developers interested in contributing should read the following guidelines:

- [Issue Guidelines](docs/guides/CONTRIBUTING.md#submit)
- [Contributing Guidelines](docs/guides/CONTRIBUTING.md)
- [Coding Guidelines](docs/guides/CODING.md)
- [ChangeLog](CHANGELOG.md)

> Please do **not** ask general questions in an issue. Issues are only to report bugs, request
  enhancements, or request new features. For general questions and discussions, use the
  [Pip Devs Forum](https://groups.google.com/forum/#!forum/pipdevs).

It is important to note that for each release, the [ChangeLog](CHANGELOG.md) is a resource that will
itemize all:

- Bug Fixes
- New Features
- Breaking Changes
   
## <a name="building"></a> Building

Developers can easily build the project using NPM and gulp.

* [Builds - Under the Hood](docs/guides/BUILD.md)

First install or update your local project's **npm** tools:

```bash
# First install all the NPM tools:
npm install

# Or update
npm update
```

Then run the **gulp** tasks:

```bash
# To clean '/build' and '/dist' directories
gulp clean

# To build distribution files in the `/dist` directory
gulp build

# To launch samples (build will open samples/index page in web browser)
gulp launch
```

For more details on how the build process works and additional commands (available for testing and
debugging) developers should read the [Build Instructions](docs/guides/BUILD.md).

## <a name="installing"></a> Installing Build (Distribution Files)

#### NPM

Core services have dependency on 3rd party libraries included into pip-webui-lib library.
Also the entire Pip WebUI framework is packaged into pip-webui library.

Change to your project's root directory.

```bash
# To install only core services with dependencies.
npm install git+ssh://git@github.com:pip-core/pip-webui-lib.git
npm install git+ssh://git@github.com:pip-core/pip-webui-core.git

# To install the entire pip-webui library
npm install git+ssh://git@github.com:pip-core/pip-webui.git
```
