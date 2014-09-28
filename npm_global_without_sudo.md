Install node packages with npm globally without sudo
======

1. Create a directory for packages:
  ```sh
  mkdir ~/.npm-packages
  ```
2. add this to `.bashrc`
  ```sh
  NPM_PACKAGES="$HOME/.npm-packages"
  NODE_PATH="$NPM_PACKAGES/lib/node_modules:$NODE_PATH"
  PATH="$NPM_PACKAGES/bin:$PATH"
  unset MANPATH
  MANPATH="$NPM_PACKAGES/share/man:$(manpath)"
  ```
3. add this to `~/.npmrc`:
  ```
  prefix="~/.npm-packages"
  ```

See this [StackOverflow thread](http://stackoverflow.com/a/13021677).

