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

* 🔍 Reviewed [#436761 python3Packages.pycyphal: 1.18.0 -&gt; 1.24.3](https://github.com/NixOS/nixpkgs/pull/436761) in [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  * *On 25 Aug 2025, 16:31:39*
* 🔍 Reviewed [#436761 python3Packages.pycyphal: 1.18.0 -&gt; 1.24.3](https://github.com/NixOS/nixpkgs/pull/436761) in [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  * *On 25 Aug 2025, 15:27:38*
* 🔍 Reviewed [#436199 python3Packages.pkg-about: 1.3.7 -&gt; 1.4.0](https://github.com/NixOS/nixpkgs/pull/436199) in [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  * *On 25 Aug 2025, 14:30:29*
* ➡️ Pushed 17 commits in [kip93/nix](https://github.com/kip93/nix) on branch `master`
  * [#a92a996](https://github.com/kip93/nix/commit/a92a996) Merge pull request #13793 from xokdvium/c++23

treewide: Bump C++ standard version to C++23
  * [#5c0eff2](https://github.com/kip93/nix/commit/5c0eff2) Merge pull request #13784 from NixOS/queryPathInfo-dont-disconnect

Fix client disconnect when queryPathInfo() returns a negative result
  * [#03101cc](https://github.com/kip93/nix/commit/03101cc) treewide: Bump C++ standard version to C++23

Compilers in nixpkgs have caught up and major distros
should also have recent enough compilers. It would be
nice to have newer features like more full featured
ranges and deducing this.
  * [#f3bd18f](https://github.com/kip93/nix/commit/f3bd18f) Merge pull request #13790 from xokdvium/fix-ci

libstore: Fix formatting
  * [#62018b3](https://github.com/kip93/nix/commit/62018b3) libstore: Fix formatting

Wasn&#39;t caught by CI because the PR wasn&#39;t fresh enough
and didn&#39;t have formatting checks enabled.
  * [#dc2478f](https://github.com/kip93/nix/commit/dc2478f) Merge pull request #13340 from mkenigs/better-error

Improve error when can&#39;t acquire db lock
  * [#8283a20](https://github.com/kip93/nix/commit/8283a20) Merge pull request #13789 from xokdvium/nix-2.3-insecure-fix

hydra: Fix otherNixes.nix_2_3
  * [#051290b](https://github.com/kip93/nix/commit/051290b) hydra: Fix otherNixes.nix_2_3

25.05 has it marked as insecure, but we don&#39;t care about it
for testing purposes.
  * [#b263bfc](https://github.com/kip93/nix/commit/b263bfc) Merge pull request #13785 from xokdvium/25.05-nixpkgs

flake: nixpkgs: nixos-unstable -&gt; nixos-25.05-small
  * [#73f6729](https://github.com/kip93/nix/commit/73f6729) git-blame-ignore-revs: Add nixfmt 1.0.0 reformat
  * [#1d943f5](https://github.com/kip93/nix/commit/1d943f5) flake: Apply nixfmt 1.0.0
  * [#aa0dc0d](https://github.com/kip93/nix/commit/aa0dc0d) Merge pull request #13757 from fzakaria/issue-13215

libfetchers/git: add support for &#39;.&#39; in gitmodules
  * [#fc33681](https://github.com/kip93/nix/commit/fc33681) flake: nixpkgs: nixos-unstable -&gt; nixos-25.05-small

About time we upgraded our nixpkgs flake input. Ideally
we&#39;d have automation to do this.

Flake lock file updates:

• Updated input &#39;nixpkgs&#39;:
    &#39;github:NixOS/nixpkgs/adaa24fbf46737f3f1b5497bf64bae750f82942e?narHash=sha256-qhFMmDkeJX9KJwr5H32f1r7Prs7XbQWtO0h3V0a0rFY%3D&#39; (2025-05-13)
  → &#39;github:NixOS/nixpkgs/cd32a774ac52caaa03bcfc9e7591ac8c18617ced?narHash=sha256-VtMQg02B3kt1oejwwrGn50U9Xbjgzfbb5TV5Wtx8dKI%3D&#39; (2025-08-17)
  * [#f51779e](https://github.com/kip93/nix/commit/f51779e) RemoteStore::addToStoreFromDump(): Invalidate cache entry for added path
  * [#c82b67f](https://github.com/kip93/nix/commit/c82b67f) BasicClientConnection::queryPathInfo(): Don&#39;t throw exception for invalid paths

This caused RemoteStore::queryPathInfoUncached() to mark the
connection as invalid (see
RemoteStore::ConnectionHandle::~ConnectionHandle()), causing it to
disconnect and reconnect after every lookup of an invalid path. This
caused huge slowdowns in conjunction with
19f89eb6842747570f262c003d977f02cb155968 and lazy-trees.
  * [#b21304f](https://github.com/kip93/nix/commit/b21304f) libfetchers/git: Add support for &#39;.&#39; in gitsubmodules

Period &#39;.&#39; is a special branch name in the gitsubmodule file which
represents the branch of the parent repository [1].

We add support for this by registering the ref of the InputAccessor to
be that of the parent input if &#39;.&#39; is encountered.

Fixes #13215

[1]: man gitmodules
  * [#d60a8ee](https://github.com/kip93/nix/commit/d60a8ee) Improve database lock permission error context

Add helpful context when opening the Nix database lock fails due to
permission errors. Instead of just showing &#34;Permission denied&#34;, now
provides guidance about possible causes:
- Running as non-root in a single-user Nix installation
- Nix daemon may have crashed
  * *On 19 Aug 2025, 18:19:46*
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 26 Aug 2025, 05:48:42 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
