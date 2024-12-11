# clang-tools static binaries

<!-- [![Build](https://github.com/cpp-linter/clang-tools-static-binaries/actions/workflows/build-amd64.yml/badge.svg)](https://github.com/cpp-linter/clang-tools-static-binaries/actions/workflows/build-amd64.yml)
[![Test](https://github.com/cpp-linter/clang-tools-static-binaries/actions/workflows/test.yml/badge.svg)](https://github.com/cpp-linter/clang-tools-static-binaries/actions/workflows/test.yml) -->
![](https://img.shields.io/badge/platform-linux--64%20%7C%20win--64%20%7C%20osx--64%20-blue)
![Maintenance](https://img.shields.io/maintenance/yes/2024)

Includes **[clang-format](https://clang.llvm.org/docs/ClangFormat.html), [clang-tidy](https://clang.llvm.org/extra/clang-tidy/), [clang-query](https://github.com/llvm/llvm-project/tree/main/clang-tools-extra/clang-query) and [clang-apply-replacements](https://github.com/llvm/llvm-project/tree/main/clang-tools-extra/clang-apply-replacements)**.

The supported versions are as follows:

| Clang Tools |OS/Version |19|18 |17 |16 |15 |14 |13 |12 |11 |10 |9  |8  |7  |
|:------------|-----------|--|---|---|---|---|---|---|---|---|---|---|---|---|
|clang-format |Linux 64   |✔️|✔️ |✔️|✔️|✔️ |✔️|✔️ |✔️ |✔️|✔️| ✔️|✔️|✔️ |
|             |Window 64  |✔️|✔️ |✔️|✔️|✔️ |✔️|✔️ |✔️ |✔️|✔️| ✔️|✔️|✔️ |
|             |macOS 64   |✔️|✔️ |✔️|✔️|✔️ |✔️|✔️ |✔️ |✔️|✔️| ✔️|✔️|✔️ |
| clang-tidy  |Linux 64   |✔️|✔️ |✔️|✔️|✔️ |✔️|✔️ |✔️ |✔️|✔️| ✔️|✔️|✔️ |
|             |Window 64  |✔️|✔️ |✔️|✔️|✔️ |✔️|✔️ |✔️ |✔️|✔️| ✔️|✔️|✔️ |
|             |macOS 64   |❌|✔️ |✔️|✔️|✔️ |✔️|✔️ |✔️ |✔️|✔️| ✔️|✔️|✔️ |
| clang-query |Linux 64   |✔️|✔️ |✔️|✔️|✔️ |✔️|✔️ |✔️ |✔️|✔️| ✔️|✔️|✔️ |
|             |Window 64  |✔️|✔️ |✔️|✔️|✔️ |✔️|✔️ |✔️ |✔️|✔️| ✔️|✔️|✔️ |
|             |macOS 64   |✔️|✔️ |✔️|✔️|✔️ |✔️|✔️ |✔️ |✔️|✔️| ✔️|✔️|✔️ |
| clang-apply-replacements |Linux 64   |✔️|✔️ |✔️|✔️|✔️ |✔️|✔️ |✔️ |✔️|✔️| ✔️|✔️|✔️ |
|             |Window 64  |✔️|✔️ |✔️|✔️|✔️ |✔️|✔️ |✔️ |✔️|✔️| ✔️|✔️|✔️ |
|             |macOS 64   |✔️|✔️ |✔️|✔️|✔️ |✔️|✔️ |✔️ |✔️|✔️| ✔️|✔️|✔️ |

> [!CAUTION]
> clang-tidy-19_macosx-amd64 - File size exceeds 2GB, unable to upload to GitHub releases. See #40

## Download

* Download clang-tools static binaries for your platform from the [Releases](https://github.com/cpp-linter/clang-tools-static-binaries/releases) tab.
* Alternatively, use the [clang-tools CLI](https://github.com/cpp-linter/clang-tools-pip) to download and manage them.

## Motivation behind this repo

I used to contribute to different repositories and they often use different versions of clang-format.

I could either compile clang-format for each one I want to have or I could try messing up with my package system (I use Arch Linux btw) and try installing all of them on my system.
This can very quickly get out of hand, hence I created this repository.

These binaries aim to:
- be as small as possible
- not require any additional dependencies apart from OS itself

This repository ([cpp-linter/clang-tools-static-binaries](https://github.com/cpp-linter/clang-tools-static-binaries)) is forked from [muttleyxd/clang-tools-static-binaries](https://github.com/muttleyxd/clang-tools-static-binaries).

## How can I trust this repository?

- Verify sha512sums of binaries against output from GitHub Actions to make sure binaries are not modified
- Fork this repository and run GitHub actions on your behalf
- Build and test manually using steps and commands from [.github/workflows](https://github.com/cpp-linter/clang-tools-static-binaries/tree/master/.github/workflows)
