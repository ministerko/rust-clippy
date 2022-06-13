# The Clippy Book

This document explains how to make additions and changes to the Clippy book, the
guide to Clippy that you're reading right now. The Clippy book is formatted with
[Markdown](https://www.markdownguide.org) and generated by
[mdbook](https://github.com/rust-lang/mdBook).

- [Get mdbook](#get-mdbook)
- [Make changes](#make-changes)

## Get mdbook

While not strictly necessary since the book source is simply Markdown text
files, having mdbook locally will allow you to build, test and serve the book
locally to view changes before you commit them to the repository. You likely
already have `cargo` installed, so the easiest option is to simply:

```shell
cargo install mdbook
```

See the mdbook [installation](https://github.com/rust-lang/mdBook#installation)
instructions for other options.

## Make changes

The book's
[src](https://github.com/joshrotenberg/rust-clippy/tree/clippy_guide/book/src)
directory contains all of the markdown files used to generate the book. If you
want to see your changes in real time, you can use the mdbook `serve` command to
run a web server locally that will automatically update changes as they are
made. From the top level of your `rust-clippy` directory:

```shell
mdbook serve book --open
```

Then navigate to `http://localhost:3000` to see the generated book. While the
server is running, changes you make will automatically be updated.

For more information, see the mdbook
[guide](https://rust-lang.github.io/mdBook/).