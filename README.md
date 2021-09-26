# Extensions Sync

[![ts](https://badgen.net/badge/icon/typescript?icon=typescript&label)](#)
[![deps](https://img.shields.io/david/oae/gnome-shell-extensions-sync)](#)
[![opensource](https://badges.frapsoft.com/os/v1/open-source.png?v=103)](#)
[![licence](https://badges.frapsoft.com/os/gpl/gpl.png?v=103)](https://github.com/oae/gnome-shell-extensions-sync/blob/master/LICENSE)
[![latest](https://img.shields.io/github/v/release/oae/gnome-shell-extensions-sync)](https://github.com/oae/gnome-shell-extensions-sync/releases/latest)
[![compare](https://img.shields.io/github/commits-since/oae/gnome-shell-extensions-sync/latest/master)](https://github.com/oae/gnome-shell-extensions-sync/compare)

Syncs gnome shell keybindings, tweaks settings and extensions with their configuration across all gnome installations

<p align="center">
  <img src="https://i.imgur.com/gmSkdbT.png" />
  <img src="https://i.imgur.com/zSZM3Cg.png" />
</p>

## Installation

### From [Git](https://github.com/oae/gnome-shell-extensions-sync)

```bash
git clone https://github.com/oae/gnome-shell-extensions-sync.git
cd ./gnome-shell-extensions-sync
yarn install
yarn build
ln -s "$PWD/dist" "$HOME/.local/share/gnome-shell/extensions/extensions-sync@elhan.io"
```

### From [Ego](https://extensions.gnome.org)

You can install it from [**here**](https://extensions.gnome.org/extension/1486/extensions-sync/)
  

## Usage

- You can select the data types that are going to be saved in the settings.

## For Github

1. Create a new gist from [here](https://gist.github.com/) I suggest you make it secret.
2. Create a new token from [here](https://github.com/settings/tokens/new). Only gist permission is needed since we edit the gists.
3. Open extension settings, select the `Github` provider and fill gist id from first step and user token from second step.

## For Gitlab

1. Create a new snippet from [here](https://gitlab.com/-/snippets/new) I suggest you make it private.
2. Create a new token from [here](https://gitlab.com/-/profile/personal_access_tokens). Only api scope is needed.
3. Open extension settings, select the `Gitlab` provider and fill snippet id from first step and user token from second step.

## For Local

1. Select a file that has read/write permission by your active user. (default backup file is in `~/.config/extensions-sync.json`)

## Development

- This extension is written in Typescript and uses rollup to compile it into javascript.
- To start development, you need nodejs installed on your system;

  - Clone the project

    ```sh
    git clone https://github.com/oae/gnome-shell-extensions-sync.git
    cd ./gnome-shell-extensions-sync
    ```

  - Install dependencies and build it

    ```sh
    yarn install
    yarn build
    ln -s "$PWD/dist" "$HOME/.local/share/gnome-shell/extensions/extensions-sync@elhan.io"
    ```

  - During development you can use `yarn watch` command to keep generated code up-to-date.
