# asdf-coq

[![Build Status](https://travis-ci.org/gingerhot/asdf-coq.svg?branch=master)](https://travis-ci.org/gingerhot/asdf-coq)

[Coq](https://coq.inria.fr/) plugin for [asdf](https://github.com/asdf-vm/asdf) version manager.


## Install

```shell
asdf plugin-add coq https://github.com/gingerhot/asdf-coq
```

## Prerequisites

* OCaml
* OPAM

you need install some packages for building Coq:

```
opam install -y num ocamlfind camlp5
```

## Usage

List all available Coq versions:

```
asdf list-all coq
```

Install one version of Coq:

```
asdf install coq 8.7.0
```

More `asdf` command details to [asdf](https://github.com/asdf-vm/asdf) README.

## Note

* CoqIDE not included in this installation
* Some Coq version depends on OCaml version, e.g. for Coq 8.6.1, OCaml must comply >= "4.01.0" and < "4.06.0". More info see `Available` item in: https://opam.ocaml.org/packages/coq/coq.8.6.1/ (change the 8.6.1 to your version). You may also need asdf [OCaml plugin](https://github.com/vic/asdf-ocaml) to install corresponding version OCaml at first.
