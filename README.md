# Discord Version Manager
### Why?
Why not? Managing Discord branches and versions on Linux is boring, why not have a tool do it for you?

### How?
Installing DVM is easy:
* `git clone https://github.com/aurieh/dvm.sh && cd dvm.sh`
* `./dvm.sh update_path` (if this doesn't work, try adding `$HOME/.dvm/sym` to your PATH manually)
* `dvm install canary` (you can replace `canary` with `stable` and `ptb`, too!)
* `dvm default canary`
* `discord` will then launch Discord Canary

There are several other commands you can use:
* `dvm run <branch>` will launch specific branch of Discord (`canary`, `ptb` or `stable`)
* `dvm update <branch>` will update the branch. Depending on your system, you might need to relink using `dvm default <branch>`
* `dvm uninstall <branch>` removes a specific branch
* `dvm clean <branch>` clears cache, local storage and any leftovers
* `dvm desktop <branch>` generates a desktop file
* `dvm list` lists all versions and branches available