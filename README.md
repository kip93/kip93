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
* ➡️ Pushed 32 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#77cb27d](https://github.com/OroraTech/nixpkgs/commit/77cb27d) cartridges: 2.2.1 -&gt; 2.3 (#252415)

* cartridges: 2.2.1 -&gt; 2.3

Diff: https://github.com/kra-mo/cartridges/compare/v2.2.1...v2.3

* cartridges: apply suggestion

Co-authored-by: Anderson Torres &lt;torres.anderson.85@protonmail.com&gt;

---------

Co-authored-by: Weijia Wang &lt;9713184+wegank@users.noreply.github.com&gt;
Co-authored-by: Anderson Torres &lt;torres.anderson.85@protonmail.com&gt;
  * [#92df924](https://github.com/OroraTech/nixpkgs/commit/92df924) Merge pull request #253238 from saschagrunert/conmon-rs

conmon-rs: 0.5.0 -&gt; 0.6.0
  * [#acccb8f](https://github.com/OroraTech/nixpkgs/commit/acccb8f) quodlibet: 4.5.0 -&gt; 4.6.0
  * [#c373e02](https://github.com/OroraTech/nixpkgs/commit/c373e02) quodlibet: refactor
  * [#fdd9171](https://github.com/OroraTech/nixpkgs/commit/fdd9171) trackma: 0.8.5 -&gt; 0.8.6

Switch to pyproject:
https://aur.archlinux.org/packages/trackma-git#comment-902732
https://github.com/z411/trackma/pull/653
  * [#ca34aba](https://github.com/OroraTech/nixpkgs/commit/ca34aba) trackma: switch to pydbus for MPRIS tracker

Trackma uses pydbus since v0.8.5:
https://github.com/z411/trackma/releases/tag/v0.8.5
https://github.com/z411/trackma/pull/529
  * [#b56f814](https://github.com/OroraTech/nixpkgs/commit/b56f814) nixos/tests/akkoma: Disable retrieving timeline
  * [#f278395](https://github.com/OroraTech/nixpkgs/commit/f278395) akkoma-fe: 2023-05-23 -&gt; 2023-08-05
  * [#dd1ca36](https://github.com/OroraTech/nixpkgs/commit/dd1ca36) akkoma: 3.9.3 -&gt; 3.10.4
  * [#df0ab79](https://github.com/OroraTech/nixpkgs/commit/df0ab79) oras: 1.0.1 -&gt; 1.1.0
  * [#571ed5c](https://github.com/OroraTech/nixpkgs/commit/571ed5c) envoy: 1.26.3 -&gt; 1.26.4
  * [#2fefc49](https://github.com/OroraTech/nixpkgs/commit/2fefc49) conmon-rs: 0.5.0 -&gt; 0.6.0

Signed-off-by: Sascha Grunert &lt;sgrunert@redhat.com&gt;
  * [#38e5440](https://github.com/OroraTech/nixpkgs/commit/38e5440) dioxus-cli: 0.3.2 -&gt; 0.4.0
  * [#e7fb265](https://github.com/OroraTech/nixpkgs/commit/e7fb265) valhalla, osmscout-server: fix build

To avoid linker errors, they need an older version of protobuf, both
with abseil-cpp built using the same C++17 standard as valhalla and
osmscout-server.
  * [#900db7c](https://github.com/OroraTech/nixpkgs/commit/900db7c) valhalla: Fix build error relating to std::set
  * [#58f7dcd](https://github.com/OroraTech/nixpkgs/commit/58f7dcd) valhalla: fix build with gcc 12
  * [#3b8f352](https://github.com/OroraTech/nixpkgs/commit/3b8f352) vcluster: 0.15.2 -&gt; 0.15.6
  * [#32cd6f0](https://github.com/OroraTech/nixpkgs/commit/32cd6f0) linuxPackages.ena: 2.8.6 -&gt; 2.8.9

Removes several patches added in d915eb8 which are now included in-tree.

Notable commits, excluding aforementioned patches:
 + linux/ena: Add rx_overruns to ena-com structs
 + linux/ena: Report RX overrun errors via net device stats
 + linux/ena: Fix incorrect dma sync when SWIOTLB is on

full changelog: https://github.com/amzn/amzn-drivers/compare/ena_linux_2.8.6...ena_linux_2.8.9
  * [#1d5976f](https://github.com/OroraTech/nixpkgs/commit/1d5976f) gawkextlib: unstable-2019-11-21 -&gt; unstable-2022-10-20
  * [#79aeeef](https://github.com/OroraTech/nixpkgs/commit/79aeeef) tuifimanager: 3.0.0 -&gt; 3.3.1
  * *On 6 Sept 2023, 15:03:33*
* 💬 Commented on [#253261 pkgsNative: init](https://github.com/NixOS/nixpkgs/issues/253261) from [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  * *On 6 Sept 2023, 14:31:10*
* ➡️ Pushed 20 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#4c87ec6](https://github.com/OroraTech/nixpkgs/commit/4c87ec6) Merge pull request #253576 from dotlambda/zammad-fetchYarnDeps

zammad: use fetchYarnDeps
  * [#631827b](https://github.com/OroraTech/nixpkgs/commit/631827b) Merge pull request #253617 from qowoz/gh

gh: 2.33.0 -&gt; 2.34.0
  * [#553f543](https://github.com/OroraTech/nixpkgs/commit/553f543) Merge pull request #253577 from dotlambda/meshcentral-fetchYarnDeps

meshcentral: use fetchYarnDeps
  * [#42f2215](https://github.com/OroraTech/nixpkgs/commit/42f2215) Merge pull request #253571 from dotlambda/apache-airflow-fetchYarnDeps

apache-airflow: use fetchYarnDeps
  * [#7d2b631](https://github.com/OroraTech/nixpkgs/commit/7d2b631) Merge pull request #253567 from dotlambda/outline-fetchYarnDeps

outline: use fetchYarnDeps
  * [#7cbc821](https://github.com/OroraTech/nixpkgs/commit/7cbc821) Merge pull request #252865 from emily-is-my-username/fix/fetchgit-deepclone

`fetchgit`: don&#39;t shallow clone if `deepClone` is requested
  * [#979817e](https://github.com/OroraTech/nixpkgs/commit/979817e) Merge pull request #253603 from wineee/dmenu

dmenu-wayland: unstable-2022-11-04 -&gt; unstable-2023-05-18
  * [#9425de0](https://github.com/OroraTech/nixpkgs/commit/9425de0) Merge pull request #253618 from r-ryantm/auto-update/yamlfmt

yamlfmt: 0.9.0 -&gt; 0.10.0
  * [#fc30ed0](https://github.com/OroraTech/nixpkgs/commit/fc30ed0) Merge pull request #253615 from r-ryantm/auto-update/podman

podman: 4.6.1 -&gt; 4.6.2
  * [#e15c884](https://github.com/OroraTech/nixpkgs/commit/e15c884) Merge pull request #253609 from r-ryantm/auto-update/convimg

convimg: 9.1 -&gt; 9.2
  * [#0afc6e6](https://github.com/OroraTech/nixpkgs/commit/0afc6e6) yamlfmt: 0.9.0 -&gt; 0.10.0
  * [#0c7527f](https://github.com/OroraTech/nixpkgs/commit/0c7527f) gh: 2.33.0 -&gt; 2.34.0

Diff: https://github.com/cli/cli/compare/v2.33.0...v2.34.0

Changelog: https://github.com/cli/cli/releases/tag/v2.34.0
  * [#5431fa2](https://github.com/OroraTech/nixpkgs/commit/5431fa2) podman: 4.6.1 -&gt; 4.6.2
  * [#8516b64](https://github.com/OroraTech/nixpkgs/commit/8516b64) convimg: 9.1 -&gt; 9.2
  * [#f33cdfa](https://github.com/OroraTech/nixpkgs/commit/f33cdfa) dmenu-wayland: unstable-2022-11-04 -&gt; unstable-2023-05-18
  * [#f5abc06](https://github.com/OroraTech/nixpkgs/commit/f5abc06) meshcentral: use fetchYarnDeps
  * [#622fe95](https://github.com/OroraTech/nixpkgs/commit/622fe95) zammad: use fetchYarnDeps
  * [#a756944](https://github.com/OroraTech/nixpkgs/commit/a756944) apache-airflow: use fetchYarnDeps
  * [#f5f1fe8](https://github.com/OroraTech/nixpkgs/commit/f5f1fe8) outline: use fetchYarnDeps
  * [#ad94541](https://github.com/OroraTech/nixpkgs/commit/ad94541) fetchgit: don&#39;t shallow clone if deepClone is requested

fixes: https://github.com/NixOS/nixpkgs/issues/179788
  * *On 6 Sept 2023, 13:51:17*
* ➡️ Pushed 942 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `feature/pkgs-native`
  * [#8fd949b](https://github.com/OroraTech/nixpkgs/commit/8fd949b) exempi: 2.6.3 -&gt; 2.6.4
  * [#04df8d6](https://github.com/OroraTech/nixpkgs/commit/04df8d6) make-startupitem: fix typo in comment
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
  * [#b675aae](https://github.com/OroraTech/nixpkgs/commit/b675aae) exim: Fix exiwhat command
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
  * [#0ab3a1f](https://github.com/OroraTech/nixpkgs/commit/0ab3a1f) nixos/nftables: add redirect for /etc/hosts
  * [#75e405c](https://github.com/OroraTech/nixpkgs/commit/75e405c) nixos/nftables: use environment.etc for redirects
  * [#9e51ec8](https://github.com/OroraTech/nixpkgs/commit/9e51ec8) nixos/nftables: add checkRulesetRedirects option
  * [#ad94541](https://github.com/OroraTech/nixpkgs/commit/ad94541) fetchgit: don&#39;t shallow clone if deepClone is requested

fixes: https://github.com/NixOS/nixpkgs/issues/179788
  * *On 6 Sept 2023, 13:50:02*
 <!-- Last activity -->


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.33.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 7 Sept 2023, 13:57:20 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
