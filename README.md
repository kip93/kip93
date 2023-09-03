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
* ➡️ Pushed 226 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#46c7997](https://github.com/OroraTech/nixpkgs/commit/46c7997) ispc: 1.20.0 -&gt; 1.21.0
  * [#b0e9686](https://github.com/OroraTech/nixpkgs/commit/b0e9686) python311Packages.pkg-about: init at 1.0.8
  * [#4a14236](https://github.com/OroraTech/nixpkgs/commit/4a14236) multiviewer-for-f1: 1.26.2 -&gt; 1.26.4
  * [#e8efc18](https://github.com/OroraTech/nixpkgs/commit/e8efc18) containerlab: 0.44.2 -&gt; 0.44.3

Diff: https://github.com/srl-labs/containerlab/compare/v0.44.2...v0.44.3

Changelog: https://github.com/srl-labs/containerlab/releases/tag/v0.44.3
  * [#d07ebff](https://github.com/OroraTech/nixpkgs/commit/d07ebff) yash: 2.54 -&gt; 2.55
  * [#d564dfa](https://github.com/OroraTech/nixpkgs/commit/d564dfa) sambamba: 1.0.0 -&gt; 1.0.1
  * [#c7bb136](https://github.com/OroraTech/nixpkgs/commit/c7bb136) kubefirst: 2.2.7 -&gt; 2.2.9
  * [#6c2f7bc](https://github.com/OroraTech/nixpkgs/commit/6c2f7bc) oneshot: 1.5.1 -&gt; 2.0.1
  * [#4fce50f](https://github.com/OroraTech/nixpkgs/commit/4fce50f) rpi-imager: disable telemetry by default
  * [#996dbb1](https://github.com/OroraTech/nixpkgs/commit/996dbb1) rpi-imager: add installCheck
  * [#6db520b](https://github.com/OroraTech/nixpkgs/commit/6db520b) rpi-imager: add passthru.updateScript
  * [#8fe2040](https://github.com/OroraTech/nixpkgs/commit/8fe2040) rpi-imager: add anthonyroussel to maintainers
  * [#22f6f91](https://github.com/OroraTech/nixpkgs/commit/22f6f91) rpi-imager: 1.7.4 -&gt; 1.7.5

See https://github.com/raspberrypi/rpi-imager/releases/tag/v1.7.5
  * [#110ebe9](https://github.com/OroraTech/nixpkgs/commit/110ebe9) python310Packages.pytorch-lightning: 2.0.6 -&gt; 2.0.7
  * [#ccffaec](https://github.com/OroraTech/nixpkgs/commit/ccffaec) nuclear: 0.6.27 -&gt; 0.6.30
  * [#6c462a5](https://github.com/OroraTech/nixpkgs/commit/6c462a5) qtstyleplugin-kvantum: fix loading builtin themes on Qt 6

Signed-off-by: Sefa Eyeoglu &lt;contact@scrumplex.net&gt;
  * [#cd135d4](https://github.com/OroraTech/nixpkgs/commit/cd135d4) qtstyleplugin-kvantum: add suffix to Qt 6 variant

Signed-off-by: Sefa Eyeoglu &lt;contact@scrumplex.net&gt;
  * [#896b2b9](https://github.com/OroraTech/nixpkgs/commit/896b2b9) ArchiSteamFarm: 5.4.7.3 -&gt; 5.4.8.3
  * [#d746f25](https://github.com/OroraTech/nixpkgs/commit/d746f25) curl: Fix cross-compilation to Windows by not forcing gssSupport

E.g. `nix build .#pkgsCross.mingwW64.curl` would fail. The params for
curl already have `gssSupport = !isStatic &amp;&amp; …`, so removing this
doesn’t really have any effect since it’s already `true` when possible
and `false` for static platforms.
  * [#9f6dad5](https://github.com/OroraTech/nixpkgs/commit/9f6dad5) c-ares: ensure passthru.tests&#39; curl is built with c-ares support

kinda pointless otherwise
  * *On 1 Sept 2023, 09:31:12*
* ➡️ Pushed 1125 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `feature/add-libpcap`
  * [#b945eca](https://github.com/OroraTech/nixpkgs/commit/b945eca) exiftool: 12.62 -&gt; 12.65

https://github.com/exiftool/exiftool/compare/12.62...12.65
  * [#65fe58d](https://github.com/OroraTech/nixpkgs/commit/65fe58d) commitizen: 3.5.2 -&gt; 3.7.0

https://github.com/commitizen-tools/commitizen/compare/v3.5.2...3.7.0

https://github.com/commitizen-tools/commitizen/releases/tag/3.7.0
https://github.com/commitizen-tools/commitizen/releases/tag/3.6.0
  * [#9745182](https://github.com/OroraTech/nixpkgs/commit/9745182) python310Packages.pyiqvia: 2022.10.0 -&gt; 2023.08.1
  * [#ed59f79](https://github.com/OroraTech/nixpkgs/commit/ed59f79) kubeseal: 0.23.0 -&gt; 0.23.1
  * [#e6f84c7](https://github.com/OroraTech/nixpkgs/commit/e6f84c7) grsync: 1.3.0 -&gt; 1.3.1
  * [#5d914aa](https://github.com/OroraTech/nixpkgs/commit/5d914aa) ocamlPackages.arp: 3.0.0 → 3.1.0
  * [#be3cdca](https://github.com/OroraTech/nixpkgs/commit/be3cdca) maintainers: add zaldnoay
  * [#116480d](https://github.com/OroraTech/nixpkgs/commit/116480d) kstars: 3.6.4 -&gt; 3.6.6
  * [#73243f1](https://github.com/OroraTech/nixpkgs/commit/73243f1) python310Packages.bpycv: 0.3.6 -&gt; 0.4.0
  * [#8b80043](https://github.com/OroraTech/nixpkgs/commit/8b80043) python310Packages.pip-tools: 7.2.0 -&gt; 7.3.0
  * [#4aa2931](https://github.com/OroraTech/nixpkgs/commit/4aa2931) libcef: 116.0.14 -&gt; 116.0.15
  * [#e5193e1](https://github.com/OroraTech/nixpkgs/commit/e5193e1) kubernetes-controller-tools: 0.12.1 -&gt; 0.13.0
  * [#3f68347](https://github.com/OroraTech/nixpkgs/commit/3f68347) faketty: 1.0.12 -&gt; 1.0.13

Diff: https://diff.rs/faketty/1.0.12/1.0.13

Changelog: https://github.com/dtolnay/faketty/releases/tag/1.0.13
  * [#9824764](https://github.com/OroraTech/nixpkgs/commit/9824764) open-stage-control: 1.25.2 -&gt; 1.25.3
  * [#1debaa9](https://github.com/OroraTech/nixpkgs/commit/1debaa9) brev-cli: 0.6.252 -&gt; 0.6.259
  * [#6e7daaa](https://github.com/OroraTech/nixpkgs/commit/6e7daaa) risor: 0.15.0 -&gt; 0.17.0

Diff: https://github.com/risor-io/risor/compare/v0.15.0...v0.17.0

Changelog: https://github.com/risor-io/risor/releases/tag/v0.17.0
  * [#744ceae](https://github.com/OroraTech/nixpkgs/commit/744ceae) tegola: 0.17.0 -&gt; 0.18.0
  * [#7f90f3b](https://github.com/OroraTech/nixpkgs/commit/7f90f3b) nixpacks: 1.12.0 -&gt; 1.13.0
  * [#6aea921](https://github.com/OroraTech/nixpkgs/commit/6aea921) napari: 0.4.17 -&gt; 0.4.18
  * [#3d52741](https://github.com/OroraTech/nixpkgs/commit/3d52741) rsyslog: 8.2306.0 -&gt; 8.2308.0
  * *On 1 Sept 2023, 09:03:35*
  * *On 1 Sept 2023, 09:00:25*
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
 <!-- Last activity -->


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.33.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 3 Sept 2023, 07:57:30 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
