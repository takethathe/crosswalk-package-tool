Crosswalk-package-tool
===================

Build the Crosswalk binary deb package.

### Preparation

Debian testing is the only tested platform. Node.js, the debuild tool,
the Crosswalk runtime, and git must be functional.

1. Download Crosswalk app tools: `git clone https://github.com/crosswalk-project/crosswalk-package-tool.git`
2. Initialize the Crosswalk app tools: `cd crosswalk-package-tool`, then `npm install`
3. The main script is `crosswalk-package-tool/bin/crosswalk-package`. Set environment PATH or invoke with directory.

### Usage

`crosswalk-package create 1`: This will setup the package generating
envrionment under 'deb_package' directory. Please make sure run this
command under Crosswalk directory. Please note that the last parameter
means the 'debian version', a number like 1, 2, 3...

`crosswalk-package build`: Build the crosswalk deb binary, it will be
generated under 'deb_package'

That's all for now. More to come soon, and if all goes well, NPMs for new years.
