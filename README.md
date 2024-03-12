# README

## Demo

You can see the slides of this repository at https://hogenttin.github.io/hogent-mkdocs/ . Play with it to see what it can do!

## Installation

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

## Basic usage

Edit, add or delete your markdown files in the [docs](./docs/) directory.

### Creating slides (debugging)

You can start up a live preview:

```console
mkdocs serve
```

## Advanced

**You don't really need this** if you want to keep things simple, but it's here if you want an example.

### Automatic deployment

This repo automatically builds the website and pushes them to https://hogenttin.github.io/hogent-mkdocs/ whenever a commit is pushed to the `main` branch. This is done using using [GitHub actions](https://docs.github.com/en/actions) . You can find the workflow in the [.github](./.github) folder.

### Formatting

A [prettier](https://prettier.io/docs/en/) config has been added in [.prettierrc.json5](./.prettierrc.json5) .

### Linting

A [markdownlint](https://github.com/DavidAnson/markdownlint) config has been added in [.markdownlint.jsonc](./.markdownlint.jsonc) .

## Configuration

### Theme

If you want another theme, you can change edit the `extra_css` entry in [mkdocs.yml](./mkdocs.yml) to point to another CSS file. You can also use an existing link like https://hogenttin.github.io/hogent-mkdocs/docs/theme.css . Using this specific URL will always keep your theme up to date with the one on this repo.

### [MkDocs](https://www.mkdocs.org/) options

You can add them to [mkdocs.yml](./mkdocs.yml) .
