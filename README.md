# goenv

rbenv, but for Go.

## Installation

To install the latest stable release:

```
git clone -b v0.0.1 https://github.com/wfarr/goenv.git ~/.goenv
```

Then add the following to your shell config at the end:

```
export PATH="$HOME/.goenv/bin:$PATH"
eval "(goenv init -)"
```

## Usage

```
» goenv help
Usage: goenv <command> [<args>]

Some useful goenv commands are:
   exec        Execute a command from a particular Go version.
   shell       Set GOENV_VERSION for the lifetime of a shell.
   local       Persist the preferred Go version in the cwd.
   global      Persist the preferred Go default version.
   install     Install a version of Go.
   uninstall   Uninstall a version of Go.
   version     Show the current Go version.
   versions    Display all versions of Go installed in `${GOENV_ROOT}/versions/*'.
   rehash      Rehash goenv shims (run this after installing executables)

See `goenv help <command>' for information on a specific command.
```

## Credits

This library was heavily, heavily, heavily inspired by
[@sstephenson](https://github.com/sstephenson)'s
[rbenv](https://github.com/sstephenson/rbenv) and
[ruby-build](https://github.com/sstephenson/ruby-build) projects.
A few ideas were also taken from [nvm](https://github.com/creationix/nvm).

A number of patterns and utilities are borrowed from that project,
and it is my hope that goenv provides the same simplicity,
elegance, and usability that I've come to love in rbenv and ruby-build
for Go users.
