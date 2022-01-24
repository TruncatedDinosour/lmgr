# LMGR

> Manage, switch and template licenses

# Dependencies

- coreutils for stuff like `head`, `awk`, ...
- fzf (optional) for `-pick-license`, `-p` flags
- git (optional) for generating info in default config automatically
- ncurses (optional) for colours (`LMGR_COLOURS=1`) using `tput`

# Installation

## Linux

- Gentoo Linux
  - [app-misc/lmgr::dinolay](https://ari-web.xyz/gentooatom/app-misc/lmgr)

## Manual

- Linux

```bash
git clone https://github.com/TruncatedDinosour/lmgr && cd lmgr

chmod a+rx lmgr

sudo install -Dm755 lmgr /usr/local/bin
```

# Configuration

Configuration can be found in `~/.config/license.conf`, it is automatically
generated on first launch

- **AUTHOR_NAME** -- Your full name
- **AUTHOR_EMAIL** -- Your email
- **AUTHOR_WEBSITE** -- Your website
- (optional) **TEMPLATE_DIR** -- Where are your license templates stored (default: `~/.config/licenses/`)

Example config:

```sh
#!/usr/bin/env sh

export AUTHOR_NAME='Joe Doe'
export AUTHOR_EMAIL='joe@doe.com'
export AUTHOR_WEBSITE='https://joe.doe/'
export TEMPLATE_DIR='/usr/share/lmgr'
```
