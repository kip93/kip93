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


<details> <!-- Last activity -->
<!-- Almost verbatim copy of https://github.com/lowlighter/metrics/blob/latest/source/templates/markdown/partials/activity.ejs, but restructured to be foldable. -->
<summary><h3>📰 Recent activity</h3></summary>

* 💬 Commented on [#79 Non-github flakes?](https://github.com/DeterminateSystems/flakehub-push/issues/79) from [DeterminateSystems/flakehub-push](https://github.com/DeterminateSystems/flakehub-push)
  * *On 21 Sept 2023, 18:07:19*
* 🌟 Starred [direnv/direnv](https://github.com/direnv/direnv)
  * *On 21 Sept 2023, 10:43:46*
* 💬 Commented on [#253261 pkgsNative: init](https://github.com/NixOS/nixpkgs/issues/253261) from [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  * *On 21 Sept 2023, 07:30:16*
* ➡️ Pushed 358 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#25393c5](https://github.com/OroraTech/nixpkgs/commit/25393c5) argocd-autopilot: 0.4.15 -&gt; 0.4.16
  * [#72a455b](https://github.com/OroraTech/nixpkgs/commit/72a455b) jetbrains-rust-rover: init at 232.9921.46(EAP)
  * [#6e05e49](https://github.com/OroraTech/nixpkgs/commit/6e05e49) buildMavenPackage: rename manualMvnArtifactIds to manualMvnArtifacts
  * [#4ec7cd4](https://github.com/OroraTech/nixpkgs/commit/4ec7cd4) buildMavenPackage: hide offline build behind feature flag

The feature flags allows for packages to opt in and should not
break current packages.
  * [#9a7693b](https://github.com/OroraTech/nixpkgs/commit/9a7693b) buildMavenPackage: refactor to run test in drv only

Uses the dependency:go-offline goal in the fixed output derivation to
download all dependencies. As a result, the derivation can be built and
tested offline in the main derivation. The advantage of this approach is
that you don&#39;t need to redownload all dependencies if there are test
failures.
  * [#355cfad](https://github.com/OroraTech/nixpkgs/commit/355cfad) nixos/vikunja: install &#39;vikunja&#39; CLI tool

See https://vikunja.io/docs/cli/
  * [#776debd](https://github.com/OroraTech/nixpkgs/commit/776debd) jamulus: set meta.mainProgram
  * [#7e5a7d1](https://github.com/OroraTech/nixpkgs/commit/7e5a7d1) jamulus: 3.8.2 -&gt; 3.10.0
  * [#6b205f7](https://github.com/OroraTech/nixpkgs/commit/6b205f7) jamulus: reformat function arguments
  * [#f7f848d](https://github.com/OroraTech/nixpkgs/commit/f7f848d) plausible: add softinio as maintainer
  * [#c4244c7](https://github.com/OroraTech/nixpkgs/commit/c4244c7) plausible: 1.5.1 -&gt; 2.0.0

Changelog: https://github.com/plausible/analytics/blob/v2.0.0/CHANGELOG.md

Co-authored-by: Kirill Radzikhovskyy &lt;kirillrdy@gmail.com&gt;
  * [#39a37b7](https://github.com/OroraTech/nixpkgs/commit/39a37b7) pricehist: init at 1.4.6
  * [#a5792e0](https://github.com/OroraTech/nixpkgs/commit/a5792e0) python3Packages.curlify: init at 2.2.1
  * [#e59a84a](https://github.com/OroraTech/nixpkgs/commit/e59a84a) maintainers: add chrpinedo
  * [#54444b5](https://github.com/OroraTech/nixpkgs/commit/54444b5) qgis: add nixos tests

Add NixOS test for QGIS and QGIS-LTR. This test creates QGIS vector
memory layer containing Nix snowflake. This proves that application can
successfully start and Python bindings are working.

By default, Python script is executed in non-interactive mode and QGIS
is closed after script is finished. This script can be also executed
interactively by running following command:

```
 nix-build -A qgis
 QGIS_TEST_INTERACTIVE=True ./result/bin/qgis  --code pkgs/applications/gis/qgis/test.py
```

In this case, QGIS is not automatically closed.
  * [#84347c2](https://github.com/OroraTech/nixpkgs/commit/84347c2) flutter: Use wrapGAppsHook

Flutter&#39;s Linux desktop embedding uses GTK. wrapGAppsHook should be used.
  * [#2c62218](https://github.com/OroraTech/nixpkgs/commit/2c62218) nixos/calibre-web: add package and enableKepubify options
  * [#0df5c9a](https://github.com/OroraTech/nixpkgs/commit/0df5c9a) flutter: Pass through engineArtifacts in wrapper
  * [#75ac518](https://github.com/OroraTech/nixpkgs/commit/75ac518) system-config-printer: 1.5.15 -&gt; 1.5.18
  * [#8a543ac](https://github.com/OroraTech/nixpkgs/commit/8a543ac) lib.systems: add qemu&#39;s funky custom name for mips n32

Qemu&#39;s name for mips64[el] using the n32 ABI is &#34;mipsn32[el]&#34;.
That&#39;s the first time I&#39;ve seen that name for it.  Oh well.
  * *On 21 Sept 2023, 07:27:09*
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 22 Sept 2023, 16:48:12 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
