# Changelog

* 2023.04.27        Current state
  * `ESC[?1049` instead of `ESC[?147` for normal/alt terminal buffer switching
  * Better `[-b c]` terminal capabilities screen restore
  * Updated [README.md](README.md) to reflect changes
  * Added `[-P service]` option to specify a custom PAM service. Useful under
    FreeBSD and others. See the [issue](https://github.com/mezantrop/sclocka/issues/1)
  * Cleaning screen is now the default action, `-c` disbles it
  * Project housekeeping, [README.md](README.md), [CHANGELOG.md](CHANGELOG.md),
    contributors list, etc
  * Fixed some headers, thanks to [Chris Pinnock](https://chrispinnock.com)

* 2023.04.24        sclocka-1.0
  * Initial release
  