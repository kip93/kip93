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

* ➡️ Pushed 722 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#813f5d7](https://github.com/OroraTech/nixpkgs/commit/813f5d7) isocodes: 4.15.0 -&gt; 4.16.0
  * [#5ae7a93](https://github.com/OroraTech/nixpkgs/commit/5ae7a93) attr: 2.5.1 -&gt; 2.5.2
  * [#62d6083](https://github.com/OroraTech/nixpkgs/commit/62d6083) python311Packages.trove-classifiers: 2023.11.29 -&gt; 2024.1.8

Changelog: https://github.com/pypa/trove-classifiers/releases/tag/2024.1.8
  * [#205ccae](https://github.com/OroraTech/nixpkgs/commit/205ccae) qpdf: 11.6.3 -&gt; 11.8.0
  * [#88d193f](https://github.com/OroraTech/nixpkgs/commit/88d193f) iproute2: 6.6.0 -&gt; 6.7.0

Changes: https://lore.kernel.org/netdev/20240108094709.050e22bc@hermes.local/T/
  * [#3ae0f90](https://github.com/OroraTech/nixpkgs/commit/3ae0f90) libedit: 20221030-3.1 -&gt; 20230828-3.1
  * [#612b322](https://github.com/OroraTech/nixpkgs/commit/612b322) enchant: 2.6.3 -&gt; 2.6.5

Changes:
- https://github.com/AbiWord/enchant/releases/tag/v2.6.4
- https://github.com/AbiWord/enchant/releases/tag/v2.6.5
  * [#a9323a3](https://github.com/OroraTech/nixpkgs/commit/a9323a3) p11-kit: fix builds on single-user systems

Add back FAKED_MODE environment variable.
This was removed in 3ca33e5ef4f8c3e24013905cf741330c9ace3a6c, which
caused tests to be run (and fail) that were previously skipped.
  * [#e6d5d5d](https://github.com/OroraTech/nixpkgs/commit/e6d5d5d) pcsclite: disable building pcsc-wirecheck{,-gen} when cross compiling
  * [#572a7c0](https://github.com/OroraTech/nixpkgs/commit/572a7c0) exempi: 2.6.4 -&gt; 2.6.5
  * [#92605d2](https://github.com/OroraTech/nixpkgs/commit/92605d2) alsa-ucm-conf: apply patch to fix SplitPCM: Device argument may not be set
  * [#953f357](https://github.com/OroraTech/nixpkgs/commit/953f357) fdk_aac: 2.0.2 -&gt; 2.0.3
  * [#77536ba](https://github.com/OroraTech/nixpkgs/commit/77536ba) libsepol: 3.5 -&gt; 3.6
  * [#f341406](https://github.com/OroraTech/nixpkgs/commit/f341406) kbd: 2.6.3 -&gt; 2.6.4
  * [#791b761](https://github.com/OroraTech/nixpkgs/commit/791b761) cmake: 3.27.8 -&gt; 3.27.9

Changes: https://github.com/Kitware/CMake/compare/v3.27.8...v3.27.9
  * [#b2d0641](https://github.com/OroraTech/nixpkgs/commit/b2d0641) nix: rebase boehmgc-coroutine-sp-fallback.patch
  * [#f7f4acc](https://github.com/OroraTech/nixpkgs/commit/f7f4acc) boehmgc: 8.2.2 -&gt; 8.2.4
  * [#cbf59c9](https://github.com/OroraTech/nixpkgs/commit/cbf59c9) libipt: 2.0.6 -&gt; 2.1
  * [#dc0f09a](https://github.com/OroraTech/nixpkgs/commit/dc0f09a) zip: fix buffer overflow on Unicode path names

When creating ZIP files with non-ASCII names (such as some European
accent chars), something was detecting a buffer overflow and bailing
out. It turns out that this has been already fixed earlier this year in
Fedora, so let&#39;s reuse their patch as-is.

Bug: https://bugzilla.redhat.com/show_bug.cgi?id=2165653
  * [#0c8f023](https://github.com/OroraTech/nixpkgs/commit/0c8f023) dav1d: 1.2.1 -&gt; 1.3.0
  * *On 10 Feb 2024, 10:53:06*
* 🔃 Opened [#287543 python312Packages.pyuavcan: remove deprecated package](https://github.com/NixOS/nixpkgs/pull/287543) in [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
                * 3 files changed `++1 --62`
  * *On 9 Feb 2024, 18:20:20*
* ⏺️ Created new branch chore/remove-pyuavcan in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs)
  * *On 9 Feb 2024, 17:46:13*
  * *On 9 Feb 2024, 17:14:23*
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 10 Feb 2024, 11:47:49 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
