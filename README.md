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

* ➡️ Pushed 123 commits in [kip93/nix](https://github.com/kip93/nix) on branch `lfs`
  * [#4387c5a](https://github.com/kip93/nix/commit/4387c5a) Merge pull request #11894 from myclevorname/nixfmt

doc/nix fmt: Mention nixfmt-rfc-style instead of nixfmt(-classic)
  * [#68e15be](https://github.com/kip93/nix/commit/68e15be) Merge pull request #11844 from roberth/papercut-nix-log

Make nix log command easy to copy
  * [#3f6855c](https://github.com/kip93/nix/commit/3f6855c) doc/nix fmt: Mention nixfmt-rfc-style instead of nixfmt(-classic)
  * [#c9433c0](https://github.com/kip93/nix/commit/c9433c0) .github/ci: Push docker only when test succeeds
  * [#2f3764a](https://github.com/kip93/nix/commit/2f3764a) .github/ci: Add nix-docker test

We still have room to spare in vm_tests, as it&#39;s quicker than `nix flake check`
  * [#3e4a83f](https://github.com/kip93/nix/commit/3e4a83f) Use range-based for
  * [#a2e4a4c](https://github.com/kip93/nix/commit/a2e4a4c) callFunction: Use std::span

This is a bit safer than having a separate nrArgs argument.
  * [#11d3b01](https://github.com/kip93/nix/commit/11d3b01) tests/nixos: add more thorough nix-docker tests
  * [#1dda18e](https://github.com/kip93/nix/commit/1dda18e) doc/manual: add documentation for non-root container images
  * [#1cfb226](https://github.com/kip93/nix/commit/1cfb226) tests/nixos: add nix-docker test
  * [#e194e27](https://github.com/kip93/nix/commit/e194e27) docker: Allow building for non-root user

Add options uid, gid, uname, and gname to docker.nix.

Setting these to e.g. 1000, 1000, &#34;user&#34;, &#34;user&#34; will build an image
which runs and allows using Nix as that user.
  * [#4b44fa0](https://github.com/kip93/nix/commit/4b44fa0) Make nix log command easy to copy on its own line
  * [#5924634](https://github.com/kip93/nix/commit/5924634) Make nix log command easier to copy
  * [#cb0eacc](https://github.com/kip93/nix/commit/cb0eacc) Merge remote-tracking branch &#39;origin/master&#39; into nix-copy-gc
  * [#1c832d6](https://github.com/kip93/nix/commit/1c832d6) Merge remote-tracking branch &#39;origin/master&#39; into nix-copy-gc
  * [#27ea437](https://github.com/kip93/nix/commit/27ea437) Support fine-grained database schema migrations

Backward-compatible schema changes (e.g. those that add tables or
nullable columns) now no longer need a change to the global schema
file (/nix/var/nix/db/schema). Thus, old Nix versions can continue to
access the database.

This is especially useful for schema changes required by experimental
features. In particular, it replaces the ad-hoc handling of the schema
changes for CA derivations (i.e. the file /nix/var/nix/db/ca-schema).

Schema versions 8 and 10 could have been handled by this mechanism in
a backward-compatible way as well.
  * [#e9b5704](https://github.com/kip93/nix/commit/e9b5704) Add release note
  * [#7f6d006](https://github.com/kip93/nix/commit/7f6d006) nix copy: Add --out-link
  * [#43ad8c5](https://github.com/kip93/nix/commit/43ad8c5) Make getDstStore() a virtual method in StoreCommand
  * [#76f75e7](https://github.com/kip93/nix/commit/76f75e7) nix copy: Add --profile flag

This allows `nix copy` to atomically copy a store path and point a
profile to it, without the risk that the store path might be GC&#39;ed in
between. This is useful for instance when deploying a new NixOS system
profile from a remote store.
  * *On 4 Dec 2024, 13:53:24*
* 💬 Commented on [#10153 git-lfs support](https://github.com/NixOS/nix/issues/10153) from [NixOS/nix](https://github.com/NixOS/nix)
  * *On 2 Dec 2024, 20:26:04*
* 💬 Commented on [#10153 git-lfs support](https://github.com/NixOS/nix/issues/10153) from [NixOS/nix](https://github.com/NixOS/nix)
  * *On 2 Dec 2024, 12:19:38*
* 💬 Commented on [#10153 git-lfs support](https://github.com/NixOS/nix/issues/10153) from [NixOS/nix](https://github.com/NixOS/nix)
  * *On 29 Nov 2024, 12:35:57*
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 4 Dec 2024, 23:47:58 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
