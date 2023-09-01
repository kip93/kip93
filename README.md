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
* ➡️ Pushed 461 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#05b53f8](https://github.com/OroraTech/nixpkgs/commit/05b53f8) mediainfo-gui: 23.06 -&gt; 23.07
  * [#4ea7276](https://github.com/OroraTech/nixpkgs/commit/4ea7276) mediainfo: 23.06 -&gt; 23.07
  * [#dad5a44](https://github.com/OroraTech/nixpkgs/commit/dad5a44) libmediainfo: 23.06 -&gt; 23.07
  * [#40e8205](https://github.com/OroraTech/nixpkgs/commit/40e8205) flutter: 3.10.5 -&gt; 3.13.0

flutter: Update remaining engine artifact hashes for v3.13.0

Co-Authored-By: hacker1024 &lt;20849728+hacker1024@users.noreply.github.com&gt;
  * [#a791f73](https://github.com/OroraTech/nixpkgs/commit/a791f73) qgis-ltr: disable building tests

No tests are currently executed during the build process. Disable
building them to save significant amount of time and resources.
  * [#0e82f77](https://github.com/OroraTech/nixpkgs/commit/0e82f77) qgis-ltr: alphabetical sorting of dependencies
  * [#09f9749](https://github.com/OroraTech/nixpkgs/commit/09f9749) qgis: alphabetical sorting of dependencies
  * [#2cf9345](https://github.com/OroraTech/nixpkgs/commit/2cf9345) qgis-ltr: 3.28.7 -&gt; 3.28.10
  * [#b2a14fc](https://github.com/OroraTech/nixpkgs/commit/b2a14fc) qgis: disable building tests

No tests are currently executed during the build process. Disable
building them to save significant amount of time and resources.
  * [#446297f](https://github.com/OroraTech/nixpkgs/commit/446297f) python310Packages.unstructured: add optional-dependencies
  * [#fc77028](https://github.com/OroraTech/nixpkgs/commit/fc77028) python310Packages.libtmux: 0.22.1 -&gt; 0.23.0post0
  * [#3d5fdc9](https://github.com/OroraTech/nixpkgs/commit/3d5fdc9) net-snmp: 5.9.3 -&gt; 5.9.4
  * [#55774d1](https://github.com/OroraTech/nixpkgs/commit/55774d1) qucs-s: 1.1.0 -&gt; 2.0.0
  * [#59c8dfb](https://github.com/OroraTech/nixpkgs/commit/59c8dfb) samba: 4.18.5 -&gt; 4.18.6
  * [#f58a607](https://github.com/OroraTech/nixpkgs/commit/f58a607) chickenPackages: turn into scope

The purpose of this change is to allow the overriding of one egg, which in turn
affects all dependents of that eggs.
  * [#a3dd3cc](https://github.com/OroraTech/nixpkgs/commit/a3dd3cc) chickenPackages.chickenEggs: update
  * [#2da0307](https://github.com/OroraTech/nixpkgs/commit/2da0307) buildFHSEnv: fix `NIX_LDFLAGS` propagation to `ld` wrapper

Before the change the following command did not work:

    $ nix develop -i --impure --expr &#39;with import &lt;nixpkgs&gt; { system = &#34;i686-linux&#34;; }; (buildFHSUserEnv { name = &#34;t&#34;; targetPkgs = ps: with ps; [ libmpc stdenv.cc ]; }).env&#39;
    $ ld -lmpc -o a
    ld: cannot find -lmpc: No such file or directory

It is expected to work as `NIX_LDFLAGS` does contain valid values:

    $ echo $NIX_LDFLAGS
    -L/usr/lib -L/usr/lib32

Note that for `gcc` it does work:

    $ printf &#34;int main(){}&#34; |  gcc -x c - -lmpc -o a

It happens because `HOST` role is enabled for `cc`:

    $ echo $NIX_CC_WRAPPER_TARGET_HOST_i686_unknown_linux_gnu
    1

But not for `BINTOOLS`:

    $ echo $NIX_BINTOOLS_WRAPPER_TARGET_HOST_i686_unknown_linux_gnu
    &lt;empty&gt;

The change adds BINTOOLS role and fixes linking:

    $ nix develop -i --impure --expr &#39;with import ~/nm { system = &#34;i686-linux&#34;; }; (buildFHSUserEnv { name = &#34;t&#34;; targetPkgs = ps: with ps; [ libmpc stdenv.cc ]; }).env&#39;
    $ printf &#34;int main(){}&#34; |  gcc -x c - -lmpc -o a
    $ ld -lmpc -o a
    ld: warning: cannot find entry symbol _start; not setting start address
  * [#69c5328](https://github.com/OroraTech/nixpkgs/commit/69c5328) omegat: 4.3.0 -&gt; 6.0.0
  * [#cc4bb23](https://github.com/OroraTech/nixpkgs/commit/cc4bb23) perf: enable `perf stat` evens supported by `libpfm`
  * [#98741b7](https://github.com/OroraTech/nixpkgs/commit/98741b7) maui-shell: 0.5.6 -&gt; 0.6.6
  * *On 31 Aug 2023, 17:02:55*
* ➡️ Pushed 106 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#854e4a2](https://github.com/OroraTech/nixpkgs/commit/854e4a2) organicmaps: 2023.06.04-13 -&gt; 2023.08.18-8
  * [#4073d2c](https://github.com/OroraTech/nixpkgs/commit/4073d2c) Re-add broken Darwin
  * [#9d8520f](https://github.com/OroraTech/nixpkgs/commit/9d8520f) ccl: 1.12 -&gt; 1.12.2
  * [#cbe6f4e](https://github.com/OroraTech/nixpkgs/commit/cbe6f4e) linux_xanmod_latest: 6.4.11 -&gt; 6.4.12
  * [#ab51eca](https://github.com/OroraTech/nixpkgs/commit/ab51eca) linux_xanmod: 6.1.46 -&gt; 6.1.47
  * [#b945eca](https://github.com/OroraTech/nixpkgs/commit/b945eca) exiftool: 12.62 -&gt; 12.65

https://github.com/exiftool/exiftool/compare/12.62...12.65
  * [#9745182](https://github.com/OroraTech/nixpkgs/commit/9745182) python310Packages.pyiqvia: 2022.10.0 -&gt; 2023.08.1
  * [#73243f1](https://github.com/OroraTech/nixpkgs/commit/73243f1) python310Packages.bpycv: 0.3.6 -&gt; 0.4.0
  * [#8b80043](https://github.com/OroraTech/nixpkgs/commit/8b80043) python310Packages.pip-tools: 7.2.0 -&gt; 7.3.0
  * [#c033c47](https://github.com/OroraTech/nixpkgs/commit/c033c47) vips: 8.14.3 -&gt; 8.14.4
  * [#9fb1308](https://github.com/OroraTech/nixpkgs/commit/9fb1308) python310Packages.stumpy: 1.11.1 -&gt; 1.12.0
  * [#e196073](https://github.com/OroraTech/nixpkgs/commit/e196073) birdfont: 2.32.3 -&gt; 2.33.1
  * [#aee8eed](https://github.com/OroraTech/nixpkgs/commit/aee8eed) libcouchbase: 3.3.7 -&gt; 3.3.8
  * [#b2386a0](https://github.com/OroraTech/nixpkgs/commit/b2386a0) bluej: 5.1.0 -&gt; 5.2.0

https://bluej.org/versions.html
  * [#902814d](https://github.com/OroraTech/nixpkgs/commit/902814d) python311Packages.fastapi: 0.95.1 -&gt; 0.95.2
  * [#18b2685](https://github.com/OroraTech/nixpkgs/commit/18b2685) python311Packages.starlette: 0.26.1 -&gt; 0.27.0

Diff: https://github.com/encode/starlette/compare/refs/tags/0.26.1...0.27.0

Changelog: https://github.com/encode/starlette/releases/tag/0.27.0
  * [#b2788a6](https://github.com/OroraTech/nixpkgs/commit/b2788a6) ddccontrol: 0.6.1 -&gt; 0.6.2
  * [#c2cd085](https://github.com/OroraTech/nixpkgs/commit/c2cd085) metabase: 0.46.6.1 -&gt; 0.46.7

Fixes CVE-2023-37470.

Changelogs:
https://github.com/metabase/metabase/releases/tag/v0.46.7
https://github.com/metabase/metabase/releases/tag/v0.46.6.4
https://github.com/metabase/metabase/releases/tag/v0.46.6.3
https://github.com/metabase/metabase/releases/tag/v0.46.6.2
  * [#eeb19e9](https://github.com/OroraTech/nixpkgs/commit/eeb19e9) djvulibre: patch multiple CVEs

Signed-off-by: Henri Rosten &lt;henri.rosten@unikie.com&gt;
  * [#fdb8abb](https://github.com/OroraTech/nixpkgs/commit/fdb8abb) moodle: 4.1.3 -&gt; 4.1.4

Fixes CVE-2023-35131, CVE-2023-35132 and CVE-2023-35133.

Changelog:
https://moodledev.io/general/releases/4.1/4.1.4
  * *On 30 Aug 2023, 11:29:53*
* ➡️ Pushed 289 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#0837ab4](https://github.com/OroraTech/nixpkgs/commit/0837ab4) zrok: 0.4.2 -&gt; 0.4.5
  * [#06366e8](https://github.com/OroraTech/nixpkgs/commit/06366e8) nwg-drawer: 0.3.8 -&gt; 0.3.9
  * [#1e7ec47](https://github.com/OroraTech/nixpkgs/commit/1e7ec47) radarr: 4.6.4.7568 -&gt; 4.7.5.7809
  * [#fb3601e](https://github.com/OroraTech/nixpkgs/commit/fb3601e) netmaker: 0.20.5 -&gt; 0.20.6
  * [#8370543](https://github.com/OroraTech/nixpkgs/commit/8370543) fheroes2: 1.0.6 -&gt; 1.0.7
  * [#ba787d2](https://github.com/OroraTech/nixpkgs/commit/ba787d2) python310Packages.ansible: 8.2.0 -&gt; 8.3.0
  * [#78edd5b](https://github.com/OroraTech/nixpkgs/commit/78edd5b) mc: 4.8.29 -&gt; 4.8.30
  * [#43475f1](https://github.com/OroraTech/nixpkgs/commit/43475f1) stress-ng: 0.15.10 -&gt; 0.16.04
  * [#a8de2f0](https://github.com/OroraTech/nixpkgs/commit/a8de2f0) pgbackrest: 2.46 -&gt; 2.47
  * [#667d019](https://github.com/OroraTech/nixpkgs/commit/667d019) vmagent: 1.91.3 -&gt; 1.93.0
  * [#c92c960](https://github.com/OroraTech/nixpkgs/commit/c92c960) libdigidocpp: 3.15.0 -&gt; 3.16.0
  * [#c34b58a](https://github.com/OroraTech/nixpkgs/commit/c34b58a) weave-gitops: 0.28.0 -&gt; 0.29.0
  * [#dc1330d](https://github.com/OroraTech/nixpkgs/commit/dc1330d) libburn: 1.5.4 -&gt; 1.5.6
  * [#be63df4](https://github.com/OroraTech/nixpkgs/commit/be63df4) ibus-engines.table-others: 1.3.16 -&gt; 1.3.17
  * [#a5017e3](https://github.com/OroraTech/nixpkgs/commit/a5017e3) besu: 23.4.1 -&gt; 23.4.4
  * [#25e0861](https://github.com/OroraTech/nixpkgs/commit/25e0861) utf8cpp: 3.2.3 -&gt; 3.2.4
  * [#fbb3f82](https://github.com/OroraTech/nixpkgs/commit/fbb3f82) pkg: 1.20.4 -&gt; 1.20.5
  * [#494196b](https://github.com/OroraTech/nixpkgs/commit/494196b) python311Packages.asyncpg: 0.27.0 -&gt; 0.28.0

Changelog: https://github.com/MagicStack/asyncpg/releases/tag/v0.28.0
  * [#0245990](https://github.com/OroraTech/nixpkgs/commit/0245990) mpd-mpris: 0.4.0-2 -&gt; 0.4.1
  * [#b0dc3d2](https://github.com/OroraTech/nixpkgs/commit/b0dc3d2) doc/stdenv: Minor syntax fix.
  * *On 30 Aug 2023, 07:56:37*
* ➡️ Pushed 92 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#cc57329](https://github.com/OroraTech/nixpkgs/commit/cc57329) postgresqlPackages.pgvector: 0.4.4 -&gt; 0.5.0

Diff: https://github.com/pgvector/pgvector/compare/v0.4.4...v0.5.0

Changelog: https://github.com/pgvector/pgvector/raw/v0.5.0/CHANGELOG.md
  * [#f487088](https://github.com/OroraTech/nixpkgs/commit/f487088) git-branchless: 0.7.1 -&gt; 0.8.0

Diff: https://github.com/arxanas/git-branchless/compare/v0.7.1...0.8.0
  * [#acafc8e](https://github.com/OroraTech/nixpkgs/commit/acafc8e) flutter.buildFlutterApplication: fix passthru being ignored

Signed-off-by: lucasew &lt;lucas59356@gmail.com&gt;
  * [#bda4a66](https://github.com/OroraTech/nixpkgs/commit/bda4a66) ispc: 1.19.0 -&gt; 1.20.0
  * [#3901f0c](https://github.com/OroraTech/nixpkgs/commit/3901f0c) libnvme: add withDocs

The libnvme documentation fails to build when cross compiling, with:

 FAILED: doc/nvme_admin_opcode.2
 /nix/store/qcvcsink30f4wh36jzg3rbvkshwzj38c-meson-1.1.1/bin/meson --internal exe --capture doc/nvme_admin_opcode.2 -- /build/source/doc/kernel-doc -module libnvme -man -function nvme_admin_opcode ../doc/../src/nvme/types.h
 Traceback (most recent call last):
   File &#34;/nix/store/qcvcsink30f4wh36jzg3rbvkshwzj38c-meson-1.1.1/bin/meson&#34;, line 6, in &lt;module&gt;
   File &#34;/nix/store/qcvcsink30f4wh36jzg3rbvkshwzj38c-meson-1.1.1/lib/python3.10/site-packages/mesonbuild/mesonmain.py&#34;, line 30, in &lt;module&gt;
     from . import mlog
 ImportError: cannot import name &#39;mlog&#39; from &#39;mesonbuild&#39; (/nix/store/qcvcsink30f4wh36jzg3rbvkshwzj38c-meson-1.1.1/lib/python3.10/site-packages/mesonbuild/__init__.py)
 [703/811] Generating doc/nvme_identify_cns_man with a custom command (wrapped by meson to capture output)
 FAILED: doc/nvme_identify_cns.2
 /nix/store/qcvcsink30f4wh36jzg3rbvkshwzj38c-meson-1.1.1/bin/meson --internal exe --capture doc/nvme_identify_cns.2 -- /build/source/doc/kernel-doc -module libnvme -man -function nvme_identify_cns ../doc/../src/nvme/types.h
 Traceback (most recent call last):
   File &#34;/nix/store/qcvcsink30f4wh36jzg3rbvkshwzj38c-meson-1.1.1/bin/meson&#34;, line 6, in &lt;module&gt;
   File &#34;/nix/store/qcvcsink30f4wh36jzg3rbvkshwzj38c-meson-1.1.1/lib/python3.10/site-packages/mesonbuild/mesonmain.py&#34;, line 30, in &lt;module&gt;
     from . import mlog
  * [#2872237](https://github.com/OroraTech/nixpkgs/commit/2872237) python3Packages.pytest-recording: 0.12.2 -&gt; 0.13.0
  * [#4959264](https://github.com/OroraTech/nixpkgs/commit/4959264) cargo-shuttle: 0.24.0 -&gt; 0.25.1

Diff: https://github.com/shuttle-hq/shuttle/compare/v0.24.0...v0.25.1

Changelog: https://github.com/shuttle-hq/shuttle/releases/tag/v0.25.1
  * [#9a18f86](https://github.com/OroraTech/nixpkgs/commit/9a18f86) heisenbridge 1.14.4 -&gt; 1.14.5
  * [#77f65ff](https://github.com/OroraTech/nixpkgs/commit/77f65ff) gobble: init at 1.3

https://github.com/EmperorPenguin18/gobble
  * [#9836685](https://github.com/OroraTech/nixpkgs/commit/9836685) python310Packages.apkit: init at unstable 2022-08-23
  * [#f949b36](https://github.com/OroraTech/nixpkgs/commit/f949b36) blackfire: 2.20.0 -&gt; 2.21.0
  * [#65fe58d](https://github.com/OroraTech/nixpkgs/commit/65fe58d) commitizen: 3.5.2 -&gt; 3.7.0

https://github.com/commitizen-tools/commitizen/compare/v3.5.2...3.7.0

https://github.com/commitizen-tools/commitizen/releases/tag/3.7.0
https://github.com/commitizen-tools/commitizen/releases/tag/3.6.0
  * [#b86adcb](https://github.com/OroraTech/nixpkgs/commit/b86adcb) swaynotificationcenter: backport PR 296
  * [#75919c9](https://github.com/OroraTech/nixpkgs/commit/75919c9) flyway: 9.21.1 -&gt; 9.21.2
  * [#28d93b8](https://github.com/OroraTech/nixpkgs/commit/28d93b8) sioyek: fix build
  * [#bb9a708](https://github.com/OroraTech/nixpkgs/commit/bb9a708) python311Packages.async-upnp-client: 0.34.1 -&gt; 0.35.0

Diff: https://github.com/StevenLooman/async_upnp_client/compare/refs/tags/0.34.1...0.35.0

Changelog: https://github.com/StevenLooman/async_upnp_client/blob/0.35.0/CHANGES.rst
  * [#0e5622c](https://github.com/OroraTech/nixpkgs/commit/0e5622c) python311Packages.bluetooth-data-tools: 1.9.0 -&gt; 1.9.1

Diff: https://github.com/Bluetooth-Devices/bluetooth-data-tools/compare/refs/tags/v1.9.0...v1.9.1

Changelog: https://github.com/Bluetooth-Devices/bluetooth-data-tools/blob/v1.9.1/CHANGELOG.md
  * [#748d749](https://github.com/OroraTech/nixpkgs/commit/748d749) python311Packages.fnv-hash-fast: 0.4.0 -&gt; 0.4.1

Diff: https://github.com/bdraco/fnv-hash-fast/compare/v0.4.0...v0.4.1

Changelog: https://github.com/bdraco/fnv-hash-fast/blob/v0.4.1/CHANGELOG.md
  * [#1792924](https://github.com/OroraTech/nixpkgs/commit/1792924) rust-traverse: init at 2.0.0

https://github.com/dmcg310/Rust-Traverse
  * [#c7f827e](https://github.com/OroraTech/nixpkgs/commit/c7f827e) atlas: init at 0.13.3
  * *On 29 Aug 2023, 15:21:22*
 <!-- Last activity -->


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.33.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 1 Sept 2023, 03:58:10 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
