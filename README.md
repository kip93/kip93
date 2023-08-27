<!-- README template, populated using this action:
     https://github.com/kip93/kip93/blob/main/.github/workflows/readme.yml. -->

<h1 align="center">👋 Hello world! I'm @kip93</h1> <!-- LOGIN => username -->

### 👤 About me

I am a passionate self-taught backend software developer, and a strong advocate for libre software.


### 💬 Some facts

* 📅 Coding since 2013.
* 💼 Currently working @ [OroraTech](https://ororatech.com/).
* 👨‍💻 [Python](https://github.com/search?q=user%3Akip93&l=python) is ❤️. <!-- LOGIN => username -->
* 💻 [NixOS](https://github.com/NixOS/) /
     [Awesome](https://github.com/awesomeWM/) /
     [kitty](https://github.com/kovidgoyal/kitty/) /
     [xonsh](https://github.com/xonsh/).
* 🌐 I have a [portfolio website](https://kip93.net/) with some more information.
* 📝 Checkout my [résumé](https://kip93.net/resume/) for even more detail.
* 📫 Reach me @ [leandro@kip93.net](mailto:leandro@kip93.net).
* 🎲 Fun fact: My first program was not a "Hello World" (it was simple R/W in an [HC11 µC](https://en.wikipedia.org/wiki/68HC11) emulator).


-----------------------------------------------------------------------------------------------------------------------


### 📈 Stats

![](./stats.svg)


### 📚 Most used languages <!-- by percentage, in decreasing order -->

![](./languages.svg)


### 🏅 Achievements

![](./achievements.svg)


-----------------------------------------------------------------------------------------------------------------------


**[📰 Recent activity](https://github.com/kip93)**
* ➡️ Pushed 389 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#ca2198d](https://github.com/OroraTech/nixpkgs/commit/ca2198d) python310Packages.molecule-plugins: init at 23.4.1
  * [#8377b96](https://github.com/OroraTech/nixpkgs/commit/8377b96) maintainers: add dawidd6
  * [#994f256](https://github.com/OroraTech/nixpkgs/commit/994f256) Fix nixBufferBuilders for newer emacs
  * [#0465502](https://github.com/OroraTech/nixpkgs/commit/0465502) libcifpp: 5.1.0.1 -&gt; 5.1.2

Diff: https://github.com/PDB-REDO/libcifpp/compare/refs/tags/v5.1.0.1...v5.1.2

Changelog: https://github.com/PDB-REDO/libcifpp/releases/tag/refs/tags/v5.1.2
  * [#1ff383d](https://github.com/OroraTech/nixpkgs/commit/1ff383d) pt2-clone: 1.61 -&gt; 1.62.2
  * [#db7d495](https://github.com/OroraTech/nixpkgs/commit/db7d495) python3Packages.pillow-simd: Fix cross compilation
  * [#6bcf6a8](https://github.com/OroraTech/nixpkgs/commit/6bcf6a8) python3Packages.pillow: Fix cross compilation

Fixes the build time error:
`ModuleNotFoundError: No module named &#39;setuptools&#39;`.
  * [#44c0e45](https://github.com/OroraTech/nixpkgs/commit/44c0e45) python311Packages.aioquic: 0.9.20 -&gt; 0.9.21
  * [#c76bb0d](https://github.com/OroraTech/nixpkgs/commit/c76bb0d) nixos/zsh: add enableLsColors

Borrowed from nixos/bash/ls-colors module
  * [#c77a792](https://github.com/OroraTech/nixpkgs/commit/c77a792) openturns: 1.20 -&gt; 1.21

Diff: https://github.com/openturns/openturns/compare/v1.20...v1.21

Changelog: https://github.com/openturns/openturns/raw/v1.21/ChangeLog
  * [#5fda11d](https://github.com/OroraTech/nixpkgs/commit/5fda11d) python311Packages.hahomematic: 2023.7.3 -&gt; 2023.8.2

Diff: https://github.com/danielperna84/hahomematic/compare/refs/tags/2023.7.3...2023.8.2

Changelog: https://github.com/danielperna84/hahomematic/releases/tag/2023.8.2
  * [#ee9d0f2](https://github.com/OroraTech/nixpkgs/commit/ee9d0f2) python311Packages.hahomematic: 2023.7.0 -&gt; 2023.7.3

Changelog: https://github.com/danielperna84/hahomematic/releases/tag/2023.7.3
  * [#ff1c16c](https://github.com/OroraTech/nixpkgs/commit/ff1c16c) skytemple: 1.4.7 -&gt; 1.5.4
  * [#13de9df](https://github.com/OroraTech/nixpkgs/commit/13de9df) python3Packages.skytemple-files: 1.4.7 -&gt; 1.5.4
  * [#9078796](https://github.com/OroraTech/nixpkgs/commit/9078796) python3Packages.explorerscript: 0.1.2 -&gt; 0.1.3
  * [#0fb2e4d](https://github.com/OroraTech/nixpkgs/commit/0fb2e4d) python3Packages.skytemple-rust: 1.4.0.post0 -&gt; 1.5.3
  * [#cc78173](https://github.com/OroraTech/nixpkgs/commit/cc78173) python3Packages.notmuch2: use bindingconfig that works on darwin

Instead of using the configure generated _notmuch_config.py, we generate
our own which correctly references each respective field.

The _notmuch_config.py in notmuch.bindingconfig contained references to
the build directory. On linux this didn&#39;t break anything due to the
sandbox always having a build root of /build. But on darwin this would
be different depending on the derivation being built. So the build
accidently worked since version.txt would end up in the same place on
linux.

It seems in practice NOTMUCH_LIB_DIR not containing the built libraries
did not break the build. Either way after this commit it will point to
the correct place.

For convenience the _notmuch_config.py from notmuch.bindingconfig is
viewable here
https://gist.github.com/keegancsmith/bdc2f0e44425ad68c8b6a85f8ed0b289

We do not remove the bindingconfig output from notmuch in this commit
since in my local testing that just caused cache invalidations on
notmuch. But can do that as well.
  * [#7e26c8d](https://github.com/OroraTech/nixpkgs/commit/7e26c8d) prometheus-exporter-nextcloud: support for auth tokens

Fixes #176849
  * [#0fcf35a](https://github.com/OroraTech/nixpkgs/commit/0fcf35a) singularity: specify &#34;nvidia-container-cli path&#34;
  * [#466e154](https://github.com/OroraTech/nixpkgs/commit/466e154) apptainer, singularity: fix wrapper PATH prefix

Fix the missing trailing /bin in f6e7fcc
  * *On 25 Aug 2023, 14:22:30*
* 💬 Commented on [#249157 python3Packages.sphinxHook: Fix cross compilation](https://github.com/NixOS/nixpkgs/issues/249157) from [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  * *On 25 Aug 2023, 13:36:55*
* ➡️ Pushed 4489 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `chore/fix-sphinx-hook`
  * [#3c21c54](https://github.com/OroraTech/nixpkgs/commit/3c21c54) python311Packages.zeroconf: 0.80.0 -&gt; 0.81.0

Diff: https://github.com/jstasiak/python-zeroconf/compare/refs/tags/0.80.0...0.81.0

Changelog: https://github.com/python-zeroconf/python-zeroconf/releases/tag/0.81.0
  * [#c260ba3](https://github.com/OroraTech/nixpkgs/commit/c260ba3) texlab: 5.9.0 -&gt; 5.9.2
  * [#589dd15](https://github.com/OroraTech/nixpkgs/commit/589dd15) cargo-bisect-rustc: 0.6.6 -&gt; 0.6.7
  * [#77ff76f](https://github.com/OroraTech/nixpkgs/commit/77ff76f) keycloak: allow enabling and disabling features
  * [#0109e11](https://github.com/OroraTech/nixpkgs/commit/0109e11) chisel: 1.9.0 -&gt; 1.9.1

Diff: https://github.com/jpillora/chisel/compare/refs/tags/v1.9.0...v1.9.1

Changelog: https://github.com/jpillora/chisel/releases/tag/v1.9.1
  * [#73d8867](https://github.com/OroraTech/nixpkgs/commit/73d8867) python311Packages.bthome-ble: 3.1.0 -&gt; 3.1.1

Diff: https://github.com/Bluetooth-Devices/bthome-ble/compare/refs/tags/v3.1.0...v3.1.1

Changelog: https://github.com/bluetooth-devices/bthome-ble/blob/v3.1.1/CHANGELOG.md
  * [#942eb6f](https://github.com/OroraTech/nixpkgs/commit/942eb6f) python311Packages.boschshcpy: 0.2.66 -&gt; 0.2.67

Diff: https://github.com/tschamm/boschshcpy/compare/0.2.66...0.2.67
  * [#2ff705a](https://github.com/OroraTech/nixpkgs/commit/2ff705a) Merge pull request #250690 from r-ryantm/auto-update/dgraph

dgraph: 23.0.1 -&gt; 23.1.0
  * [#104ea46](https://github.com/OroraTech/nixpkgs/commit/104ea46) Merge pull request #250691 from r-ryantm/auto-update/cirrus-cli

cirrus-cli: 0.101.2 -&gt; 0.102.0
  * [#697252e](https://github.com/OroraTech/nixpkgs/commit/697252e) xplr: add figsoda to maintainers
  * [#ec58e59](https://github.com/OroraTech/nixpkgs/commit/ec58e59) xplr: fix build on aarch64-linux and x86_64-darwin
  * [#0f750be](https://github.com/OroraTech/nixpkgs/commit/0f750be) cloud-sql-proxy: 2.6.0 -&gt; 2.6.1
  * [#e6d94b7](https://github.com/OroraTech/nixpkgs/commit/e6d94b7) Merge pull request #250697 from XYenon/master

yazi: init at 0.1.3
  * [#0dd53d0](https://github.com/OroraTech/nixpkgs/commit/0dd53d0) Merge pull request #250776 from figsoda/clima

clima: init at 1.1.0
  * [#041cf2e](https://github.com/OroraTech/nixpkgs/commit/041cf2e) Merge pull request #250734 from ncfavier/weechat

weechat-unwrapped: 4.0.3 -&gt; 4.0.4
  * [#9ced47b](https://github.com/OroraTech/nixpkgs/commit/9ced47b) Merge pull request #250772 from figsoda/xc

xc: 0.4.1 -&gt; 0.5.0
  * [#931bebd](https://github.com/OroraTech/nixpkgs/commit/931bebd) Merge pull request #250771 from figsoda/dysk

dysk: 2.7.2 -&gt; 2.8.0
  * [#434fe8e](https://github.com/OroraTech/nixpkgs/commit/434fe8e) maintainers: remove @alexeyre from maintainers-list.nix
  * [#cb14c82](https://github.com/OroraTech/nixpkgs/commit/cb14c82) scli: remove @alexeyre from maintainers
  * [#be152a8](https://github.com/OroraTech/nixpkgs/commit/be152a8) nimbo: remove @alexeyre from maintainers
  * *On 25 Aug 2023, 13:32:05*
* ⏺️ Created new branch chore/fix-pillow in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs)
  * *On 25 Aug 2023, 13:23:06*
 <!-- Last activity -->


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.33.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 27 Aug 2023, 22:57:23 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
