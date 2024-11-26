# README

Build a documentation website using markdown.

You can see the slides of this repository at https://hogenttin.github.io/hogent-mkdocs/ . Play with it to see what it can do!

## Basic usage

### Installation

1. Install [python](https://www.python.org/downloads/) .
2. (optional) Create a [python environment](https://docs.python.org/3/library/venv.html). E.g. for Linux:

   ```bash
   python -m venv venv
   source ./venv/bin/activate
   ```

3. Install the dependencies:

   ```bash
   pip install --requirement requirements.txt
   ```

### How do I use this?

Edit, add or delete your markdown files in the [docs](./docs/) directory, and run `mkdocs build` to generate the website in the [site](./site) folder. **That's all to get started!** :rocket:

If you want to edit the sidebar, then just edit the `nav` entry in [mkdocs.yml](./mkdocs.yml) .

### Live preview

MkDocs allows you to start up a live preview, so you can instantly see how your content looks like whilst editing the markdown files.

```bash
mkdocs serve
```

---

<details>

<summary>Configuration</summary>

## Configuration

:bulb: **You don't have to change these files or settings** if you want to keep things simple. In that case, just ignore this section.

### Theme

If you want another theme, you can change edit the `theme` entry in [mkdocs.yml](./mkdocs.yml). You can find a lot of themes at https://github.com/mkdocs/catalog#-theming .

### [MkDocs](https://www.mkdocs.org/) options

You can add them to [mkdocs.yml](./mkdocs.yml) .

### [MkDocs](https://www.mkdocs.org/) plugins

You can add additional functionality using [MkDocs plugins](https://github.com/mkdocs/catalog). These can be enabled by editing [mkdocs.yml](./mkdocs.yml) . E.g., the [mkdocs-git-revision-date-localized-plugin](https://github.com/timvink/mkdocs-git-revision-date-localized-plugin) plugin for showing the timestamp of the last edit is added in this repo as an example on how to do it.

</details>

---

<details>

<summary>Additional tools</summary>

## Additional tools

:bulb: **You don't need this** if you want to keep things simple. In that case, just ignore this section. Otherwise, it's here if you want an example.

### Automatic deployment

This repo automatically builds the website and pushes them to https://hogenttin.github.io/hogent-mkdocs/ whenever a commit is pushed to the `main` branch. This is done using using [GitHub actions](https://docs.github.com/en/actions) . You can find the workflow in the [.github](./.github) folder.

</details>
