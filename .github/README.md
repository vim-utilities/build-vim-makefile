# Init Makefile
[heading__top]:
  #build-vim-makefile
  "&#x2B06; Copies, and customizes, Makefile script to target path"


Copies, and customizes, Makefile script to target path


## [![Byte size of Init Makefile][badge__main__build_vim_makefile__source_code]][build_vim_makefile__main__source_code] [![Open Issues][badge__issues__build_vim_makefile]][issues__build_vim_makefile] [![Open Pull Requests][badge__pull_requests__build_vim_makefile]][pull_requests__build_vim_makefile] [![Latest commits][badge__commits__build_vim_makefile__main]][commits__build_vim_makefile__main]  [![Build Status][badge_travis_ci]][build_travis_ci]


---


- [:arrow_up: Top of Document][heading__top]

- [:building_construction: Requirements][heading__requirements]

- [:zap: Quick Start][heading__quick_start]

  - [:floppy_disk: Clone][heading__clone]
  - [:heavy_plus_sign: Install][heading__install]
  - [:fire: Uninstall][heading__uninstall]
  - [:arrow_up: Upgrade][heading__upgrade]
  - [:bookmark_tabs: Documentation][heading__documentation]

- [&#x1F9F0; Usage][heading__usage]

- [&#x1F5D2; Notes][heading__notes]

- [:chart_with_upwards_trend: Contributing][heading__contributing]

  - [:trident: Forking][heading__forking]
  - [:currency_exchange: Sponsor][heading__sponsor]

- [:card_index: Attribution][heading__attribution]

- [:balance_scale: Licensing][heading__license]


---



## Requirements
[heading__requirements]:
  #requirements
  "&#x1F3D7; Prerequisites and/or dependencies that this project needs to function properly"


This repository makes use of Git Submodules to track dependencies, to avoid incomplete downloads clone with the `--recurse-submodules` option...


```Bash
git clone --recurse-submodules git@github.com:vim-utilities/build-vim-makefile.git
```


To update tracked Git Submodules issue the following commands...


```Bash
git pull

git submodule update --init --merge --recursive
```


To force upgrade of Git Submodules...


```Bash
git submodule update --init --merge --recursive --remote
```


> Note, forcing and update of Git Submodule tracked dependencies may cause instabilities and/or merge conflicts; if however everything operates as expected after an update please consider submitting a Pull Request.


______


## Quick Start
[heading__quick_start]:
  #quick-start
  "&#9889; Perhaps as easy as one, 2.0,..."


> Perhaps as easy as one, 2.0,...


---


### Clone
[heading__clone]:
  #clone
  "&#x1f4be;"


Clone this project...


```Bash
mkdir -vp ~/git/hub/vim-utilities

cd ~/git/hub/vim-utilities

git clone git@github.com:vim-utilities/build-vim-makefile.git
```


---


### Install
[heading__install]:
  #install
  "&#x2795;"


Install via `make install` command...


```Bash
cd ~/git/hub/vim-utilities/build-vim-makefile

make install
```


---


### Uninstall
[heading__uninstall]:
  #uninstall
  "&#x1f525;"


Uninstalled via `make uninstall` target...


```Bash
cd ~/git/hub/vim-utilities/build-vim-makefile

make uninstall
```


... Which will remove script, tab-completion, and documentation symbolic links.


---


### Upgrade
[heading__upgrade]:
  #upgrade
  "&#x2b06;"


To update in the future use `make upgrade` command...


```Bash
cd ~/git/hub/vim-utilities/build-vim-makefile

make upgrade
```


---


### Documentation
[heading__documentation]:
  #documentation
  "&#x1F4D1;"


After installation, documentation may be accessed via Vim's `man` command, eg...


```Vim
man build-vim-makefile
```



______


## Usage
[heading__usage]:
  #usage
  "&#x1F9F0; How to utilize this repository"


Make a directory for Vim new plugin project...


```Bash
mkdir -p ~/git/hub/vim-utilities/project-name
```


Run `build-vim-makefile` script for new project...


```Bash
build-vim-makefile --path ~/git/hub/vim-utilities/project-name\
                   --author "S0AndS0"\
                   --version "0.0.1"
```


______


## Notes
[heading__notes]:
  #notes
  "&#x1F5D2; Additional things to keep in mind when developing"


To print available command-line options, along with currently set values, use the `--help` or `-h` flag...


```Bash
build-vim-makefile --path ~/git/hub/vim-utilities/project-name\
                   --author "S0AndS0"\
                   --version "0.0.1"\
                   --help
```


This repository may not be feature complete and/or fully functional, Pull Requests that add features or fix bugs are certainly welcomed.


______


## Contributing
[heading__contributing]:
  #contributing
  "&#x1F4C8; Options for contributing to build-vim-makefile and vim-utilities"


Options for contributing to build-vim-makefile and vim-utilities


---


### Forking
[heading__forking]:
  #forking
  "&#x1F531; Tips for forking build-vim-makefile"


Start making a [Fork][build_vim_makefile__fork_it] of this repository to an account that you have write permissions for.


- Add remote for fork URL. The URL syntax is _`git@github.com:<NAME>/<REPO>.git`_...


```Bash
cd ~/git/hub/vim-utilities/build-vim-makefile

git remote add fork git@github.com:<NAME>/build-vim-makefile.git
```


- Commit your changes and push to your fork, eg. to fix an issue...


```Bash
cd ~/git/hub/vim-utilities/build-vim-makefile


git commit -F- <<'EOF'
:bug: Fixes #42 Issue


**Edits**


- `<SCRIPT-NAME>` script, fixes some bug reported in issue
EOF


git push fork main
```


> Note, the `-u` option may be used to set `fork` as the default remote, eg. _`git push fork main`_ however, this will also default the `fork` remote for pulling from too! Meaning that pulling updates from `origin` must be done explicitly, eg. _`git pull origin main`_


- Then on GitHub submit a Pull Request through the Web-UI, the URL syntax is _`https://github.com/<NAME>/<REPO>/pull/new/<BRANCH>`_


> Note; to decrease the chances of your Pull Request needing modifications before being accepted, please check the [dot-github](https://github.com/vim-utilities/.github) repository for detailed contributing guidelines.


---


### Sponsor
  [heading__sponsor]:
  #sponsor
  "&#x1F4B1; Methods for financially supporting vim-utilities that maintains build-vim-makefile"


Thanks for even considering it!


Via Liberapay you may [![sponsor__shields_io__liberapay]][sponsor__link__liberapay] on a repeating basis.


Regardless of if you're able to financially support projects such as build-vim-makefile that vim-utilities maintains, please consider sharing projects that are useful with others, because one of the goals of maintaining Open Source repositories is to provide value to the community.


______


## Attribution
[heading__attribution]:
  #attribution
  "&#x1F4C7; Resources that where helpful in building this project so far."


- [GitHub -- `github-utilities/make-readme`](https://github.com/github-utilities/make-readme)

- [StackOverflow -- How do I check if file exists in Makefile so I can delete it](https://stackoverflow.com/questions/5553352/)

- [StackOverflow -- How to have config option in Makefile](https://stackoverflow.com/questions/58378555/)


______


## License
[heading__license]:
  #license
  "&#x2696; Legal side of Open Source"


```
Copies, and customizes, Makefile script to target path
Copyright (C) 2020 S0AndS0

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as published
by the Free Software Foundation, version 3 of the License.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.
```


For further details review full length version of [AGPL-3.0][branch__current__license] License.



[branch__current__license]:
  /LICENSE
  "&#x2696; Full length version of AGPL-3.0 License"


[badge__commits__build_vim_makefile__main]:
  https://img.shields.io/github/last-commit/vim-utilities/build-vim-makefile/main.svg

[commits__build_vim_makefile__main]:
  https://github.com/vim-utilities/build-vim-makefile/commits/main
  "&#x1F4DD; History of changes on this branch"


[build_vim_makefile__community]:
  https://github.com/vim-utilities/build-vim-makefile/community
  "&#x1F331; Dedicated to functioning code"


[issues__build_vim_makefile]:
  https://github.com/vim-utilities/build-vim-makefile/issues
  "&#x2622; Search for and _bump_ existing issues or open new issues for project maintainer to address."

[build_vim_makefile__fork_it]:
  https://github.com/vim-utilities/build-vim-makefile/
  "&#x1F531; Fork it!"

[pull_requests__build_vim_makefile]:
  https://github.com/vim-utilities/build-vim-makefile/pulls
  "&#x1F3D7; Pull Request friendly, though please check the Community guidelines"

[build_vim_makefile__main__source_code]:
  https://github.com/vim-utilities/build-vim-makefile/
  "&#x2328; Project source!"

[badge__issues__build_vim_makefile]:
  https://img.shields.io/github/issues/vim-utilities/build-vim-makefile.svg

[badge__pull_requests__build_vim_makefile]:
  https://img.shields.io/github/issues-pr/vim-utilities/build-vim-makefile.svg

[badge__main__build_vim_makefile__source_code]:
  https://img.shields.io/github/repo-size/vim-utilities/build-vim-makefile


[sponsor__shields_io__liberapay]:
  https://img.shields.io/static/v1?logo=liberapay&label=Sponsor&message=vim-utilities

[sponsor__link__liberapay]:
  https://liberapay.com/vim-utilities
  "&#x1F4B1; Sponsor developments and projects that vim-utilities maintains via Liberapay"


[badge_travis_ci]:
  https://travis-ci.com/vim-utilities/build-vim-makefile.svg?branch=main

[build_travis_ci]:
  https://travis-ci.com/vim-utilities/build-vim-makefile

