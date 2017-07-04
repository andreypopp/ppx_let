# ppx_let wrapper for use with BuckleScript

This is an npm package which wraps [opam][]-installed ppx\_let package for use with
[BuckleScript][].

## Usage

Make sure you have opam installed and install `ppx_let` opam package:

    opam install ppx_let

Install `andreypopp/ppx_let`:

    npm install andreypopp/ppx_let

Add these lines to `bsconfig.json`:

    ...
    "ppx-flags": [
      "ppx_let/ppx"
    ],
    ...

Now you can write monadic code (hint: useful with `a Js.Promise.t`!).

[opam]: http://opam.ocaml.org
[BuckleScript]: https://github.com/bucklescript/bucklescript
