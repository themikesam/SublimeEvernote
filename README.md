Evernote for Sublime Text
=========================

This plugin was overhauled & upgraded by Emanuele D'Osualdo. View his [SublimeEvernote](https://github.com/bordaigorl/sublime-evernote) repo, or simply download the plugin from Sublime's package manager.

I'm keeping this repo alive only for historical/archival purposes.

---

[Sublime Text](http://www.sublimetext.com/3) plugin for [Evernote](http://www.evernote.com)

This package is based on [SublimeEvernote](https://github.com/jamiesun/SublimeEvernote).
It adds support for Sublime Text 3 (thanks to [timlockridge](https://github.com/timlockridge/SublimeEvernote)) and includes new features as open/update of notes from Sublime.

# Main Features

 * **Send a note to Evernote:** converts the markdown document in the current view into rich text and sends it to your Evernote. You will be able to choose a title, tags and the notebook where to store it.
 * **Open a note from Evernote**: shows panels to choose a note from a notebook, converts it to markdown and presents it in a view.
 * **Update note**: when editing the markdown of an opened note you can save it back to Evernote (again in rich text).
 * **Full two-way support for metadata**: just put a YAML-like header in your markdown file, and send/update to evernote commands will respect the info. The open command produces the header for imported notes. For example:
```yaml
---
title: Title
tags: list, of, tags
notebook: Notebook name
---
Contents
```
* **Inline css**: some tags can be styled (with inline style attributes). This required a small patch in `markdown2.py`.


# Installation

clone this repository with

```sh
$ git clone --recursive http://github.com/bordaigorl/sublime-evernote.git
```

in

* Windows: `%APPDATA%/Roaming/Sublime Text 3/Packages/`
* OSX: `~/Library/Application Support/Sublime Text 3/Packages/`
* Linux: `~/.Sublime Text 3/Packages/`
* Portable Installation: `Sublime Text 3/Data/`

# Usage

**Note: When you first run this package from the command palette, it will launch a browser window with your Evernote developer token. Copy the token and paste it into the prompt at the bottom of your Sublime window. Sublime will store the token data in `Sublime Text 3/Packages/User/SublimeEvernote.sublime-settings`**

`Command Palette` > `Evernote: Send to Evernote`
`Command Palette` > `Evernote: Open Evernote Note`
`Command Palette` > `Evernote: Update Evernote Note`
`Command Palette` > `Evernote: Reconfigure`

# Acknowledgements

 * Original Plugin: [jamiesun](https://github.com/jamiesun/SublimeEvernote)
 * Port to ST3:
     - [rekotan](https://github.com/rekotan/SublimeEvernote)
     - [timlockridge](https://github.com/timlockridge/SublimeEvernote)
 * Markdown2 converter: [trentm](https://github.com/trentm/python-markdown2/)
 * HTML2Markdown: [Aaron Swartz](https://github.com/aaronsw/html2text)
 * Evernote API: <https://github.com/evernote/evernote-sdk-python>
