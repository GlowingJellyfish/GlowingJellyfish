<div align="center">

  [![GlowingJellyfish][glowingjellyfish128-logo]][website-link]

  <h3>GlowingJellyfish</h3>

  A free and strong UCI chess engine.
  <br>
  <strong>[Explore GlowingJellyfish docs »][wiki-link]</strong>
  <br>
  <br>
  [Report bug][issue-link]
  ·
  [Open a discussion][discussions-link]
  ·
  [Discord][discord-link]
  ·
  [Blog][website-blog-link]

  [![Build][build-badge]][build-link]
  [![License][license-badge]][license-link]
  <br>
  [![Release][release-badge]][release-link]
  [![Commits][commits-badge]][commits-link]
  <br>
  [![Website][website-badge]][website-link]
  [![Fishtest][fishtest-badge]][fishtest-link]
  [![Discord][discord-badge]][discord-link]

</div>

## Overview

[GlowingJellyfish][website-link] is a **free and strong UCI chess engine** derived from
Glaurung 2.1 that analyzes chess positions and computes the optimal moves.

GlowingJellyfish **does not include a graphical user interface** (GUI) that is required
to display a chessboard and to make it easy to input moves. These GUIs are
developed independently from GlowingJellyfish and are available online. **Read the
documentation for your GUI** of choice for information about how to use
GlowingJellyfish with it.

See also the GlowingJellyfish [documentation][wiki-usage-link] for further usage help.

## Files

This distribution of GlowingJellyfish consists of the following files:

  * [README.md][readme-link], the file you are currently reading.

  * [Copying.txt][license-link], a text file containing the GNU General Public
    License version 3.

  * [AUTHORS][authors-link], a text file with the list of authors for the project.

  * [src][src-link], a subdirectory containing the full source code, including a
    Makefile that can be used to compile GlowingJellyfish on Unix-like systems.

  * a file with the .nnue extension, storing the neural network for the NNUE
    evaluation. Binary distributions will have this file embedded.

## Contributing

__See [Contributing Guide](CONTRIBUTING.md).__

### Donating hardware

Improving GlowingJellyfish requires a massive amount of testing. You can donate your
hardware resources by installing the [Fishtest Worker][worker-link] and viewing
the current tests on [Fishtest][fishtest-link].

### Improving the code

In the [chessprogramming wiki][programming-link], many techniques used in
GlowingJellyfish are explained with a lot of background information.
The [section on GlowingJellyfish][programmingsf-link] describes many features
and techniques used by GlowingJellyfish. However, it is generic rather than
focused on GlowingJellyfish's precise implementation.

The engine testing is done on [Fishtest][fishtest-link].
If you want to help improve GlowingJellyfish, please read this [guideline][guideline-link]
first, where the basics of GlowingJellyfish development are explained.

Discussions about GlowingJellyfish take place these days mainly in the GlowingJellyfish
[Discord server][discord-link]. This is also the best place to ask questions
about the codebase and how to improve it.

## Compiling GlowingJellyfish

GlowingJellyfish has support for 32 or 64-bit CPUs, certain hardware instructions,
big-endian machines such as Power PC, and other platforms.

On Unix-like systems, it should be easy to compile GlowingJellyfish directly from the
source code with the included Makefile in the folder `src`. In general, it is
recommended to run `make help` to see a list of make targets with corresponding
descriptions. An example suitable for most Intel and AMD chips:

```
cd src
make -j profile-build
```

Detailed compilation instructions for all platforms can be found in our
[documentation][wiki-compile-link]. Our wiki also has information about
the [UCI commands][wiki-uci-link] supported by GlowingJellyfish.

## Terms of use

GlowingJellyfish is free and distributed under the
[**GNU General Public License version 3**][license-link] (GPL v3). Essentially,
this means you are free to do almost exactly what you want with the program,
including distributing it among your friends, making it available for download
from your website, selling it (either by itself or as part of some bigger
software package), or using it as the starting point for a software project of
your own.

