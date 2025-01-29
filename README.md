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

* 🌟 Starred [qmk/qmk_userspace](https://github.com/qmk/qmk_userspace)
  * *On 28 Jan 2025, 23:57:25*
* ➡️ Pushed 44 commits in [b-camacho/nix](https://github.com/b-camacho/nix) on branch `lfs`
  * [#64a3899](https://github.com/b-camacho/nix/commit/64a3899) Merge pull request #12331 from DeterminateSystems/git-dir

GitRepo::fetch(): Ignore $GIT_DIR
  * [#e0c6ed1](https://github.com/b-camacho/nix/commit/e0c6ed1) Fix help test in dev shell

Not sure what the intent was expecting help.sh to fail in the main suite, but it caused `meson test` to fail inside a `nix develop` shell:

  $ meson test help --print-errorlogs
  ninja: Entering directory `/home/eelco/Dev/nix-master/build&#39;
  1/1 nix-functional-tests:main / help        UNEXPECTEDPASS   4.02s
  * [#41983db](https://github.com/b-camacho/nix/commit/41983db) GitRepo::fetch(): Ignore $GIT_DIR

Fixes #12325.
  * [#bd10b85](https://github.com/b-camacho/nix/commit/bd10b85) GitRepo::fetch(): Cleanup
  * [#2975c2c](https://github.com/b-camacho/nix/commit/2975c2c) Merge pull request #12329 from NixOS/backport

Add mergify backport rule for 2.26
  * [#c5dc749](https://github.com/b-camacho/nix/commit/c5dc749) Add mergify backport rule for 2.26
  * [#a28195d](https://github.com/b-camacho/nix/commit/a28195d) Merge pull request #12328 from NixOS/bump-2.27.0

Bump version
  * [#2d507ff](https://github.com/b-camacho/nix/commit/2d507ff) Merge pull request #12327 from NixOS/update-release-script

Update the release script
  * [#65f95c5](https://github.com/b-camacho/nix/commit/65f95c5) Bump version
  * [#f472be2](https://github.com/b-camacho/nix/commit/f472be2) Update the release script
  * [#7af6329](https://github.com/b-camacho/nix/commit/7af6329) Merge pull request #12326 from NixOS/release-notes

Nix 2.26 release notes
  * [#21f2e29](https://github.com/b-camacho/nix/commit/21f2e29) Add release credits
  * [#617bf84](https://github.com/b-camacho/nix/commit/617bf84) Add a few more release notes
  * [#d8dbb71](https://github.com/b-camacho/nix/commit/d8dbb71) release notes: 2.26.0
  * [#069ca2a](https://github.com/b-camacho/nix/commit/069ca2a) Merge pull request #12324 from NixOS/disable-lto

x86_64-darwin: Disable LTO
  * [#b09b4dc](https://github.com/b-camacho/nix/commit/b09b4dc) x86_64-darwin: Disable LTO

LTO on x86_64-darwin appears to break the ability to catch exceptions
correctly (maybe just for exception types defined in different
libraries). This leads to many weird test failures,
e.g. https://hydra.nixos.org/build/286312387 and
https://hydra.nixos.org/build/286312341.
  * [#b8c296f](https://github.com/b-camacho/nix/commit/b8c296f) Merge pull request #12322 from DeterminateSystems/fix-fetchurl-test

Fix fetchurl test
  * [#9e324df](https://github.com/b-camacho/nix/commit/9e324df) Fix fetchurl test

https://hydra.nixos.org/build/286311974
  * [#27c9f7e](https://github.com/b-camacho/nix/commit/27c9f7e) Fix name
  * [#69fde53](https://github.com/b-camacho/nix/commit/69fde53) Clean up packaging a bit

- Multiple choices of stdenv are handled more consistently, especially for the dev
  shells which were previously not done correctly.

- Some stray nix code was moving into the `packaging` directory
  * *On 27 Jan 2025, 14:46:45*
* ➡️ Pushed 44 commits in [kip93/nix](https://github.com/kip93/nix) on branch `lfs`
  * [#64a3899](https://github.com/kip93/nix/commit/64a3899) Merge pull request #12331 from DeterminateSystems/git-dir

GitRepo::fetch(): Ignore $GIT_DIR
  * [#e0c6ed1](https://github.com/kip93/nix/commit/e0c6ed1) Fix help test in dev shell

Not sure what the intent was expecting help.sh to fail in the main suite, but it caused `meson test` to fail inside a `nix develop` shell:

  $ meson test help --print-errorlogs
  ninja: Entering directory `/home/eelco/Dev/nix-master/build&#39;
  1/1 nix-functional-tests:main / help        UNEXPECTEDPASS   4.02s
  * [#41983db](https://github.com/kip93/nix/commit/41983db) GitRepo::fetch(): Ignore $GIT_DIR

Fixes #12325.
  * [#bd10b85](https://github.com/kip93/nix/commit/bd10b85) GitRepo::fetch(): Cleanup
  * [#2975c2c](https://github.com/kip93/nix/commit/2975c2c) Merge pull request #12329 from NixOS/backport

Add mergify backport rule for 2.26
  * [#c5dc749](https://github.com/kip93/nix/commit/c5dc749) Add mergify backport rule for 2.26
  * [#a28195d](https://github.com/kip93/nix/commit/a28195d) Merge pull request #12328 from NixOS/bump-2.27.0

Bump version
  * [#2d507ff](https://github.com/kip93/nix/commit/2d507ff) Merge pull request #12327 from NixOS/update-release-script

Update the release script
  * [#65f95c5](https://github.com/kip93/nix/commit/65f95c5) Bump version
  * [#f472be2](https://github.com/kip93/nix/commit/f472be2) Update the release script
  * [#7af6329](https://github.com/kip93/nix/commit/7af6329) Merge pull request #12326 from NixOS/release-notes

Nix 2.26 release notes
  * [#21f2e29](https://github.com/kip93/nix/commit/21f2e29) Add release credits
  * [#617bf84](https://github.com/kip93/nix/commit/617bf84) Add a few more release notes
  * [#d8dbb71](https://github.com/kip93/nix/commit/d8dbb71) release notes: 2.26.0
  * [#069ca2a](https://github.com/kip93/nix/commit/069ca2a) Merge pull request #12324 from NixOS/disable-lto

x86_64-darwin: Disable LTO
  * [#b09b4dc](https://github.com/kip93/nix/commit/b09b4dc) x86_64-darwin: Disable LTO

LTO on x86_64-darwin appears to break the ability to catch exceptions
correctly (maybe just for exception types defined in different
libraries). This leads to many weird test failures,
e.g. https://hydra.nixos.org/build/286312387 and
https://hydra.nixos.org/build/286312341.
  * [#b8c296f](https://github.com/kip93/nix/commit/b8c296f) Merge pull request #12322 from DeterminateSystems/fix-fetchurl-test

Fix fetchurl test
  * [#9e324df](https://github.com/kip93/nix/commit/9e324df) Fix fetchurl test

https://hydra.nixos.org/build/286311974
  * [#27c9f7e](https://github.com/kip93/nix/commit/27c9f7e) Fix name
  * [#69fde53](https://github.com/kip93/nix/commit/69fde53) Clean up packaging a bit

- Multiple choices of stdenv are handled more consistently, especially for the dev
  shells which were previously not done correctly.

- Some stray nix code was moving into the `packaging` directory
  * *On 27 Jan 2025, 14:46:40*
* ➡️ Pushed 394 commits in [kip93/nix](https://github.com/kip93/nix) on branch `master`
  * [#a2e4a4c](https://github.com/kip93/nix/commit/a2e4a4c) callFunction: Use std::span

This is a bit safer than having a separate nrArgs argument.
  * [#11d3b01](https://github.com/kip93/nix/commit/11d3b01) tests/nixos: add more thorough nix-docker tests
  * [#1dda18e](https://github.com/kip93/nix/commit/1dda18e) doc/manual: add documentation for non-root container images
  * [#1cfb226](https://github.com/kip93/nix/commit/1cfb226) tests/nixos: add nix-docker test
  * [#e194e27](https://github.com/kip93/nix/commit/e194e27) docker: Allow building for non-root user

Add options uid, gid, uname, and gname to docker.nix.

Setting these to e.g. 1000, 1000, &#34;user&#34;, &#34;user&#34; will build an image
which runs and allows using Nix as that user.
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
  * [#f206325](https://github.com/kip93/nix/commit/f206325) tests/functional/flakes/relative-paths.sh: Fix build failure in hydraJobs.tests.functional_user
  * [#91e7d49](https://github.com/kip93/nix/commit/91e7d49) Merge remote-tracking branch &#39;origin/master&#39; into relative-flakes
  * [#71d4bb8](https://github.com/kip93/nix/commit/71d4bb8) parentPath -&gt; parentInputPath
  * [#09d7197](https://github.com/kip93/nix/commit/09d7197) shellcheck
  * [#21fc07c](https://github.com/kip93/nix/commit/21fc07c) Merge remote-tracking branch &#39;origin/master&#39; into relative-flakes
  * [#3180671](https://github.com/kip93/nix/commit/3180671) Allow the &#39;url&#39; flake input attribute to be a path literal

https://github.com/NixOS/nix/pull/10089#issuecomment-1978133326
  * [#49f592d](https://github.com/kip93/nix/commit/49f592d) call-flake.nix: Fix relative path resolution

`parentNode.sourceInfo.outPath` does not include the subdir of the
parent flake, while `parentNode.outPath` does. So we need to use the
latter.
  * [#b2be6fe](https://github.com/kip93/nix/commit/b2be6fe) Improve support for subflakes

Subflakes are flakes in the same tree, accessed in flake inputs via
relative paths (e.g. `inputs.foo.url = &#34;path:./subdir&#34;`). Previously
these didn&#39;t work very well because they would be separately copied to
the store, which is inefficient and makes references to parent
directories tricky or impossible. Furthermore, they had their own NAR
hash in the lock file, which is superfluous since the parent is
already locked.

Now subflakes are accessed via the accessor of the calling flake. This
avoids the unnecessary copy and makes it possible for subflakes to
depend on flakes in a parent directory (so long as they&#39;re in the same
tree).

Lock file nodes for relative flake inputs now have a new `parent` field:

  {
    &#34;locked&#34;: {
      &#34;path&#34;: &#34;./subdir&#34;,
      &#34;type&#34;: &#34;path&#34;
    },
    &#34;original&#34;: {
      &#34;path&#34;: &#34;./subdir&#34;,
      &#34;type&#34;: &#34;path&#34;
    },
    &#34;parent&#34;: [
      &#34;foo&#34;,
      &#34;bar&#34;
    ]
  }

which denotes that `./subdir` is to be interpreted relative to the
directory of the `bar` input of the `foo` input of the root flake.

Extracted from the lazy-trees branch.
  * *On 21 Jan 2025, 17:28:48*
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 29 Jan 2025, 13:48:20 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
