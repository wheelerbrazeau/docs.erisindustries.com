---

layout: docs
title: "Tutorials | Building From Source"

---

You will need `go` installed to do this.

## [Install Go](https://golang.org/doc/install)

At the current time, `eris` requires `go` >= {{ site.data.coding["golang"].minimum }}. Go is not needed if you install `eris` via a binary installation (details below).

An easy way to install go (for OSX and Linux) is via Travis-CI's [Gimme](https://github.com/travis-ci/gimme) tool. First you install gimme; then `eval $(gimme {{ site.data.coding["golang"].authoritative }})` and you'll be all set up.

Otherwise, please see the documentation in the above link to install go.

Make sure that Go is properly installed by running:

```
go version
```

Once you have go installed, then you will want to make sure that you also have your `$GOPATH` in your `$PATH`. Most gophers add the following line to their `~/.bashrc`, `~/.profile`, `~/.zshrc` file or other relevant file.

```
export PATH="$GOPATH/bin:$PATH"
```

**Note** you will need to make sure that you perform the above command for the *user* which will be running eris.

If you do not add that line to the relevant shell file then you can just type that line into the shell each time you log in. You can check that this change was added by `echo $PATH` and making sure that your path has been updated appropriately.

Now you're ready to install the components of the Eris platform.

## Building `eris` from source.

Go is very easy to build from source. Indeed it is really only one command.

```
go get github.com/eris-ltd/eris-cli/cmd/eris
```

Now you're ready to go.

```
eris init
```

**Tip**: To see all the new stuff happening:

```irc
eris update --branch develop
```
