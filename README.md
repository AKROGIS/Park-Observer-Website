# Park Observer Website

An internal NPS website for Park Observer documentation and support files.

This contents of this repository is the master copy of the deployed content at https://akrgis.nps.gov/apps/observer, except as noted below.

## Deployed files not in repo

1. All `*.ipa` files in the `downloads` folder/sub-folders
2. All deployed `*.tpk` files in the `maps` folder.
3. [ParkObserver.pyt](https://github.com/AKROGIS/Park-Observer-poz2fgdb)
   to the `downloads2` folder.

The `ipa` and `tpk` files are large binary files that are not suitable
for maintainingin a github repo. Master files can be found on the T
drive.

Several of the files in the `specs` folder are derived from other
content. See the readme file in that folder for details.

## Repo files not deployed

Note: It won't hurt if these files get deployed to the
web server, but they are not used by the website.

1. This readme.md file.
2. git files (.gitignore .gitattributes .git/)
3. specs/readme.md
4. help2/*.md

Some of the html files in `specs` were generated from markdown
in the Park Observer repo.  These html files should not be edited
directly, but rather updated per the instructions in
specs\readme.md when the source is updated.

The html files in `help2` are mostly generated from markdown (*.md)
files with the same names.  These html files provide the document
structure, navigation and style, but the content of each
article in the `main` tag is generated from the content in the
similarly names markdown file.  There is also a note to the same
effect at the top of each markdown file, as well as
instructions for updating the html from the markdown.
