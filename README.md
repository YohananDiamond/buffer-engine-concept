# Buffer Engine (Concept)

> This is an experimental project and anything is subject to change.

This repository is supposed to store concepts about a text-based
environment similar to Vim, Emacs and others.

Some of its goals are:

- To be modular: (mostly) everything should be a module, and they could
  be added, replaced, edited or moved - even the most internal ones -.

- To be portable: it should work at least in the current three major
  desktop platforms: Linux, MacOS and Windows.

- To be fast: runtime and (mostly) startup should not be slow. Only modules that
  need to be loaded should be so.

One another goal - supported by the modular and fast goals - is to work
as a framework that can be used to make more text-based applications,
like git interfaces, to-do list managers etc. without a big overhead.

The starting point is in [this index file](INDEX.md) (still incomplete).

<!-- Talk about portability in USB somewhere else -->

## Contributing

If you feel like contributing to the concepts in the repositories, thank
you! I'll be happy for receiving new concepts, critics or even just
organization of the repository via a Github **Issue** or **Pull
Request**.

Reading the [contributing guidelines](CONTRIBUTING.md) file is recommended.
