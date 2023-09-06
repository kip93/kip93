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
* ➡️ Pushed 610 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#19cb4d5](https://github.com/OroraTech/nixpkgs/commit/19cb4d5) Merge staging-next into staging
  * [#b1c95fb](https://github.com/OroraTech/nixpkgs/commit/b1c95fb) python3Packages.pip: silence pip warning in build
  * [#30b6520](https://github.com/OroraTech/nixpkgs/commit/30b6520) python3.pkgs.pip: install man pages
  * [#ea8fbff](https://github.com/OroraTech/nixpkgs/commit/ea8fbff) python311Packages.cryptography-vectors: 41.0.2 -&gt; 41.0.3
  * [#65fb82b](https://github.com/OroraTech/nixpkgs/commit/65fb82b) python311Packages.cryptography: 41.0.2 -&gt; 41.0.3

Changelog: https://cryptography.io/en/latest/changelog/#v41-0-3
  * [#74ac830](https://github.com/OroraTech/nixpkgs/commit/74ac830) protobuf: init 3.24
  * [#8fd949b](https://github.com/OroraTech/nixpkgs/commit/8fd949b) exempi: 2.6.3 -&gt; 2.6.4
  * [#67df31a](https://github.com/OroraTech/nixpkgs/commit/67df31a) playerctl: support cross compilation

documentation build requires an emulator when cross compiling;
pass `withDocs = false` to disable.
  * [#4ed0668](https://github.com/OroraTech/nixpkgs/commit/4ed0668) python310Packages.faust-cchardet: 2.1.18 -&gt; 2.1.19

Diff: https://github.com/faust-streaming/cChardet/compare/refs/tags/v2.1.18...v2.1.19

Changelog: https://github.com/faust-streaming/cChardet/releases/tag/v2.1.19
  * [#3f52185](https://github.com/OroraTech/nixpkgs/commit/3f52185) boot.initrd.systemd: make TPM2 modules optional
  * [#dc7cdbe](https://github.com/OroraTech/nixpkgs/commit/dc7cdbe) cargo-auditable-cargo-wrapper: add test
  * [#8522d78](https://github.com/OroraTech/nixpkgs/commit/8522d78) cargo-auditable-cargo-wrapper: fix wrapper

Packages were not correctly built with carog-auditable due to the
missing auditable flag
  * [#23b3bf2](https://github.com/OroraTech/nixpkgs/commit/23b3bf2) python310Packages.pikepdf: 8.2.1 -&gt; 8.3.0

Diff: https://github.com/pikepdf/pikepdf/compare/v8.2.1...v8.3.0

Changelog: https://github.com/pikepdf/pikepdf/blob/v8.3.0/docs/releasenotes/version8.rst
  * [#4337cf0](https://github.com/OroraTech/nixpkgs/commit/4337cf0) lvm2: 2.03.21 -&gt; 2.03.22

https://github.com/lvmteam/lvm2/blob/v2_03_22/WHATS_NEW
  * [#f8262c2](https://github.com/OroraTech/nixpkgs/commit/f8262c2) ceph: 17.2.5 -&gt; 18.2.0

The following issues were encountered during the upgrade:

* &#34;Could NOT find thrift (missing: thrift_LIBRARIES thrift_INCLUDE_DIR)&#34;
  Fixed by disabling Jaeger support, see added comment.
* ```
  /build/ceph-18.2.0/src/extblkdev/ExtBlkDevInterface.h:38:10: fatal error: sys/capability.h: No such file or directory
    38 | #include &lt;sys/capability.h&gt;
  ```
  Fixed by `libcap` dependency.
  Ceph&#39;s Debian dependencies include both `libcap` and `libcap-ng`:
  https://github.com/ceph/ceph/blob/c8c946c970300d37c345af9fc6b25abb003e00b5/debian/control#L38-L39
* ```
  Manually-specified variables were not used by the project:
    MGR_PYTHON_VERSION
  ```
  Dropped 4 years ago for Ceph 15:
  https://github.com/ceph/ceph/commit/5fc657b40dc7d27e84d4b62b5f37d9c771d74fcd
  So I removed the flag.
* Warning:
  ```
  -- Could NOT find nasm
  ```
  Looking at the code (macros such as `HAVE_NASM_X64`), nasm existence actually results in some optimised crypto SIMD instructions being compiled, so we probably want this for performance.
  Adding `nasm` to `nativeBuildInputs` first brought error:
  ```
  /nix/store/p6dlr3skfhxpyphipg2bqnj52999banh-bash-5.2-p15/bin/bash: line 1: /build/ceph-18.2.0/src/nasm-wrapper: cannot execute: required file not found
  make[2]: *** [src/crypto/isa-l/CMakeFiles/ceph_crypto_isal.dir/build.make:117: src/crypto/isa-l/CMakeFiles/ceph_crypto_isal.dir/isa-l_crypto/aes/cbc_multibinary.asm.o] Error 127
  ```
  Solution: `patchShebangs src/nasm-wrapper`, even better `patchShebangs src/`.
* ```
  Manually-specified variables were not used by the project:
    WITH_SYSTEM_CIMG
    WITH_SYSTEM_JSONCPP
  ```
  These never were Ceph CMake options, so I removed them.
* `libcap-ng` is Linux-only, and only used for the `mount.ceph` command:
  https://github.com/ceph/ceph/blob/c8c946c970300d37c345af9fc6b25abb003e00b5/src/CMakeLists.txt#L829-L830
  Thus use it for Linux only.
* The Parquet build error is now gone, so we can enable support for it.
  * [#01b07af](https://github.com/OroraTech/nixpkgs/commit/01b07af) temporal-cli: Disable tests on x86_64-darwin due to Rosetta 2

They succeed for me (with multiple runs) on x86_64-darwin native (no
Rosetta 2). Afaik, Hydra performs x86_64-darwin builds on Rosetta 2 on
aarch64-darwin. I do not have the hardware to reproduce this (and it
could be a build issue), so let’s disable the tests for now and go from
there.
  * [#614b639](https://github.com/OroraTech/nixpkgs/commit/614b639) ubootTools: add man pages

As far as I can tell, there are no makefile targets to install these, or
anything like that, so we have to do it by hand.

This adds man pages for dumpimage, kwboot, mkeficapsule, and mkimage.
There are no man pages in other sections than 1.
  * [#46383fc](https://github.com/OroraTech/nixpkgs/commit/46383fc) linuxManualConfig: set badPlatforms

Older kernels shouldn&#39;t be marked as supporting architectures that
were only added to the kernel later.
  * [#8c7898a](https://github.com/OroraTech/nixpkgs/commit/8c7898a) stegsolve: more precise license
  * [#0984477](https://github.com/OroraTech/nixpkgs/commit/0984477) kodiPackages.certifi: 2022.9.24 -&gt; 2023.5.7
  * *On 6 Sept 2023, 12:00:52*
* ➡️ Pushed 44 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#54f9a6e](https://github.com/OroraTech/nixpkgs/commit/54f9a6e) ddccontrol: 0.6.2 -&gt; 0.6.3
  * [#1875196](https://github.com/OroraTech/nixpkgs/commit/1875196) op-geth: 1.101106.0 -&gt; 1.101200.0
  * [#77a450f](https://github.com/OroraTech/nixpkgs/commit/77a450f) Merge pull request #253359 from r-ryantm/auto-update/protonmail-bridge

protonmail-bridge: 3.3.2 -&gt; 3.4.1
  * [#4690c42](https://github.com/OroraTech/nixpkgs/commit/4690c42) pv-migrate: 1.2.0 -&gt; 1.3.0
  * [#3c28508](https://github.com/OroraTech/nixpkgs/commit/3c28508) pluto: 5.18.2 -&gt; 5.18.3
  * [#321f0e1](https://github.com/OroraTech/nixpkgs/commit/321f0e1) phpExtensions.opentelemetry: 1.0.0beta6 -&gt; 1.0.0beta7
  * [#40daff2](https://github.com/OroraTech/nixpkgs/commit/40daff2) gitui: 0.24.1 -&gt; 0.24.2

Changelog: https://github.com/extrawurst/gitui/blob/0.24.2/CHANGELOG.md
  * [#b21ef1a](https://github.com/OroraTech/nixpkgs/commit/b21ef1a) codeql: 2.14.2 -&gt; 2.14.3
  * [#d3e1909](https://github.com/OroraTech/nixpkgs/commit/d3e1909) protonmail-bridge: 3.3.2 -&gt; 3.4.1
  * [#21d18dc](https://github.com/OroraTech/nixpkgs/commit/21d18dc) matrix-synapse: 1.91.0 -&gt; 1.91.1

https://github.com/matrix-org/synapse/releases/tag/v1.91.1
Signed-off-by: Sumner Evans &lt;me@sumnerevans.com&gt;
  * [#0c40d64](https://github.com/OroraTech/nixpkgs/commit/0c40d64) cloudfoundry-cli: 8.7.1 -&gt; 8.7.2
  * [#2fe9b16](https://github.com/OroraTech/nixpkgs/commit/2fe9b16) civo: 1.0.61 -&gt; 1.0.65
  * [#91c779c](https://github.com/OroraTech/nixpkgs/commit/91c779c) checkov: 2.4.22 -&gt; 2.4.25

Diff: https://github.com/bridgecrewio/checkov/compare/refs/tags/2.4.22...2.4.25

Changelog: https://github.com/bridgecrewio/checkov/releases/tag/2.4.25
  * [#a0463e8](https://github.com/OroraTech/nixpkgs/commit/a0463e8) zon2nix: 0.1.1 -&gt; 0.1.2

Diff: https://github.com/nix-community/zon2nix/compare/v0.1.1...v0.1.2

Changelog: https://github.com/nix-community/zon2nix/blob/v0.1.2/CHANGELOG.md
  * [#4a65ac3](https://github.com/OroraTech/nixpkgs/commit/4a65ac3) python310Packages.sklearn-deap: refactor

- add format
- add unittestCheckHook to nativeCheckInputs
- enable pythonImportsCheck
- change the license to MIT from LGPL3
  * [#69953bf](https://github.com/OroraTech/nixpkgs/commit/69953bf) python310Packages.sklearn-deap: 0.2.3 -&gt; 0.3.0

Diff: https://github.com/rsteca/sklearn-deap/compare/0.2.3...0.3.0
  * [#e66d494](https://github.com/OroraTech/nixpkgs/commit/e66d494) pysensation: init at 1.0.0

https://github.com/mimseyedi/pysentation
  * [#9c6b830](https://github.com/OroraTech/nixpkgs/commit/9c6b830) anytype: wayland support
  * [#6c5d6e2](https://github.com/OroraTech/nixpkgs/commit/6c5d6e2) harmonia: 0.7.1 -&gt; 0.7.2
  * [#b675aae](https://github.com/OroraTech/nixpkgs/commit/b675aae) exim: Fix exiwhat command
  * *On 5 Sept 2023, 13:00:42*
* ➡️ Pushed 77 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#caaf41e](https://github.com/OroraTech/nixpkgs/commit/caaf41e) python310Packages.appthreat-vulnerability-db: 5.2.5 -&gt; 5.4.1
  * [#a58c29c](https://github.com/OroraTech/nixpkgs/commit/a58c29c) python310Packages.idasen: 0.10.0 -&gt; 0.10.1
  * [#94bfdb5](https://github.com/OroraTech/nixpkgs/commit/94bfdb5) python310Packages.pyaml: 23.7.0 -&gt; 23.9.1
  * [#12962a9](https://github.com/OroraTech/nixpkgs/commit/12962a9) sbt-extras: 2023-07-25 -&gt; 2023-08-28
  * [#f5c50d5](https://github.com/OroraTech/nixpkgs/commit/f5c50d5) python310Packages.s3fs: 2023.6.0 -&gt; 2023.9.0
  * [#ed1a0ab](https://github.com/OroraTech/nixpkgs/commit/ed1a0ab) python310Packages.ansible-core: 2.15.2 -&gt; 2.15.3
  * [#8012e0d](https://github.com/OroraTech/nixpkgs/commit/8012e0d) python310Packages.jupyter-console: 6.6.1 -&gt; 6.6.3

Changelog: https://github.com/jupyter/jupyter_console/releases/tag/v6.6.3
  * [#a960eac](https://github.com/OroraTech/nixpkgs/commit/a960eac) python310Packages.jupyter-console: add jupyter team as maintainers
  * [#eb85576](https://github.com/OroraTech/nixpkgs/commit/eb85576) python310Packages.jupyter-console: rename from jupyter_console
  * [#fd80879](https://github.com/OroraTech/nixpkgs/commit/fd80879) herbstluftwm: fix tests with recent X versions
  * [#a481f7c](https://github.com/OroraTech/nixpkgs/commit/a481f7c) fwts: 23.05.00 -&gt; 23.07.00
  * [#d0d2a84](https://github.com/OroraTech/nixpkgs/commit/d0d2a84) gama: 2.24 -&gt; 2.25
  * [#6cfa5c5](https://github.com/OroraTech/nixpkgs/commit/6cfa5c5) inotify-tools: 3.22.6.0 -&gt; 4.23.8.0
  * [#9ceb610](https://github.com/OroraTech/nixpkgs/commit/9ceb610) libblockdev: 3.0.2 -&gt; 3.0.3
  * [#9a4f4fd](https://github.com/OroraTech/nixpkgs/commit/9a4f4fd) riemann_c_client: 1.10.5 -&gt; 2.1.1
  * [#0874967](https://github.com/OroraTech/nixpkgs/commit/0874967) python310Packages.python-manilaclient: 4.5.1 -&gt; 4.6.0
  * [#c4a9adf](https://github.com/OroraTech/nixpkgs/commit/c4a9adf) birdtray: 1.9.0 -&gt; 1.11.3
  * [#7b42c82](https://github.com/OroraTech/nixpkgs/commit/7b42c82) python311Packages.gitpython: 3.1.32 -&gt; 3.1.33

Diff: https://github.com/gitpython-developers/GitPython/compare/refs/tags/3.1.32...3.1.33

Changelog: https://github.com/gitpython-developers/GitPython/blob/3.1.33/doc/source/changes.rst
  * [#bbaa00d](https://github.com/OroraTech/nixpkgs/commit/bbaa00d) ocenaudio: 3.12.5 -&gt; 3.12.6
  * [#40654da](https://github.com/OroraTech/nixpkgs/commit/40654da) fldigi: 4.1.26 -&gt; 4.1.27
  * *On 5 Sept 2023, 10:57:56*
* ➡️ Pushed 196 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `chore/fix-sphinx-hook`
  * [#1a8886c](https://github.com/OroraTech/nixpkgs/commit/1a8886c) code-maat: init at 1.0.3

* the JAR is provided in ./libexec/code-maat (e.g. to reuse as a JAR dependnecy
in a Java project)
* the JAR is wrapped as an executable in ./bin/code-maat

Closes https://github.com/NixOS/nixpkgs/issues/208339
  * [#6959687](https://github.com/OroraTech/nixpkgs/commit/6959687) nixos/mautrix-telegram: drop removed --base-config flag

See also: https://github.com/mautrix/python/commit/9b67b17ac4927f63cc9a71dc450b9296c849b3ab
  * [#57df80f](https://github.com/OroraTech/nixpkgs/commit/57df80f) python310Packages.mautrix: 0.20.0 -&gt; 0.20.1

Changelog: https://github.com/mautrix/python/releases/tag/v0.20.1
Diff: https://github.com/mautrix/python/compare/v0.20.0...v0.20.1
  * [#5ee40b8](https://github.com/OroraTech/nixpkgs/commit/5ee40b8) exiv2: fix build on armv7l-linux

Remove failing tests for now, they&#39;re fixed in 0.28
  * [#5ab4510](https://github.com/OroraTech/nixpkgs/commit/5ab4510) nixos/budgie: Use the Network Manager Applet indicator

Signed-off-by: Federico Damián Schonborn &lt;fdschonborn@gmail.com&gt;
  * [#1db1e3c](https://github.com/OroraTech/nixpkgs/commit/1db1e3c) stdenv: Fix possible issues discovered with

```
set -o errexit -o nounset -o pipefail
shopt -s inherit_errexit
```

in `stdenv/default-builder.sh`
  * [#2127f21](https://github.com/OroraTech/nixpkgs/commit/2127f21) khard: add manpages to output
  * [#60241e2](https://github.com/OroraTech/nixpkgs/commit/60241e2) ldtk: 1.3.3 -&gt; 1.3.4
  * [#c0158e9](https://github.com/OroraTech/nixpkgs/commit/c0158e9) dosfstools: backport reproducible builds patch

Upstream, dosfstools respects SOURCE_DATE_EPOCH since this commit:
https://github.com/dosfstools/dosfstools/commit/8da7bc93315cb0c32ad868f17808468b81fa76ec
This means tools like mkfs.vfat will create deterministic outputs when SOURCE_DATE_EPOCH is set.
A backport in nixpkgs is warranted since this was already merged in 2021 and no release of dosfstools has been made since then.

Co-authored-by: Paul Meyer &lt;49727155+katexochen@users.noreply.github.com&gt;
  * [#dffc973](https://github.com/OroraTech/nixpkgs/commit/dffc973) hotdoc: 0.13.7 -&gt; 0.15
  * [#cb49832](https://github.com/OroraTech/nixpkgs/commit/cb49832) Remove dotnet dependency
  * [#582e30f](https://github.com/OroraTech/nixpkgs/commit/582e30f) wasabiwallet: 2.0.3 -&gt; 2.0.4
  * [#ebc420c](https://github.com/OroraTech/nixpkgs/commit/ebc420c) signal-desktop-beta: 6.24.0-beta.1 -&gt; 6.30.0-beta.2
  * [#25f0477](https://github.com/OroraTech/nixpkgs/commit/25f0477) signal-desktop: 6.27.1 -&gt; 6.29.1
  * [#2a3e20a](https://github.com/OroraTech/nixpkgs/commit/2a3e20a) geos: pull upstream fix for gcc-13 build failure

Without the change build against `gcc-13` fails as:

    $ nix build --impure --expr &#39;with import ./. {}; geos.override { stdenv = gcc13Stdenv; }&#39; -L
    ...
    /build/geos-3.11.2/include/geos/shape/fractal/HilbertEncoder.h:41:5: error: &#39;uint32_t&#39; does not name a type
       41 |     uint32_t encode(const geom::Envelope* env);
          |     ^~~~~~~~
    /build/geos-3.11.2/include/geos/shape/fractal/HilbertEncoder.h:21:1: note: &#39;uint32_t&#39; is defined in header &#39;&lt;cstdint&gt;&#39;; did you forget to &#39;#include &lt;cstdint&gt;&#39;?
       20 | #include &lt;vector&gt;
      +++ |+#include &lt;cstdint&gt;
  * [#55e4f1f](https://github.com/OroraTech/nixpkgs/commit/55e4f1f) cm256cc: pull fix pending upstream inclusion for gcc-13

Without the change build fails on `gcc-13` as:

    $ nix build --impure --expr &#39;with import ./. {}; cm256cc.override { stdenv = gcc13Stdenv; }&#39; -L
    ...
    /build/source/unit_test/data.h:37:9: error: &#39;uint16_t&#39; does not name a type
       37 |         uint16_t i;
          |         ^~~~~~~~
    /build/source/unit_test/data.h:33:1: note: &#39;uint16_t&#39; is defined in header &#39;&lt;cstdint&gt;&#39;; this is probably fixable by adding &#39;#include &lt;cstdint&gt;&#39;
       32 | #include &lt;string.h&gt;
      +++ |+#include &lt;cstdint&gt;
  * [#04df8d6](https://github.com/OroraTech/nixpkgs/commit/04df8d6) make-startupitem: fix typo in comment
  * [#0ab3a1f](https://github.com/OroraTech/nixpkgs/commit/0ab3a1f) nixos/nftables: add redirect for /etc/hosts
  * [#75e405c](https://github.com/OroraTech/nixpkgs/commit/75e405c) nixos/nftables: use environment.etc for redirects
  * [#9e51ec8](https://github.com/OroraTech/nixpkgs/commit/9e51ec8) nixos/nftables: add checkRulesetRedirects option
  * *On 5 Sept 2023, 09:45:56*
 <!-- Last activity -->


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.33.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 6 Sept 2023, 13:57:44 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