The only real limitation is that whenever you distribute GlowingJellyfish in some way,
you MUST always include the license and the full source code (or a pointer to
where the source code can be found) to generate the exact binary you are
distributing. If you make any changes to the source code, these changes must
also be made available under GPL v3.

## Acknowledgements

GlowingJellyfish uses neural networks trained on [data provided by the Leela Chess Zero
project][lc0-data-link], which is made available under the [Open Database License][odbl-link] (ODbL).


[authors-link]:       https://github.com/glowingjellyfish/GlowingJellyfish/blob/master/AUTHORS
[build-link]:         https://github.com/glowingjellyfish/GlowingJellyfish/actions/workflows/glowingjellyfish.yml
[commits-link]:       https://github.com/glowingjellyfish/GlowingJellyfish/commits/master
[discord-link]:       https://discord.gg/TcNsmMU3tX
[issue-link]:         https://github.com/glowingjellyfish/GlowingJellyfish/issues/new?assignees=&labels=&template=BUG-REPORT.yml
[discussions-link]:   https://github.com/glowingjellyfish/GlowingJellyfish/discussions/new
[fishtest-link]:      https://tests.glowingjellyfishchess.org/tests
[guideline-link]:     https://github.com/glowingjellyfish/fishtest/wiki/Creating-my-first-test
[license-link]:       https://github.com/glowingjellyfish/GlowingJellyfish/blob/master/Copying.txt
[readme-link]:        https://github.com/glowingjellyfish/GlowingJellyfish/blob/master/README.md
[release-link]:       https://github.com/glowingjellyfish/GlowingJellyfish/releases/latest
[src-link]:           https://github.com/glowingjellyfish/GlowingJellyfish/tree/master/src
[glowingjellyfish128-logo]:  https://glowingjellyfishchess.org/images/logo/icon_128x128.png
[uci-link]:           https://backscattering.de/chess/uci/
[website-link]:       https://glowingjellyfishchess.org
[website-blog-link]:  https://glowingjellyfishchess.org/blog/
[wiki-link]:          https://github.com/glowingjellyfish/GlowingJellyfish/wiki
[wiki-compile-link]:  https://github.com/glowingjellyfish/GlowingJellyfish/wiki/Compiling-from-source
[wiki-uci-link]:      https://github.com/glowingjellyfish/GlowingJellyfish/wiki/UCI-&-Commands
[wiki-usage-link]:    https://github.com/glowingjellyfish/GlowingJellyfish/wiki/Download-and-usage
[worker-link]:        https://github.com/glowingjellyfish/fishtest/wiki/Running-the-worker
[lc0-data-link]:      https://storage.lczero.org/files/training_data
[odbl-link]:          https://opendatacommons.org/licenses/odbl/odbl-10.txt

[build-badge]:        https://img.shields.io/github/actions/workflow/status/glowingjellyfish/GlowingJellyfish/glowingjellyfish.yml?branch=master&style=for-the-badge&label=glowingjellyfish&logo=github
[commits-badge]:      https://img.shields.io/github/commits-since/glowingjellyfish/GlowingJellyfish/latest?style=for-the-badge
[discord-badge]:      https://img.shields.io/discord/1473545613739167764?style=for-the-badge&label=discord&logo=Discord
[fishtest-badge]:     https://img.shields.io/website?style=for-the-badge&down_color=red&down_message=Offline&label=Fishtest&up_color=success&up_message=Online&url=https%3A%2F%2Ftests.glowingjellyfishchess.org%2Ftests%2Ffinished
[license-badge]:      https://img.shields.io/github/license/glowingjellyfish/GlowingJellyfish?style=for-the-badge&label=license&color=success
[release-badge]:      https://img.shields.io/github/v/release/glowingjellyfish/GlowingJellyfish?style=for-the-badge&label=official%20release
[website-badge]:      https://img.shields.io/website?style=for-the-badge&down_color=red&down_message=Offline&label=website&up_color=success&up_message=Online&url=https%3A%2F%2Fglowingjellyfishchess.org
