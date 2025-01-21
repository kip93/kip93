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

* 💬 Commented on [#10153 git-lfs support](https://github.com/NixOS/nix/pull/10153) from [NixOS/nix](https://github.com/NixOS/nix)
  * *On 21 Jan 2025, 15:59:22*
* 🔍 Reviewed [#10153 git-lfs support](https://github.com/NixOS/nix/pull/10153) in [NixOS/nix](https://github.com/NixOS/nix)
  * *On 21 Jan 2025, 15:59:23*
* ➡️ Pushed 110 commits in [b-camacho/nix](https://github.com/b-camacho/nix) on branch `lfs`
  * [#ed4f2c3](https://github.com/b-camacho/nix/commit/ed4f2c3) scripts/install-darwin-multi-user: workaround dscl failing sometimes
  * [#d329b26](https://github.com/b-camacho/nix/commit/d329b26) Fix manual
  * [#ef2739b](https://github.com/b-camacho/nix/commit/ef2739b) Example of referencing parent directories
  * [#0792152](https://github.com/b-camacho/nix/commit/0792152) Rename Override -&gt; OverrideTarget
  * [#e8c7dd9](https://github.com/b-camacho/nix/commit/e8c7dd9) Rename allowRelative -&gt; preserveRelativePaths
  * [#75cda2d](https://github.com/b-camacho/nix/commit/75cda2d) Document path values in inputs

Co-authored-by: Robert Hensing &lt;roberth@users.noreply.github.com&gt;
  * [#01c96f9](https://github.com/b-camacho/nix/commit/01c96f9) libmain: fix ignoring empty lines in the print-build-logs option
  * [#9223d64](https://github.com/b-camacho/nix/commit/9223d64) Remove dead code
  * [#8534c42](https://github.com/b-camacho/nix/commit/8534c42) Merge remote-tracking branch &#39;origin/master&#39; into relative-flakes
  * [#985b2f9](https://github.com/b-camacho/nix/commit/985b2f9) Remove FIXME
  * [#00b99b8](https://github.com/b-camacho/nix/commit/00b99b8) Remove FIXME
  * [#0b00bf7](https://github.com/b-camacho/nix/commit/0b00bf7) Merge remote-tracking branch &#39;origin/master&#39; into relative-flakes
  * [#f206325](https://github.com/b-camacho/nix/commit/f206325) tests/functional/flakes/relative-paths.sh: Fix build failure in hydraJobs.tests.functional_user
  * [#91e7d49](https://github.com/b-camacho/nix/commit/91e7d49) Merge remote-tracking branch &#39;origin/master&#39; into relative-flakes
  * [#71d4bb8](https://github.com/b-camacho/nix/commit/71d4bb8) parentPath -&gt; parentInputPath
  * [#09d7197](https://github.com/b-camacho/nix/commit/09d7197) shellcheck
  * [#21fc07c](https://github.com/b-camacho/nix/commit/21fc07c) Merge remote-tracking branch &#39;origin/master&#39; into relative-flakes
  * [#3180671](https://github.com/b-camacho/nix/commit/3180671) Allow the &#39;url&#39; flake input attribute to be a path literal

https://github.com/NixOS/nix/pull/10089#issuecomment-1978133326
  * [#49f592d](https://github.com/b-camacho/nix/commit/49f592d) call-flake.nix: Fix relative path resolution

`parentNode.sourceInfo.outPath` does not include the subdir of the
parent flake, while `parentNode.outPath` does. So we need to use the
latter.
  * [#b2be6fe](https://github.com/b-camacho/nix/commit/b2be6fe) Improve support for subflakes

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
  * *On 21 Jan 2025, 15:58:09*
* ➡️ Pushed 110 commits in [kip93/nix](https://github.com/kip93/nix) on branch `lfs`
  * [#ed4f2c3](https://github.com/kip93/nix/commit/ed4f2c3) scripts/install-darwin-multi-user: workaround dscl failing sometimes
  * [#d329b26](https://github.com/kip93/nix/commit/d329b26) Fix manual
  * [#ef2739b](https://github.com/kip93/nix/commit/ef2739b) Example of referencing parent directories
  * [#0792152](https://github.com/kip93/nix/commit/0792152) Rename Override -&gt; OverrideTarget
  * [#e8c7dd9](https://github.com/kip93/nix/commit/e8c7dd9) Rename allowRelative -&gt; preserveRelativePaths
  * [#75cda2d](https://github.com/kip93/nix/commit/75cda2d) Document path values in inputs

Co-authored-by: Robert Hensing &lt;roberth@users.noreply.github.com&gt;
  * [#01c96f9](https://github.com/kip93/nix/commit/01c96f9) libmain: fix ignoring empty lines in the print-build-logs option
  * [#9223d64](https://github.com/kip93/nix/commit/9223d64) Remove dead code
  * [#8534c42](https://github.com/kip93/nix/commit/8534c42) Merge remote-tracking branch &#39;origin/master&#39; into relative-flakes
  * [#985b2f9](https://github.com/kip93/nix/commit/985b2f9) Remove FIXME
  * [#00b99b8](https://github.com/kip93/nix/commit/00b99b8) Remove FIXME
  * [#0b00bf7](https://github.com/kip93/nix/commit/0b00bf7) Merge remote-tracking branch &#39;origin/master&#39; into relative-flakes
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
  * *On 21 Jan 2025, 15:58:04*
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 21 Jan 2025, 19:47:49 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
