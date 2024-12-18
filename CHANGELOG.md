# Changelog

* 2024.11.29        sclocka-1.1.2.2
  * ANSI Escape secuences is back as a backup method of getting the screen size
  * Use `-r` option if you dont want to disabe echo and put terminal into raw mode

* 2024.11.23        sclocka-1.1.2.1
  * Set default terminal sreen size to 80x24
  * Suppress `-Wunused-result` when compiled under GCC
  * Show an error message when failed to start an external screensaver

* 2024.11.23        sclocka-1.1.2
  * Missed `FD_ZERO()` added to init the descriptor set to the null set.

* 2024.11.23        sclocka-1.1.1
  * Use `struct winsize` instead of ANSI Escape sequences for getting terminal window size

* 2024.11.22        sclocka-1.1.0
  * `-E  "/path/to/binary/saver args"` option to execute external program as a screensaver.
    Use at your own risk, probably not all the external screensavers will work as expected,
    also they may crash and overall consequences (including security) may be unexpected
    or potentially dangerous.

* 2023.08.18        sclocka-1.0.3
  * `Makefile` fixed, simplified
  * `sclocka.c` minor typo fix
  * `README.md` updated

* 2023.08.17        sclocka-1.0.2
  * `WITH_PAM` variable to control linking PAM library; OpenBSD support

* 2023.07.21        sclocka-1.0.1
  * Form Feed (^L) the default method to clear/restore screen after the show
  * `[-B]` option for Black-only, no screensaver animation
  * [Makefile](Makefile) tweaks; [README.md](README.md) updated for NetBSD
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
