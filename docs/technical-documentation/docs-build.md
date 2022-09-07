# Introduction

This documentation is built using [MkDocs](http://www.mkdocs.org/), a static site generator that is geared towards building project documentation. The documentation is created in the [Markdown](http://en.wikipedia.org/wiki/Markdown) format, and it all resides in the [`docs`](https://github.com/Islandora/documentation/tree/main/docs) directory in the repository. The organization of the documentation is controlled by the [`mkdocs.yml`](https://github.com/Islandora/documentation/blob/main/mkdocs.yml) in the root of the repository.

!!! Tip "Video version available"
    Some of the material in this tutorial is presented in our video, [How to Build Documentation](https://youtu.be/YgSXicNow5w).


## Prerequisites

You will need to have `mkdocs` software installed locally, as well as a required plugin and the MkDocs _Material_ theme. Below we will show you how to install `mkdocs` using the Python language's `pip` tool. For more details on installing and using MkDocs visit the [MkDocs installation guide](https://www.mkdocs.org/#installation).

- Open a terminal window.

- Install `mkdocs`:

    Windows / Linux:

    `sudo -H pip install mkdocs`

    macOS:

    `pip3 install mkdocs`



- Install plugin to enable display of the last revision date:

     Windows / Linux:

     `sudo -H pip install mkdocs-git-revision-date-localized-plugin`

    macOS:

    `pip3 install mkdocs-git-revision-date-localized-plugin`



- Install Material theme:

    Windows / Linux:

    `sudo -H pip install mkdocs-material`

    macOS:

    `pip3 install mkdocs-material`



## Build and Deploy documentation

Make sure you have all the submodules:

`git submodule update --init --recursive`

Documentation is build by running to the following command in the root of the repository:

`mkdocs build --clean`

This command will create a static `site` folder in the root of the repository.

You can preview any changes you have made to the documentation by running the following command:

`mkdocs serve`

And then visiting http://localhost:8111 in your browser.

To deploy documentation to GitHub Pages, issue the following command:

`mkdocs gh-deploy --clean`

To stop the `mkdocs serve` command just type the key combination "Control-c".
