# README

Build a documentation website using markdown.

You can see the slides of this repository at https://hogenttin.github.io/hogent-mkdocs/ . Play with it to see what it can do!

## Table of Contents

-   [Basic usage](#basic-usage)
    -   [Installation](#installation)
    -   [How do I use this?](#how-do-i-use-this)
    -   [Live preview](#live-preview)
-   [Configuration](#configuration)
    -   [Theme](#theme)
    -   [MkDocs options](#mkdocs-options)
    -   [MkDocs plugins](#mkdocs-plugins)
-   [Additional tools](#additional-tools)
    -   [Automatic deployment](#automatic-deployment)
    -   [Formatting](#formatting)
    -   [Linting](#linting)

## Basic usage

### Installation

1. Install [python](https://www.python.org/downloads/) .
2. (optional) Create a [python environment](https://docs.python.org/3/library/venv.html). E.g. for Linux:

    ```console
    python -m venv venv
    source ./venv/bin/activate
    ```

3. Install the dependencies:

    ```console
    pip install --requirement requirements.txt
    ```

### How do I use this?

Edit, add or delete your markdown files in the [docs](./docs/) directory, and run `mkdocs build` to generate the website in the [site](./site) folder. **That's all to get started!** :rocket:

If you want to edit the sidebar, then just edit the `nav` entry in [mkdocs.yml](./mkdocs.yml) .

### Live preview

MkDocs allows you to start up a live preview, so you can instantly see how your content looks like whilst editing the markdown files.

```console
mkdocs serve
```

## Configuration

:bulb: **You don't have to change these files or settings** if you want to keep things simple. In that case, just ignore this section.

### Theme

If you want another theme, you can change edit the `theme` entry in [mkdocs.yml](./mkdocs.yml). You can find a lot of themes at https://github.com/mkdocs/catalog#-theming .

### [MkDocs](https://www.mkdocs.org/) options

You can add them to [mkdocs.yml](./mkdocs.yml) .

### [MkDocs](https://www.mkdocs.org/) plugins

You can add additional functionality using [MkDocs plugins](https://github.com/mkdocs/catalog). These can be enabled by editing [mkdocs.yml](./mkdocs.yml) . E.g., the [Mermaid](https://github.com/fralau/mkdocs-mermaid2-plugin) plugin for drawing graphs is added in this repo as an example on how to do it.

## Additional tools

### Automatic deployment

This repo automatically builds the website and pushes them to https://hogenttin.github.io/hogent-mkdocs/ whenever a commit is pushed to the `main` branch. This is done using using [GitHub actions](https://docs.github.com/en/actions) . You can find the workflow in the [.github](./.github) folder.

### Formatting

An [editorconfig](https://editorconfig.org/) config has been added in [.editorconfig](./.editorconfig) .

A [prettier](https://prettier.io/docs/en/) config has been added in [.prettierrc.json5](./.prettierrc.json5) .

:warning: Use 4 spaces for indentation of nested lists. Otherwise the nesting may not work. This is consistent with the [original MarkDown](https://daringfireball.net/projects/markdown/syntax#list) and the [CommonMark](https://spec.commonmark.org/0.31.2/#lists) specs.

### Linting

A [markdownlint](https://github.com/DavidAnson/markdownlint) config has been added in [.markdownlint.jsonc](./.markdownlint.jsonc) .
