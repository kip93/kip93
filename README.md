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
* 🔃 Opened [#197247 Documentation: add vmTools](https://github.com/NixOS/nixpkgs/pull/197247) in [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  * 2 files changed `++117 --0`
  * *On 22 Oct 2022, 16:38:25*
* ➡️ Pushed 1 commit in [kip93/nixpkgs](https://github.com/kip93/nixpkgs) on branch `vmTools-docs`
  * [#172fe68](https://github.com/kip93/nixpkgs/commit/172fe68) Remove unused reference
  * *On 22 Oct 2022, 16:36:24*
* ⏺️ Created new branch vmTools-docs in [kip93/nixpkgs](https://github.com/kip93/nixpkgs)
  * *On 22 Oct 2022, 16:27:49*
* ➡️ Pushed 634 commits in [kip93/nixpkgs](https://github.com/kip93/nixpkgs) on branch `master`
  * [#0bea4a1](https://github.com/kip93/nixpkgs/commit/0bea4a1) cc-wrapper/setup-hook.sh: remove duplicate flags in NIX_CFLAGS_COMPILE
  * [#a1801d7](https://github.com/kip93/nixpkgs/commit/a1801d7) apparmor: 3.0.7 -&gt; 3.1.1

https://gitlab.com/apparmor/apparmor/-/wikis/Release_Notes_3.1
  * [#2fc8634](https://github.com/kip93/nixpkgs/commit/2fc8634) dnsmasq: 2.86 -&gt; 2.87
  * [#1220237](https://github.com/kip93/nixpkgs/commit/1220237) libfido2: 1.11.0 -&gt; 1.12.0
  * [#abcaa92](https://github.com/kip93/nixpkgs/commit/abcaa92) openblas: Enable &amp; honour parallel building
  * [#e4e3daf](https://github.com/kip93/nixpkgs/commit/e4e3daf) gpgme: fix i686 build
  * [#8a34b9e](https://github.com/kip93/nixpkgs/commit/8a34b9e) python310Packages.poetry-core: 1.1.0 -&gt; 1.2.0
  * [#d6ef2ac](https://github.com/kip93/nixpkgs/commit/d6ef2ac) popt: 1.18 -&gt; 1.19
  * [#c40a7bf](https://github.com/kip93/nixpkgs/commit/c40a7bf) libsForQt5.plasma-wayland-protocols: 1.7.0 -&gt; 1.8.0
  * [#231bd21](https://github.com/kip93/nixpkgs/commit/231bd21) modemmanager: 1.18.10 -&gt; 1.18.12
  * [#53e860a](https://github.com/kip93/nixpkgs/commit/53e860a) bitwarden: 2022.8.1 -&gt; 2022.9.1
  * [#d8cdbe8](https://github.com/kip93/nixpkgs/commit/d8cdbe8) git: Disable tests that fail on ZFS with formD normalization

These two tests are regularly creating problems for my hydra instance,
because its builders run on ZFS and that makes them fail consistently.

The issue has something to do with unicode normalization. My pools have
formD normalization configured, that might be the culprit in this case.

Closes: #185882
  * [#57b727f](https://github.com/kip93/nixpkgs/commit/57b727f) thc-hydra: 9.3 -&gt; 9.4
  * [#7d731f3](https://github.com/kip93/nixpkgs/commit/7d731f3) nixos/nspawn: Remove not compliant options

The attribute set sharedOptions pulls in not compliant unit options:
- requiredBy
- wantedBy
- aliases

see man5 systemd.nspawn
  * [#96e4a0f](https://github.com/kip93/nixpkgs/commit/96e4a0f) libcxxabi: remove link with build libcxxabi
  * [#fb91bfc](https://github.com/kip93/nixpkgs/commit/fb91bfc) compiler-rt: build builtins on darwin

The missing xcrun meant builtins were missing from darwin. This
apparently wasn&#39;t an issue until now, but is in projects using
`@available` checks. (The ARM64 hack was apparently the previous
solution to fixing broken SDK detection.)
  * [#817ca36](https://github.com/kip93/nixpkgs/commit/817ca36) treewide: change postgresql_10 in documentation and examples to postgresql_14
  * [#aa14831](https://github.com/kip93/nixpkgs/commit/aa14831) postgresql_10: remove ahead of 22.11 release, because it will go EOL 2022-11-10
  * [#71b05ec](https://github.com/kip93/nixpkgs/commit/71b05ec) darwin.cctools: 949.0.1 -&gt; 973.0.1
  * [#1e12026](https://github.com/kip93/nixpkgs/commit/1e12026) libreoffice: fix #152506 - add explicit dependencies on grep and coreutils to wrapper
  * *On 22 Oct 2022, 16:23:57*
 <!-- Last activity -->


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.28.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 24 Oct 2022, 17:59:07 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
