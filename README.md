Prefer
======
Simple wrapper around the [`defaults`] command to easily configure [preferences] across macOS with a
`pref`[`erence`]`s/*.`[`y`\[`a`\]`ml`][YAML] or [`.json`][JSON] file located in the current directory, else globally in [`$XDG_CONFIG_HOME`]`/pref`[`erence`]`s/*.y`[`a`]`ml` or `~/.pref`[`erence`]`s/*.y`[`a`]`ml`.

Useful with [.files].

[CLI]
-----
`docket `[`--dump`]` ~/.dock.yml`

Options
---------------------------------------------------------------------------------------------------------------------------------------------
| Option         | Description                                                                                                              |
|:---------------|:-------------------------------------------------------------------------------------------------------------------------|
| `-`[`-h`]`elp` | Display brief usage information.                                                                                         |
| `-`[`-d`]`ump` | Display your current Dock configuration in [YAML] (or `--json`) format. Optionally specify a config file to save output. |
| `-`[`-j`]`son` | Force [JSON] over YAML format.                                                                                           |

Install
-------
~~~ sh
brew tap danielbayley/prefer https://github.com/danielbayley/docket
brew install prefer
~~~
or with [`brew bundle`] using a _[Brewfile]_:
~~~ rb
# Brewfile
repo = "danielbayley/prefer"
tap repo, "https://github.com/#{repo}"
brew "prefer"
~~~

License
-------
[MIT] © [Daniel Bayley]

[MIT]:                LICENSE.md
[Daniel Bayley]:      https://github.com/danielbayley

[`defaults`]:         https://
[preferences]:        https://support.apple.com/guide/mac-help/mh35859/mac

[YAML]:               https://yaml.org
[JSON]:               https://json.org

[homebrew]:           https://brew.sh
[`brew bundle`]:      https://docs.brew.sh/Manpage#bundle-subcommand
[brewfile]:           https://github.com/Homebrew/homebrew-bundle#usage

[.files]:             https://github.com/danielbayley/homebrew-dotfiles
[`$XDG_CONFIG_HOME`]: https://wiki.archlinux.org/title/XDG_Base_Directory#Specification

[cli]:                man.md
