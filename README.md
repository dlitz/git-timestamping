Git post-commit timestamping hook
=================================

This is inspired by [Ocead's Automated Timestamping] but it works without
touching the working tree, index, or stash.  It's a post-commit hook that
communicates with an [RFC 3161]/[RFC 5816] timestamping service (currently
hard-coded to [freetsa.org]) and writes the result into a separate branch.

*I recommend you do not use this.*  It's buggy and basically only works with a
linear history.  I wrote it in a hurry for one private project and probably
won't keep working on it.  I am open to pull requests, but it might be better to
contribute to Ocead's tool instead.

License
-------
This software is released under the [MIT License].

Code formatting
---------------
I run [isort] and [black] on the source code.

[Ocead's Automated Timestamping]: https://github.com/Ocead/timestamping
[RFC 3161]: https://www.rfc-editor.org/rfc/rfc3161.html
[RFC 5816]: https://www.rfc-editor.org/rfc/rfc5816.html
[freetsa.org]: https://freetsa.org/
[MIT License]: LICENSE
[isort]: https://pycqa.github.io/isort/
[black]: https://black.readthedocs.io/en/stable/
