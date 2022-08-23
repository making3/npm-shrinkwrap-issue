# npm-shrinkwrap-issue

This repository is for reproducing an issue when installing a tarball thrugh NPM, where a npm-shrinkwrap.json file included in the tarball is ignored. 

## Prerequisites 

- NPM v8+ (NPM v6 can be used to compare)

To reproduce:

1. Clone this repository. 
2. Run `npm pack`.
3. In a separate directory, run `npm install /path/to/packed/npm-shrinkwrap-issue-1.0.0.tgz`.
4. Notice React is installed at version 17.0.2 (or later).
