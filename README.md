# Obsidian Tasks Custom Icons

This repository contains a commandline tool (for developers/designers) to easily create CSS snippets that when added to Obsidian will replace the emojis used by the [Obsidian Tasks](https://github.com/obsidian-tasks-group/obsidian-tasks) with monotone icons matching the text colour.

As a Tasks end-user, you can simply [install](https://help.obsidian.md/Extending+Obsidian/CSS+snippets) one of the CSS snippets in this repository to your obsidian vault to replace the [Tasks Emoji Format](https://publish.obsidian.md/tasks/Reference/Task+Formats/Tasks+Emoji+Format) emojis with monotone icons.

## Lucide-based Icon set

![Lucide-based icon theme screenshot](lucide/screenshot.png)

[Download CSS Snippet](https://raw.githubusercontent.com/replete/obsidian-tasks-custom-icons/main/lucide/obsidian-tasks-lucide-icons.css)

Date and recurring icons modified from https://lucide.dev


## Creating a custom icon set

**Prerequisites:** Node.JS must be installed. I cannot provide support if this is unfamiliar, but it is fairly straightforward:

- Clone/fork/download this repository
- From a terminal, run `npm install` from the cloned/forked/downloaded directory
- Duplicate the `lucide` icon set folder, renaming it to your new icon set name, e.g. `fancyicons`
- Replace/edit the duplicated SVG files in your new folder
- Run `npm run build`, to generate `obsidian-tasks-<icon folder name>-icons.css` and `demo.html` files within each icon set folder within the repository
    <small> _Dev Tip:_ Create a text file named `copysnippetpath.txt` within an icon set folder, containing an absolute path to another folder (e.g '`/Users/username/MyVault/.obsidian/snippets/`') to cause an extra copy of `obsidian-tasks-<icon folder name>-icons.css` to be written each time you run `npm run build`. Obsidian will reload this file whenever you update it if you enable the CSS snippet, allowing for in-situ preview of your custom icon set</small>
- Adjust SVG icons as desired

If license permits, consider opening a PR with your icon set, reproducing appropriate licenses within `LICENSE.TXT`.

## Support development
<a href="https://www.buymeacoffee.com/replete"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=replete&button_colour=BD5FFF&font_colour=ffffff&font_family=Poppins&outline_colour=000000&coffee_colour=FFDD00" /></a>